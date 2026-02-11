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

Third-Party Extensions
Admin
FastAPI Admin - Functional admin panel that provides a user interface for performing CRUD operations on your data. Currently only works with the Tortoise ORM.
FastAPI Amis Admin - A high-performance, efficient and easily extensible FastAPI admin framework.
Piccolo Admin - A powerful and modern admin GUI, using the Piccolo ORM.
SQLAlchemy Admin - Admin Panel for FastAPI/Starlette that works with SQLAlchemy models.
Starlette Admin - Admin framework for FastAPI/Starlette, supporting SQLAlchemy, SQLModel, MongoDB, and ODMantic.
Auth
AuthX - Customizable Authentications and Oauth2 management for FastAPI.
FastAPI Auth - Pluggable auth that supports the OAuth2 Password Flow with JWT access and refresh tokens.
FastAPI Azure Auth - Azure AD authentication for your APIs with single and multi tenant support.
FastAPI Cloud Auth - Simple integration between FastAPI and cloud authentication services (AWS Cognito, Auth0, Firebase Authentication).
FastAPI Login - Account management and authentication (based on Flask-Login).
FastAPI JWT Auth - JWT auth (based on Flask-JWT-Extended).
FastAPI Permissions - Row-level permissions.
FastAPI Security - Implements authentication and authorization as dependencies in FastAPI.
FastAPI Simple Security - Out-of-the-box API key security manageable through path operations.
FastAPI Users - Account management, authentication, authorization.
Databases
ORMs
Edgy ORM - Complex databases made simple.
FastAPI SQLAlchemy - Simple integration between FastAPI and SQLAlchemy.
Fastapi-SQLA - SQLAlchemy extension for FastAPI with support for pagination, asyncio, and pytest.
FastAPIwee - A simple way to create REST API based on PeeWee models.
GINO - A lightweight asynchronous ORM built on top of SQLAlchemy core for Python asyncio.
FastAPI Example
ORM - An async ORM.
ormar - Ormar is an async ORM that uses Pydantic validation and can be used directly in FastAPI requests and responses so you are left with only one set of models to maintain. Alembic migrations included.
FastAPI Example - Using FastAPI with ormar.
Piccolo - An async ORM and query builder, supporting Postgres and SQLite, with batteries (migrations, security, etc).
FastAPI Examples - Using FastAPI with Piccolo.
Prisma Client Python - An auto-generated, fully type safe ORM powered by Pydantic and tailored specifically for your schema - supports SQLite, PostgreSQL, MySQL, MongoDB, MariaDB and more.
FastAPI Example
Tortoise ORM - An easy-to-use asyncio ORM (Object Relational Mapper) inspired by Django.
FastAPI Example - An example of the Tortoise-ORM FastAPI integration.
Tutorial: Setting up Tortoise ORM with FastAPI
Aerich - Tortoise ORM migrations tools.
Saffier ORM - The only Python ORM you will ever need.
SQLModel - SQLModel (which is powered by Pydantic and SQLAlchemy) is a library for interacting with SQL databases from Python code, with Python objects.
Query Builders
asyncpgsa - A wrapper around asyncpg for use with SQLAlchemy Core.
Databases - Async SQL query builder that works on top of the SQLAlchemy Core expression language.
PyPika - A SQL query builder that exposes the full richness of the SQL language.
ODMs
Beanie - Asynchronous Python ODM for MongoDB, based on Motor and Pydantic, which supports data and schema migrations out of the box.
MongoEngine - A Document-Object Mapper (think ORM, but for document databases) for working with MongoDB from Python.
Motor - Asynchronous Python driver for MongoDB.
ODMantic - AsyncIO MongoDB ODM integrated with Pydantic.
PynamoDB - A pythonic interface to Amazon's DynamoDB.
Other Tools
Pydantic-SQLAlchemy - Convert SQLAlchemy models to Pydantic models.
FastAPI-CamelCase - CamelCase JSON support for FastAPI utilizing Pydantic.
CamelCase Models with FastAPI and Pydantic - Accompanying blog post from the author of the extension.
Dependency Injection
Wireup - Inject dependencies with zero runtime overhead in FastAPI; Share dependencies across web, cli or other interfaces.
Developer Tools
FastAPI Code Generator - Create a FastAPI app from an OpenAPI file, enabling schema-driven development.
FastAPI Client Generator - Generate a mypy- and IDE-friendly API client from an OpenAPI spec.
FastAPI Cruddy Framework - A companion library to FastAPI designed to bring the development productivity of Ruby on Rails, Ember.js or Sails.js to the FastAPI ecosystem.
FastAPI MVC - Developer productivity tool for making high-quality FastAPI production-ready APIs.
FastAPI Profiler - A FastAPI Middleware of joerick/pyinstrument to check your service performance.
FastAPI Versioning - API versioning.
Jupyter Notebook REST API - Run your Jupyter notebooks as RESTful API endpoints.
Manage FastAPI - CLI tool for generating and managing FastAPI projects.
msgpack-asgi - Automatic MessagePack content negotiation.
Email
FastAPI Mail - Lightweight mail system for sending emails and attachments (individual and bulk).
Utils
Apitally - API analytics, monitoring, and request logging for FastAPI.
ASGI Correlation ID - Request ID logging middleware.
FastAPI Cache - A simple lightweight cache system.
FastAPI Cache - A tool to cache FastAPI response and function results, with support for Redis, Memcached, DynamoDB, and in-memory backends.
FastAPI Chameleon - Adds integration of the Chameleon template language to FastAPI.
FastAPI CloudEvents - CloudEvents integration for FastAPI.
FastAPI Contrib - Opinionated set of utilities: pagination, auth middleware, permissions, custom exception handlers, MongoDB support, and Opentracing middleware.
FastAPI FastCRUD) - Robust async CRUD operations and flexible endpoint creation utilities.
FastAPI Events - Asynchronous event dispatching/handling library for FastAPI and Starlette.
FastAPI FeatureFlags - Simple implementation of feature flags for FastAPI.
FastAPI Injectable - Use FastAPI's dependency injection outside route handlers in CLI tools, background tasks, workers, and more.
FastAPI Jinja - Adds integration of the Jinja template language to FastAPI.
FastAPI Lazy - Lazy package to start your project using FastAPI.
FastAPI Limiter - A request rate limiter for FastAPI.
FastAPI Listing - A library to design/build listing APIs using component-based architecture, inbuilt query paginator, sorter, django-admin like filters & much more.
FastAPI MQTT - An extension for the MQTT protocol.
FastAPI Opentracing - Opentracing middleware and database tracing support for FastAPI.
FastAPI Pagination - Pagination for FastAPI.
FastAPI Plugins - Redis and Scheduler plugins.
FastAPI ServiceUtils - Generator for creating API services.
FastAPI SocketIO - Easy integration for FastAPI and SocketIO.
FastAPI Utilities - Reusable utilities: class-based views, response inferring router, periodic tasks, timing middleware, SQLAlchemy session, OpenAPI spec simplification.
FastAPI Websocket Pub/Sub - The classic pub/sub pattern made easily accessible and scalable over the web and across your cloud in realtime.
FastAPI Websocket RPC - RPC (bidirectional JSON RPC) over Websockets made easy, robust, and production ready.
OpenTelemetry FastAPI Instrumentation - Library provides automatic and manual instrumentation of FastAPI web frameworks, instrumenting http requests served by applications utilizing the framework.
Prerender Python Starlette - Starlette middleware for Prerender.
Prometheus FastAPI Instrumentator - A configurable and modular Prometheus Instrumentator for your FastAPI application.
SlowApi - Rate limiter (based on Flask-Limiter).
Starlette Context - Allows you to store and access the request data anywhere in your project, useful for logging.
Starlette Exporter - One more prometheus integration for FastAPI and Starlette.
Starlette OpenTracing - Opentracing support for Starlette and FastAPI.
Starlette Prometheus - Prometheus integration for FastAPI and Starlette.
Strawberry GraphQL - Python GraphQL library based on dataclasses.
Resources
Official Resources
Documentation - Comprehensive documentation.
Tutorial - Official tutorial showing you how to use FastAPI with most of its features, step by step.
Source Code - Hosted on GitHub.
Discord - Chat with other FastAPI users.
External Resources
TestDriven.io FastAPI - Multiple FastAPI-specific articles that focus on developing and testing production-ready RESTful APIs, serving up machine learning models, and more.
Podcasts
Build The Next Generation Of Python Web Applications With FastAPI - In this episode of Podcast Init, the creator of FastAPI, Sebastián Ramirez, shares his motivations for building FastAPI and how it works under the hood.
FastAPI on PythonBytes - Nice overview of the project.
Articles
FastAPI has Ruined Flask Forever for Me
Why we switched from Flask to FastAPI for production machine learning - In-depth look at why you may want to move from Flask to FastAPI.
Tutorials
Async SQLAlchemy with FastAPI - Learn how to use SQLAlchemy asynchronously.
Deploy Machine Learning Models with Keras, FastAPI, Redis and Docker
Developing and Testing an Asynchronous API with FastAPI and Pytest - Develop and test an asynchronous API with FastAPI, Postgres, Pytest, and Docker using Test-Driven Development.
FastAPI for Flask Users - Learn FastAPI with a side-by-side code comparison to Flask.
Implementing FastAPI Services – Abstraction and Separation of Concerns - FastAPI application and service structure for a more maintainable codebase.
Introducing FARM Stack - FastAPI, React, and MongoDB - Getting started with a complete FastAPI web application stack.
Multitenancy with FastAPI, SQLAlchemy and PostgreSQL - Learn how to make FastAPI applications multi-tenant ready.
Porting Flask to FastAPI for ML Model Serving - Comparison of Flask vs FastAPI.
Real-time data streaming using FastAPI and WebSockets - Learn how to stream data from FastAPI directly into a real-time chart.
Running FastAPI applications in production - Use Gunicorn with systemd for production deployments.
Serving Machine Learning Models with FastAPI in Python - Use FastAPI to quickly and easily deploy and serve machine learning models in Python as a RESTful API.
Streaming video with FastAPI - Learn how to serve video streams.
Using Hypothesis and Schemathesis to Test FastAPI - Apply property-based testing to FastAPI.
Talks
PyConBY 2020: Serve ML models easily with FastAPI - From the talk by Sebastian Ramirez you will learn how to easily build a production-ready web (JSON) API for your ML models with FastAPI, including best practices by default.
PyCon UK 2019: FastAPI from the ground up - This talk shows how to build a simple REST API for a database from the ground up using FastAPI.
Videos
Building a Stock Screener with FastAPI - A you build a web-based stock screener with FastAPI, you'll be introduced to many of FastAPI's features, including Pydantic models, dependency injection, background tasks, and SQLAlchemy integration.
Building Web APIs Using FastAPI - Use FastAPI to build a web application programming interface (RESTful API).
FastAPI - A Web Framework for Python - See how to do numeric validations with FastAPI.
FastAPI vs. Django vs. Flask - Which framework is best for Python in 2020? Which uses async/await the best? Which is the fastest?
Serving Machine Learning Models As API with FastAPI - Build a machine learning API with FastAPI.
Courses
Test-Driven Development with FastAPI and Docker - Learn how to build, test, and deploy a text summarization microservice with Python, FastAPI, and Docker.
Modern APIs with FastAPI and Python - A course designed to get you creating new APIs running in the cloud with FastAPI quickly.
Full Web Apps with FastAPI Course - You'll learn to build full web apps with FastAPI, equivalent to what you can do with Flask or Django.
The Definitive Guide to Celery and FastAPI - Learn how to add Celery to a FastAPI application to provide asynchronous task processing.
Best Practices
FastAPI Best Practices - Collection of best practices in a GitHub repo.
FastAPI-Dishka-FastStream - Combines FastAPI, dishka, faststream, sqlalchemy, pydantic.
Hosting
PaaS
(Platforms-as-a-Service)

