# Forge AI V2

> **AI-powered software engineering workspace for understanding and interacting with software repositories.**

Forge AI V2 is a full-stack application designed to help developers understand, analyze, search, and interact with software repositories using deterministic code analysis and AI-assisted capabilities.

The project is being built **from scratch**, with the goal of understanding the complete system rather than simply assembling libraries or copying implementations.

---

# 1. Project Vision

Modern software repositories can become difficult to understand as their size and complexity increase.

Forge AI V2 aims to provide a workspace where a developer can import a repository and progressively understand:

- Repository structure
- Files and directories
- Codebase statistics
- Dependencies
- Architecture
- Individual source files
- Relationships between components
- Documentation
- Repository-specific questions

The long-term goal is to combine **deterministic software analysis** with **AI-assisted understanding**.

---

# 2. Project Objective

The target Forge workflow is:

```text
Developer
    ↓
Import Repository
    ↓
Browse Files
    ↓
Analyze Codebase
    ↓
Understand Structure
    ↓
Understand Dependencies
    ↓
Ask Questions
    ↓
AI-Assisted Explanation
    ↓
Generate Documentation
    ↓
Understand Architecture
```

The project will be developed incrementally.

Only functionality that has been **implemented and verified** will be marked as completed.

---

# 3. Development Philosophy

Forge AI V2 is being developed using:

```text
LEARN
  ↓
UNDERSTAND
  ↓
DESIGN
  ↓
IMPLEMENT
  ↓
TEST
  ↓
EXPLAIN
  ↓
DOCUMENT
  ↓
COMMIT
  ↓
ADVANCE
```

The project will **not** follow:

```text
COPY → PASTE → MOVE ON
```

The objective is not only to produce working software.

The objective is to be able to:

- Explain the implementation
- Understand why it was designed that way
- Debug it
- Modify it
- Extend it
- Identify limitations
- Discuss security implications
- Explain design decisions in technical interviews

---

# 4. Current Project Status

**Current Phase:** Day 0 — Foundation & Project Setup

**Current Development Stage:** Initial React/Vite project created successfully.

### Status Legend

- 🟢 Implemented and verified
- 🟡 Currently learning / in progress
- 🔵 Planned
- 🔴 Not started

| Area | Status |
|---|---|
| Initial project setup | 🟢 |
| Node.js / npm setup | 🟢 |
| Vite setup | 🟢 |
| React project | 🟢 |
| HTML fundamentals | 🟡 |
| CSS fundamentals | 🔵 |
| JavaScript fundamentals | 🔵 |
| React fundamentals | 🟡 |
| Frontend UI | 🔵 |
| HTTP / REST | 🟡 |
| FastAPI | 🔴 |
| PostgreSQL | 🔴 |
| SQL | 🟡 |
| Authentication | 🔴 |
| Repository ingestion | 🔴 |
| Repository analysis | 🔴 |
| AI / LLM integration | 🔴 |
| Retrieval / RAG | 🔴 |
| Documentation generation | 🔴 |
| Architecture analysis | 🔴 |
| Testing | 🔴 |
| Security hardening | 🔴 |
| Deployment | 🔴 |

> **Important:** Planned functionality is not considered implemented functionality.

---

# 5. Current Project Structure

The project currently contains the following structure:

```text
forge-ai-v2/
│
├── node_modules/
├── public/
├── src/
│
├── .gitignore
├── .oxlintrc.json
├── index.html
├── package.json
├── package-lock.json
├── README.md
└── vite.config.js
```

Current `src/` structure:

```text
src/
│
├── assets/
├── App.jsx
├── App.css
├── index.css
└── main.jsx
```

This is the initial Vite + React structure.

The project structure will evolve as actual application requirements appear.

Folders and abstractions will not be introduced unnecessarily.

---

# 6. Current Development Environment

The current environment is:

```text
Node.js : v22.14.0
npm     : 10.9.2
```

The project was created using Vite.

Initial command:

```bash
npm create vite@latest forge-ai-v2
```

Configuration selected:

```text
Framework : React
Variant   : JavaScript
Linter    : Oxlint
Install   : Yes
```

