# ⚡ FastAPI Learning Repository

> A personal learning repository created while exploring FastAPI deeply.

Hello 👋  
My name is **Krishnamohan Yagneswaran**.  

I am currently learning **FastAPI** and building this repository as a structured way to understand core backend concepts like:

- Sync vs Async
- ASGI vs WSGI
- Request/Response lifecycle
- Validation
- Dependency Injection
- Authentication
- Database integration
- Deployment basics

This repository will continuously evolve.  

If I learn something new, I will update this repo.  
If you know something useful, feel free to contribute.

This is not a finished product — it is a living learning document.

---

# 🚀 What is FastAPI?

**FastAPI** is a modern, high-performance web framework for building APIs with Python.

It is:

- Built on Starlette (ASGI framework)
- Uses Pydantic for validation
- Async-ready
- Extremely fast
- Automatically generates API documentation

Why it is popular:

- Very clean syntax
- Built-in validation
- Automatic Swagger documentation
- Strong type-based development
- Production ready

---

# 🧠 Learning Roadmap

## 1️⃣ Python Foundations (Required Before FastAPI)

- Functions
- Classes
- Type hints
- Virtual environments
- JSON handling
- Basic HTTP methods

---

## 2️⃣ ASGI vs WSGI

| Feature | WSGI | ASGI |
|----------|--------|--------|
| Sync | ✅ | ✅ |
| Async | ❌ | ✅ |
| WebSockets | ❌ | ✅ |

FastAPI runs on ASGI servers like:

- Uvicorn
- Hypercorn

Understanding this difference is important before learning async.

---

## 3️⃣ Sync vs Async (Very Important Concept)

### Sync (`def`)

- Blocking
- One request handled at a time
- Easier to understand

### Async (`async def`)

- Non-blocking
- Better for I/O operations
- Handles multiple requests efficiently

Example:

```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/sync")
def sync_route():
    return {"message": "This is sync"}

@app.get("/async")
async def async_route():
    return {"message": "This is async"}