AWS Elastic Beanstalk
Deta (example)
Fly (tutorial, Deploy from a Git repo)
Google App Engine
Heroku (Step-by-step tutorial, ML model on Heroku tutorial)
Microsoft Azure App Service
IaaS
(Infrastructure-as-a-Service)

AWS EC2
Google Compute Engine
Digital Ocean
Linode
Serverless
Frameworks:

Chalice
Mangum - Adapter for running ASGI applications with AWS Lambda and API Gateway.
Vercel - (formerly Zeit) (example).
Compute:

AWS Lambda (example)
Google Cloud Functions
Azure Functions
Google Cloud Run (example)
Projects
Boilerplate
Full Stack FastAPI and PostgreSQL - Base Project Generator - Full Stack FastAPI Template , which includes FastAPI, React, SQLModel, PostgreSQL, Docker, GitHub Actions, automatic HTTPS, and more (developed by the creator of FastAPI, Sebastián Ramírez).
FastAPI and Tortoise ORM - Powerful but simple template for web APIs w/ FastAPI (as web framework) and Tortoise-ORM (for working via database without headache).
FastAPI Model Server Skeleton - Skeleton app to serve machine learning models production-ready.
cookiecutter-spacy-fastapi - Quick deployments of spaCy models with FastAPI.
cookiecutter-fastapi - Cookiecutter template for FastAPI projects using: Machine Learning, Poetry, Azure Pipelines and pytest.
openapi-python-client - Generate modern FastAPI Python clients (via FastAPI) from OpenAPI.
Pywork - Yeoman generator to scaffold a FastAPI app.
fastapi-gino-arq-uvicorn - Template for a high-performance async REST API, in Python. FastAPI + GINO + Arq + Uvicorn (w/ Redis and PostgreSQL).
FastAPI and React Template - Full stack cookiecutter boilerplate using FastAPI, TypeScript, Docker, PostgreSQL, and React.
FastAPI Nano - Simple FastAPI template with factory pattern architecture.
FastAPI template - Flexible, lightweight FastAPI project generator. It includes support for SQLAlchemy, multiple databases, CI/CD, Docker, and Kubernetes.
FastAPI on Google Cloud Run - Boilerplate for API building with FastAPI, SQLModel, and Google Cloud Run.
FastAPI with Firestore - Boilerplate for API building with FastAPI and Google Cloud Firestore.
fastapi-alembic-sqlmodel-async - This is a project template which uses FastAPI, Alembic, and async SQLModel as ORM.
fastapi-starter-project - A project template which uses FastAPI, SQLModel, Alembic, Pytest, Docker, GitHub Actions CI.
Full Stack FastAPI and MongoDB - Base Project Generator - Full stack, modern web application generator, which includes FastAPI, MongoDB, Docker, Celery, React frontend, automatic HTTPS and more.
Uvicorn Poetry FastAPI Project Template - Cookiecutter project template for starting a FastAPI application. Runs in a Docker container with Uvicorn ASGI server on Kubernetes. Supports AMD64 and ARM64 CPU architectures.
Docker Images
inboard - Docker images to power your FastAPI apps and help you ship faster.
uvicorn-gunicorn-fastapi-docker - Docker image with Uvicorn managed by Gunicorn for high-performance FastAPI web applications in Python 3.7 and 3.6 with performance auto-tuning.
uvicorn-gunicorn-poetry - Docker image with Gunicorn using Uvicorn workers for running Python web applications. Uses Poetry for managing dependencies and setting up a virtual environment. Supports AMD64 and ARM64 CPU architectures.
uvicorn-poetry - Docker image with Uvicorn ASGI server for running Python web applications on Kubernetes. Uses Poetry for managing dependencies and setting up a virtual environment. Supports AMD64 and ARM64 CPU architectures.
Open Source Projects
Astrobase - Simple, fast, and secure deployments anywhere.
Awesome FastAPI Projects - Organized list of projects that use FastAPI.
Bitcart - Platform for merchants, users and developers which offers easy setup and use.
Bali - Simplify Cloud Native Microservices development base on FastAPI and gRPC.
Bunnybook - A tiny social network built with FastAPI, React+RxJs, Neo4j, PostgreSQL, and Redis.
Coronavirus-tg-api - API for tracking the global coronavirus (COVID-19, SARS-CoV-2) outbreak.
Dispatch - Manage security incidents.
FastAPI CRUD Example:
Async flavor
Sync Flavor
FastAPI with Observability - Observe FastAPI app with three pillars of observability: Traces (Tempo), Metrics (Prometheus), Logs (Loki) on Grafana through OpenTelemetry and OpenMetrics.
DogeAPI - API with high performance to create a simple blog and CRUD with OAuth2PasswordBearer.
FastAPI Websocket Broadcast - Websocket 'broadcast' demo.
FastAPI with Celery, RabbitMQ, and Redis - Minimal example utilizing FastAPI and Celery with RabbitMQ for task queue, Redis for Celery backend, and Flower for monitoring the Celery tasks.
FuturamaAPI - A REST and GraphQL playground built with best practices, providing WebSockets, SSE, callbacks, secret messages, and more.
JeffQL - Simple authentication and login API using GraphQL and JWT.
JSON-RPC Server - JSON-RPC server based on FastAPI.
Mailer - Dead-simple mailer micro-service for static websites.
Markdown-Videos - API for generating thumbnails to embed into your markdown content.
Nemo - Be productive with Nemo.
OPAL (Open Policy Administration Layer) - Real-time authorization updates on top of Open-Policy; built with FastAPI, Typer, and FastAPI WebSocket pub/sub.
OSBot-Fast-API - Type-safe FastAPI wrapper that provides middleware, HTTP event tracking, AWS Lambda integration, test utilities, and auto-conversion between Type_Safe, Pydantic, and dataclasses.
Polar - A funding and monetization platform for developers, built with FastAPI, SQLAlchemy, Alembic, and Arq.
RealWorld Example App - mongo
RealWorld Example App - postgres
redis-streams-fastapi-chat - A simple Redis Streams backed chat app using Websockets, Asyncio and FastAPI/Starlette.
Sprites as a service - Generate your personal 8-bit avatars using Cellular Automata.
Slackers - Slack webhooks API.
TermPair - View and control terminals from your browser with end-to-end encryption.
Universities - API service for obtaining information about +9600 universities worldwide.



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