---

# 7. Running the Current Project

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

The Vite development server provides the local development environment for the frontend.

---

# 8. Current React Application Flow

The current application begins with:

```text
index.html
    ↓
<div id="root"></div>
    ↓
src/main.jsx
    ↓
React createRoot()
    ↓
<App />
    ↓
src/App.jsx
    ↓
Browser UI
```

The purpose of `main.jsx` is to connect the React application to the HTML element where React will render the application.

---

# 9. Technology Stack

## Frontend

- React
- JavaScript
- Vite
- Tailwind CSS
- React Router

## Backend

- Python
- FastAPI
- Pydantic
- REST APIs

## Database

- PostgreSQL
- SQL
- SQLAlchemy
- Alembic

## Authentication

- Secure password hashing
- Authentication credentials/tokens as appropriate
- Authorization
- Repository ownership checks

## AI

- LLM API
- Repository-grounded context
- Retrieval/RAG when required

## Development Tools

- Git
- GitHub
- VS Code
- Browser Developer Tools
- Postman or equivalent
- pytest

> Technologies will be introduced only when they solve an actual project requirement.

---

# 10. Target Architecture

The initial target architecture is:

```text
                         USER
                           │
                           ▼
                   ┌───────────────┐
                   │    React      │
                   │   Frontend    │
                   └───────┬───────┘
                           │
                       HTTP / REST
                           │
                           ▼
                   ┌───────────────┐
                   │    FastAPI    │
                   │    Backend    │
                   └───────┬───────┘
                           │
                 ┌─────────┴─────────┐
                 ▼                   ▼
          ┌─────────────┐     ┌──────────────┐
          │ PostgreSQL  │     │  Repository  │
          │  Database   │     │  Processing  │
          └─────────────┘     └──────┬───────┘
                                      │
                                      ▼
                               ┌────────────┐
                               │ AI / LLM   │
                               └────────────┘
```

This architecture is a **target design**.

It will be updated when implementation reveals better or necessary design decisions.

---

# 11. Core Request Flow

A typical Forge request is expected to follow:

```text
Browser
   ↓
React UI
   ↓
HTTP Request
   ↓
FastAPI Endpoint
   ↓
Request Validation
   ↓
Application / Service Logic
   ↓
Database / Repository Processing / AI
   ↓
HTTP Response
   ↓
React
   ↓
User
```

The exact flow will depend on the feature.

---

# 12. Core Features

## 12.1 Authentication

Target functionality:

- User registration
- Secure password storage
- Login
- Authentication
- Authorization
- Protected frontend routes
- Protected backend APIs
- Repository ownership
- Logout
- Credential expiry/handling

**Current status:** 🔴 Not implemented

---

## 12.2 Repository Import

Initial repository ingestion will focus on ZIP uploads.

Target flow:

```text
User
  ↓
Select ZIP
  ↓
Frontend Validation
  ↓
HTTP Multipart Upload
  ↓
FastAPI
  ↓
File Validation
  ↓
Safe Extraction
  ↓
File Enumeration
  ↓
Metadata Storage
  ↓
Repository Analysis
```

Security considerations:

- File-size limits
- File-type validation
- Safe ZIP extraction
- Path-traversal protection
- Temporary-file cleanup
- Ownership validation
- Malicious file handling
- No automatic execution of uploaded code

**Current status:** 🔴 Not implemented

---

## 12.3 File Browsing

Target functionality:

```text
Repository
   ↓
Directories
   ↓
Files
   ↓
File Contents
```

The user should be able to browse a repository through the Forge interface.

**Current status:** 🔴 Not implemented

---

## 12.4 Repository Analysis

Forge will first perform deterministic analysis before using AI interpretation.

Potential metrics:

- Total files
- Directory count
- File types
- Language distribution
- File sizes
- Largest files
- Repository hierarchy
- Dependencies
- Basic code metrics

Important principle:

> **Repository facts should be computed from the actual repository rather than fabricated by an AI model.**

**Current status:** 🔴 Not implemented

---

## 12.5 AI Code Understanding

Target functionality:

- Explain a source file
- Explain a function
- Summarize code
- Explain relationships between files
- Answer repository-specific questions

Expected flow:

```text
User Question
      ↓
Relevant Repository Context
      ↓
Prompt Construction
      ↓
LLM API
      ↓
Response Validation
      ↓
Forge UI
```

**Current status:** 🔴 Not implemented

---

## 12.6 Repository-Grounded Q&A

The AI should answer questions using the actual repository as context.

Examples:

```text
"Where is authentication implemented?"

"How does the backend communicate with the database?"

"Which file handles repository uploads?"

"What happens when a user logs in?"
```

The system should distinguish between:

```text
Repository-derived facts
        vs.
AI interpretation
        vs.
AI uncertainty
```

**Current status:** 🔴 Not implemented

---

## 12.7 Documentation Generation

Target workflow:

```text
Repository
    ↓
Repository Analysis
    ↓
Relevant Files
    ↓
AI
    ↓
Documentation
    ↓
Validation
    ↓
Storage / Display
```

AI-generated documentation must not invent repository facts.

**Current status:** 🔴 Not implemented

---

## 12.8 Architecture Understanding

The architecture view should eventually be based on actual repository information.

Potential sources:

- Directory structure
- Files
- Imports
- Dependencies
- Modules
- Relationships

The underlying architecture information must be derived from real repository data.

**Current status:** 🔴 Not implemented

---

## 12.9 Search

Target functionality:

- File search
- Repository search
- Code search
- Potential semantic search later

**Current status:** 🔴 Not implemented

---

# 13. AI and RAG Strategy

AI will not be added simply for the sake of adding AI.

The initial progression will be:

```text
LLM API
   ↓
Explain File
   ↓
Summarize Repository
   ↓
Repository Q&A
   ↓
Documentation
   ↓
Architecture Understanding
```

Retrieval/RAG will be introduced when repository size makes direct context passing impractical.

Potential RAG architecture:

```text
Repository
    ↓
Chunking
    ↓
Indexing / Embeddings
    ↓
Retrieval
    ↓
Ranking
    ↓
Relevant Context
    ↓
LLM
```

The project will not introduce a vector database unless there is a genuine requirement.

---

# 14. Database Design

PostgreSQL will be used as the primary relational database.

Potential entities include:

```text
Users
Repositories
Repository Files
Analyses
Analysis Findings
Conversations
Messages
Documents
Notifications
Activities
GitHub Accounts
```

These tables will **not** be created all at once.

Each entity will be introduced when required.

For every database table, the project will document:

- Purpose
- Columns
- Primary key
- Foreign keys
- Relationships
- Constraints
- Indexes
- Ownership
- Security considerations

---

# 15. Authentication Architecture

Forge will distinguish:

### Authentication

> Who are you?

### Authorization

> What are you allowed to access?

Target flow:

```text
Registration
    ↓
Password Hashing
    ↓
Database
    ↓
Login
    ↓
Credential Verification
    ↓
Authentication Credential
    ↓
Authenticated Request
    ↓
Backend Verification
    ↓
Authorization
    ↓
Protected Resource
```

The backend must enforce authorization.

The frontend must never be treated as the authority for access control.

---

# 16. Security Principles

Security will be considered throughout development.

Areas include:

- Password hashing
- Authentication
- Authorization
- Repository ownership
- SQL injection prevention
- XSS
- CSRF where applicable
- CORS
- Secret management
- API-key protection
- Upload validation
- ZIP path traversal
- Prompt injection
- Malicious repository content
- Data leakage
- Rate limiting
- Token limits
- Private repository privacy

Uploaded repository code must not be automatically executed.

---

# 17. Testing Strategy

Testing will be introduced alongside implementation.

### Frontend

- Component behavior
- User interaction
- API integration
- Loading states
- Error states

### Backend

- API endpoints
- Validation
- Authentication
- Authorization
- Database operations
- Repository upload
- Failure handling

### Important Failure Cases

```text
Invalid login
Invalid ZIP
Oversized ZIP
Expired credential
Unauthorized repository
Missing file
AI timeout
AI failure
Database failure
Empty search
Invalid API request
```

