# ⚡ FastAPI Learning Repository – Beginner to Advanced Guide

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-Learning-green)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Contributions](https://img.shields.io/badge/Contributions-Welcome-orange)
![Stars](https://img.shields.io/badge/Support-Give%20a%20Star-yellow)

> A structured **FastAPI tutorial and learning roadmap** covering async programming, ASGI architecture, backend fundamentals, and scalable API development.

Hello 👋  
My name is **Krishnamohan Yagneswaran**.

This repository is my personal **FastAPI learning guide**, created to deeply understand modern backend development using Python.

It is designed as a:

- FastAPI beginner guide  
- FastAPI roadmap  
- FastAPI async vs sync explanation  
- Backend API architecture reference  
- Structured documentation resource  

---

# 🚀 What You Will Learn in This FastAPI Guide

This repository covers important FastAPI and backend development concepts including:

- Sync vs Async in Python  
- ASGI vs WSGI architecture  
- FastAPI request/response lifecycle  
- Pydantic validation  
- Dependency Injection  
- Authentication (JWT, OAuth concepts)  
- Database integration (SQL & NoSQL basics)  
- Deployment fundamentals  
- Scalable backend architecture principles  

This is not just a tutorial — it is a structured backend knowledge base.

---

# 🧠 Who Is This Repository For?

- Beginners learning FastAPI  
- Developers transitioning from Flask/Django  
- Students learning backend development  
- Developers wanting to understand async programming  
- Anyone building REST APIs with Python  

---

# 📚 FastAPI Documentation & Deep Explanations

All detailed explanations, architecture notes, and structured breakdowns are available inside the **Wiki pages** of this repository.

The Wiki includes:

- FastAPI engine explanation  
- Async vs Sync deep dive  
- ASGI server understanding  
- Internal request flow  
- Architecture concepts  

👉 Please check the **Wiki tab** for in-depth explanations and structured documentation.

---

import { useEffect, useRef, useState } from "react";
import { LABELS } from "../data/survey";

export default function VoiceInput({ language, setValue }) {
  const recognitionRef = useRef(null);
  const finalTextRef = useRef(""); // stores accumulated text
  const recordingRef = useRef(false);
  const updateTimerRef = useRef(null);

  const mediaRecorderRef = useRef(null);
  const audioChunksRef = useRef([]);

  const [supported, setSupported] = useState(false);
  const [recording, setRecording] = useState(false);
  const [micStatus, setMicStatus] = useState("idle"); 
  // idle | listening | hearing | paused | error

  const uiLang = language === "ta" ? "ta" : "en";
  const speechLang = language === "ta" ? "ta-IN" : "en-IN";

  useEffect(() => {
    const SpeechRecognition =
      window.SpeechRecognition || window.webkitSpeechRecognition;

    if (!SpeechRecognition) {
      setSupported(false);
      return;
    }

    const recognition = new SpeechRecognition();
    recognition.continuous = true;
    recognition.interimResults = true;
    recognition.lang = speechLang;

    recognition.onresult = (event) => {
      let interim = "";
      setMicStatus("hearing");

      for (let i = event.resultIndex; i < event.results.length; i++) {
        const text = event.results[i][0].transcript;

        if (event.results[i].isFinal) {
          finalTextRef.current += text.trim() + " ";
        } else {
          interim += text;
        }
      }

      clearTimeout(updateTimerRef.current);
      updateTimerRef.current = setTimeout(() => {
        setValue((finalTextRef.current + interim).trim());
      }, 200);
    };

    recognition.onaudiostart = () => setMicStatus("listening");
    recognition.onspeechend = () => setMicStatus("paused");
    recognition.onerror = () => setMicStatus("error");

    recognition.onend = () => {
      if (recordingRef.current) {
        setTimeout(() => {
          try {
            recognition.start();
          } catch {}
        }, 400);
      }
    };

    recognitionRef.current = recognition;
    setSupported(true);

    return () => {
      recordingRef.current = false;
      recognition.stop();
    };
  }, [language, setValue]);

  if (!supported) return null;

  const startRecording = async () => {
    if (recording) return;

    // ✅ DO NOT clear text
    // Instead, continue from what user already has
    finalTextRef.current = finalTextRef.current || "";

    recordingRef.current = true;
    setRecording(true);
    setMicStatus("listening");

    try {
      recognitionRef.current.start();
    } catch {}

    const stream = await navigator.mediaDevices.getUserMedia({ audio: true });
    const mediaRecorder = new MediaRecorder(stream);

    audioChunksRef.current = [];

    mediaRecorder.ondataavailable = (e) => {
      if (e.data.size > 0) audioChunksRef.current.push(e.data);
    };

    mediaRecorder.start();
    mediaRecorderRef.current = mediaRecorder;
  };

  const stopRecording = () => {
    recordingRef.current = false;
    setRecording(false);
    setMicStatus("idle");

    recognitionRef.current?.stop();
    mediaRecorderRef.current?.stop();

    mediaRecorderRef.current.onstop = async () => {
      const audioBlob = new Blob(audioChunksRef.current, {
        type: "audio/webm",
      });

      const formData = new FormData();
      formData.append("audio", audioBlob);

      const res = await fetch("/api/speech-to-text", {
        method: "POST",
        body: formData,
      });

      const data = await res.json();

      if (data?.text) {
        // ✅ Append backend text, do not overwrite
        finalTextRef.current += data.text.trim() + " ";
        setValue(finalTextRef.current.trim());
      }
    };
  };

  return (
    <div style={{ marginTop: 8 }}>
      {!recording ? (
        <button className="secondary" onClick={startRecording}>
          {LABELS[uiLang]?.ui?.start_voice || "🎙️ Start Voice Input"}
        </button>
      ) : (
        <button className="secondary" onClick={stopRecording}>
          {LABELS[uiLang]?.ui?.stop_voice || "⏹ Stop Recording"}
        </button>
      )}

      <div style={{ marginTop: 6, fontSize: 13 }}>
        {micStatus === "idle" && "🎤 Mic ready"}
        {micStatus === "listening" && "🔴 Listening…"}
        {micStatus === "hearing" && "🟢 Hearing voice"}
        {micStatus === "paused" && "⏸️ Paused"}
        {micStatus === "error" && "❌ Mic error"}
      </div>
    </div>
  );
}



# 🔍 Keywords Covered in This Repository

FastAPI tutorial  
FastAPI roadmap  
FastAPI for beginners  
Async vs Sync Python  
ASGI server explained  
FastAPI architecture  
Python backend development  
REST API with FastAPI  
FastAPI best practices  

---

# ⭐ Support This FastAPI Learning Project

If you find this repository helpful:

- Give it a ⭐ star  
- Share it with other developers  
- Contribute improvements  
- Suggest better explanations  

Your support motivates me to keep learning and expanding this FastAPI guide 🚀

---

Built and maintained by  
**Krishnamohan Yagneswaran**