**Current status:** 🔴 Not implemented

---

# 18. DSA Connections

Forge will naturally connect software engineering concepts with DSA.

Examples:

| Forge Problem | Possible DSA Concept |
|---|---|
| Repository hierarchy | Tree |
| Directory traversal | DFS / BFS |
| Dependencies | Graph |
| Circular dependencies | Cycle detection |
| File lookup | Hash table |
| Search/indexing | Search structures |
| Processing tasks | Queue |
| Sorting metrics | Sorting algorithms |
| Caching/lookup | Hashing |

These concepts will be learned separately when necessary and then connected back to the actual project.

---

# 19. Networking Connections

Forge will also be used to understand practical networking.

Topics include:

- Client-server architecture
- HTTP
- HTTPS
- DNS
- TCP
- TLS
- REST
- JSON
- CORS
- HTTP status codes
- Latency
- Timeouts
- Retries
- Rate limiting
- WebSockets if streaming is required

Example:

```text
Browser
   ↓
HTTP Request
   ↓
FastAPI
   ↓
Processing
   ↓
HTTP Response
   ↓
Browser
```

---

# 20. Operating System Connections

The project will also connect application development with OS concepts.

Relevant areas include:

- Processes
- Threads
- Files
- File systems
- Memory
- CPU usage
- Concurrency
- Asynchronous I/O
- Resource limits
- Temporary files
- Cleanup
- Background processing

For example, if repository analysis becomes expensive, we need to understand why performing it directly inside a normal HTTP request may become problematic.

---

# 21. Ten-Day MVP Roadmap

The current target is to build a **working Forge AI V2 MVP in approximately 10 days**.

This is an aggressive implementation target.

It does **not** mean mastering every advanced technology in ten days.

### Day 0 — Foundation

- Project setup
- Understand project structure
- Understand Vite
- Understand React entry point
- Establish README
- Establish Git workflow
- Establish development process

**Status:** 🟡 In progress

---

### Day 1 — Web + React Foundations

Learn and apply:

- HTML
- CSS
- JavaScript fundamentals
- JSX
- React components
- Props
- State
- Events
- Basic UI structure

Build the first Forge UI.

**Status:** 🔵 Planned

---

### Day 2 — React Frontend

Learn and implement:

- React state
- Forms
- Controlled inputs
- Lists
- Conditional rendering
- Hooks
- Routing
- API service structure
- Loading states
- Error states

Create the initial Forge application interface.

**Status:** 🔵 Planned

---

### Day 3 — HTTP + FastAPI

Learn:

- HTTP
- Requests
- Responses
- Methods
- Status codes
- REST
- JSON
- API endpoints
- FastAPI
- Pydantic
- Validation

Create the initial backend.

**Status:** 🔵 Planned

---

### Day 4 — PostgreSQL + SQL

Learn:

- Database fundamentals
- Tables
- Rows
- Columns
- Primary keys
- Foreign keys
- Relationships
- SQL
- JOINs
- Constraints
- Indexes
- Transactions
- Basic schema design

Connect FastAPI to PostgreSQL.

**Status:** 🔵 Planned

---

### Day 5 — Authentication

Implement:

- Registration
- Password hashing
- Login
- Authentication
- Authorization
- Protected APIs
- Protected frontend routes
- Repository ownership model

**Status:** 🔵 Planned

---

### Day 6 — Repository Ingestion

Implement:

- ZIP upload
- Multipart requests
- File validation
- Safe extraction
- Path-traversal protection
- File enumeration
- Repository metadata
- File browsing

**Status:** 🔵 Planned

---

### Day 7 — Repository Analysis

Implement deterministic analysis:

- File count
- Directory count
- File types
- Language distribution
- File sizes
- Repository hierarchy
- Basic dependency information
- Search foundation

Connect analysis results to the frontend.

**Status:** 🔵 Planned

---

### Day 8 — AI Integration

Implement:

- LLM API integration
- File explanation
- Repository context
- Repository Q&A
- Error handling
- AI response validation

**Status:** 🔵 Planned

---

### Day 9 — Documentation + Architecture

Implement the first versions of:

- Documentation generation
- Repository search
- Architecture information
- Dependency understanding
- Improved repository Q&A

**Status:** 🔵 Planned

---

### Day 10 — Integration + Verification

Focus on:

- End-to-end integration
- Testing
- Security review
- Error handling
- README completion
- Code cleanup
- Git history
- Deployment preparation
- Interview preparation

**Status:** 🔵 Planned

---

# 22. What Will NOT Be Forced Into the 10-Day MVP

The following will only be introduced if the project genuinely requires them:

- Microservices
- Redis
- Kafka
- Kubernetes
- Complex distributed systems
- Vector databases
- Background job infrastructure
- Advanced caching
- GitHub OAuth
- Large-scale cloud architecture
- Complex observability systems

The principle is:

> **Do not add infrastructure just because it appears impressive on a resume.**

---

# 23. Interview Preparation

Forge AI V2 is also being developed as an interview-preparation project.

Interview preparation will be based on the **actual implementation**.

Expected categories include:

### Project

- Why did you build Forge?
- What problem does it solve?
- Explain the architecture.
- Explain a complete request.
- What was the hardest part?
- What would you improve?

### Frontend

- React
- JavaScript
- JSX
- State
- Props
- Hooks
- Rendering
- Routing

### Backend

- FastAPI
- REST
- Request validation
- Error handling
- Service architecture
- API design

### Database

- SQL
- PostgreSQL
- JOINs
- Indexes
- Transactions
- ACID
- Query optimization
- Schema design

### Security

- Authentication
- Authorization
- Password hashing
- JWT/session concepts
- SQL injection
- XSS
- CSRF
- Upload security
- Prompt injection

### AI

- LLMs
- Tokens
- Context windows
- Hallucinations
- Prompt design
- Retrieval
- RAG
- Embeddings
- AI security

### System Design

- Scalability
- Caching
- Queues
- Background processing
- Database scaling
- Rate limiting
- Reliability
- Observability

The objective is to progress from:

```text
Basic
  ↓
Intermediate
  ↓
Advanced
  ↓
System Design
```

rather than memorizing advanced terminology before understanding the fundamentals.

---

# 24. Git Workflow

Each meaningful feature should follow:

```text
Implement
   ↓
Test
   ↓
Check git diff
   ↓
Update README
   ↓
Commit
   ↓
Push
```

Example commit:

```bash
git add .
git commit -m "feat: add repository upload validation"
git push
```

Commits should represent meaningful development progress.

Fake or misleading commits will not be used.

---

# 25. README Maintenance Policy

This README is a **living document**.

It will be updated throughout development.

Whenever a meaningful feature is completed:

1. Verify the feature.
2. Update the relevant project status.
3. Update architecture if necessary.
4. Update project structure if necessary.
5. Document important implementation decisions.
6. Document security considerations.
7. Document testing performed.
8. Record the development milestone.
9. Commit the changes.
10. Push to GitHub.

### Status must remain truthful.

For example:

```text
❌ "AI-powered repository analysis implemented"
```

when only an API call exists.

Instead:

```text
🟡 LLM integration in progress
```

until the actual feature has been implemented and verified.

---

# 26. Development Log

## Day 0 — Foundation & Setup

### Completed

- [x] Created Forge AI V2 project
- [x] Created React + Vite frontend
- [x] Selected JavaScript variant
- [x] Configured Oxlint
- [x] Installed project dependencies
- [x] Verified Node.js
- [x] Verified npm
- [x] Started local development environment
- [x] Reviewed initial project structure
- [x] Understood the role of `main.jsx`
- [x] Defined Forge AI V2 architecture
- [x] Defined development methodology
- [x] Created living README structure

### Currently Learning

- [ ] HTML fundamentals
- [ ] CSS fundamentals
- [ ] JavaScript fundamentals
- [ ] React fundamentals
- [ ] Vite fundamentals
- [ ] Git workflow

### Not Yet Implemented

- [ ] Forge UI
- [ ] Backend
- [ ] PostgreSQL
- [ ] Authentication
- [ ] Repository upload
- [ ] File browsing
- [ ] Repository analysis
- [ ] Search
- [ ] AI integration
- [ ] Repository Q&A
- [ ] Documentation generation
- [ ] Architecture analysis
- [ ] Testing
- [ ] Deployment

---

# 27. Learning Status

## Web Development

| Topic | Status |
|---|---|
| HTML | 🟡 Starting |
| CSS | 🔴 Not learned |
| JavaScript | 🔴 Not learned |
| DOM | 🔴 Not learned |

## React

| Topic | Status |
|---|---|
| React purpose | 🟡 Basic |
| Components | 🔴 Not learned |
| JSX | 🟡 Basic |
| Props | 🔴 Not learned |
| State | 🔴 Not learned |
| Events | 🔴 Not learned |
| Hooks | 🔴 Not learned |
| Routing | 🔴 Not learned |

## Backend

| Topic | Status |
|---|---|
| HTTP | 🟡 Basic |
| REST | 🟡 Basic |
| FastAPI | 🔴 Not learned |
| PostgreSQL | 🔴 Not learned |
| SQL | 🟡 Basic |
| Authentication | 🔴 Not learned |

## Engineering

| Topic | Status |
|---|---|
| Git | 🟡 Basic |
| Testing | 🔴 Not learned |
| Security | 🔴 Not learned |
| System Design | 🔴 Not learned |
| AI / LLM | 🔴 Not learned in implementation |
| RAG | 🔴 Not learned |

---

# 28. Definition of MVP Completion

The Forge AI V2 MVP will be considered complete only when the following are actually implemented and verified:

- [ ] Frontend
- [ ] Backend
- [ ] PostgreSQL
- [ ] Authentication
- [ ] Authorization
- [ ] Repository ingestion
- [ ] Safe repository processing
- [ ] Real file browsing
- [ ] Deterministic repository analysis
- [ ] Repository search
- [ ] AI file explanation
- [ ] Repository-grounded Q&A
- [ ] Documentation capability
- [ ] Architecture information
- [ ] Loading states
- [ ] Error states
- [ ] Basic testing
- [ ] Security controls
- [ ] Documentation
- [ ] Git history
- [ ] Deployment preparation

---

# 29. Personal Success Criteria

The project is not considered successful merely because the application runs.

By the end of the project, the developer should be able to explain:

- How React renders the application
- How components communicate
- How state works
- How routing works
- How HTTP requests work
- How React communicates with FastAPI
- How FastAPI handles requests
- How validation works
- How PostgreSQL stores the data
- How SQL queries retrieve data
- How authentication works
- How authorization works
- How repositories are uploaded
- How files are safely processed
- How repository metrics are calculated
- How AI receives repository context
- How repository-grounded Q&A works
- How failures are handled
- How security risks are mitigated
- How the system could scale
- Why each major architectural decision was made

---

# 30. Long-Term Roadmap

After the initial MVP, potential future development includes:

```text
MVP
 ↓
Improved Repository Analysis
 ↓
Advanced Retrieval / RAG
 ↓
GitHub Integration
 ↓
Private Repository Support
 ↓
Advanced Architecture Visualization
 ↓
Intelligent Engineering Recommendations
 ↓
Scalability Improvements
 ↓
Production Deployment
```

These features are future possibilities and are not currently implemented.

---

# 31. Core Principle

> **Build it. Understand it. Break it. Fix it. Explain it.**

Forge AI V2 is not just a project to put on a resume.

It is a practical environment for learning:

```text
Web Development
        +
Software Engineering
        +
Backend Development
        +
Databases
        +
Networking
        +
Operating Systems
        +
DSA
        +
AI
        +
Security
        +
System Design
```

The final goal is to build a real system while becoming capable of defending every major technical decision behind it.

---

# 32. Current Next Step

**Day 0 — Next Task:**

```text
HTML Fundamentals
        ↓
CSS Fundamentals
        ↓
JavaScript Fundamentals
        ↓
React Fundamentals
        ↓
First Forge UI
```

No major feature will be built before the required concepts are understood.

**Current objective: Learn the foundation, then build Forge from it.**