# Hi, I'm Saurabh Chauhan 👋

### Senior Full Stack Engineer • AI Engineer • Founder @ Trackye

I build production AI-powered SaaS products, developer infrastructure, and scalable backend systems.

Currently building **Trackye** — an AI Memory platform that helps marketing agencies capture organizational knowledge, automate workflows, and generate business insights using AI.

## 🚀 About Me

I'm a **Senior Full Stack Engineer** with **5+ years** of experience designing and shipping production software.

My experience spans AI applications, multi-tenant SaaS, cloud infrastructure, backend architecture, and developer tooling. I enjoy solving complex engineering problems that require thoughtful system design, scalable architectures, and clean abstractions.

Previously I worked at **Travelopia**, building reservation and analytics platforms serving global travel brands, where I helped modernize legacy systems, built scalable backend services, and developed applications processing **1.2M+ records** and **40K+ bookings**.

Today I'm focused on building AI-native software that combines Large Language Models with production engineering.


# 🧠 Currently Building

## Trackye — AI Memory for Agencies

Trackye is an AI-powered SaaS that captures conversations, voice notes, tasks, meetings, documents, and marketing platform data, then transforms them into organizational memory, automated quotes & reports, AI-powered workflows, and actionable business insights.

### Highlights

* 🤖 AI Agents
* 🧠 LLM Integrations (OpenAI, Claude, Gemini)
* 📚 Retrieval-Augmented Generation (RAG)
* 🔗 MCP-compatible AI Tools
* ⚡ Workflow Automation
* 🏢 Multi-tenant SaaS Architecture
* 📈 Marketing Platform Integrations
* 💬 WhatsApp Business API
* 📊 Meta Ads, Facebook, Instagram, Google Analytics, Search console, Youtube analytics & Google Business Profile Integrations

**Website:** https://trackye.com

# ⚙️ Engineering Philosophy

I enjoy building software that is:

* Simple to extend
* Easy to maintain
* Secure by default
* Production ready
* AI-native
* Built with long-term scalability in mind

Most of my work revolves around:

* AI Applications
* Backend Architecture
* Distributed Systems
* Developer Experience
* Cloud Infrastructure
* Multi-tenant SaaS
* Performance & Reliability

# 💻 Technical Expertise

## Languages

* TypeScript
* JavaScript
* SQL

## Frontend

* Next.js
* React
* Tailwind CSS
* Server Actions

## Backend

* Node.js
* NestJS
* REST APIs
* PostgreSQL
* Prisma
* Supabase
* Redis

## AI Engineering

* AI Agents
* LLM Integrations
* Retrieval-Augmented Generation (RAG)
* Model Context Protocol (MCP)
* Prompt Engineering
* Function Calling
* Structured Outputs
* Semantic Search
* Vector Search
* AI Workflow Automation

## Cloud & DevOps

* AWS
* GitHub Actions
* CI/CD
* Vercel

---

# 📈 Professional Highlights

* ✅ 5+ years of Full Stack Engineering experience
* ✅ Founder of an AI SaaS startup
* ✅ Built production multi-tenant SaaS platforms
* ✅ Designed AI-powered applications using LLMs
* ✅ Experience building AI Agents, RAG pipelines, and workflow automation
* ✅ Architected scalable backend systems
* ✅ Built cloud-native applications on AWS
* ✅ Developed analytics platforms serving **40K+ bookings**
* ✅ Designed systems processing **1.2M+ records**
* ✅ End-to-end ownership from architecture to production deployment

# 🏗️ Engineering Patterns & Architecture Notes

Most of these patterns were extracted from production systems while building multi-tenant SaaS applications and AI-powered platforms. Rather than framework tutorials, they document reusable architectural decisions that improve scalability, maintainability, security, developer experience, and cloud-native architectures.

---

## 🛡️ Security & Backend Infrastructure

### 🚦 Generic Distributed Rate Limiter with Local Fallback

A production-ready distributed sliding-window rate limiter using **Upstash Redis** with an automatic in-memory fallback for local development. Designed to prevent abuse while maintaining an excellent developer experience.

**Highlights**

- Distributed sliding-window algorithm
- Composite IP + Identity rate limiting
- Upstash Redis integration
- Automatic local development fallback
- Cost amplification protection
- Production-safe architecture

**Topics**

`Redis` • `Distributed Systems` • `Security` • `Rate Limiting`

🔗 https://gist.github.com/symbiote-ux/6a5a18db53bc667ab6faaffb3cce0838

---

### ⚡ Type-safe Next.js Server Action Middleware

A reusable middleware layer for **Next.js Server Actions** that centralizes authentication, validation, structured logging, dependency injection, and error handling.

**Highlights**

- Authentication middleware
- Zod validation
- Structured logging
- Safe error boundaries
- Type-safe actions
- Dependency injection

**Topics**

`Next.js` • `TypeScript` • `Security` • `Developer Experience`

🔗 https://gist.github.com/symbiote-ux/493d26aff99c1f3a91dfe5064893bb9c

---

### 🔒 Preventing IDOR in Next.js Server Actions

An architectural pattern demonstrating how to eliminate **Insecure Direct Object Reference (IDOR)** vulnerabilities using reusable middleware for authentication, authorization, validation, and safe error handling.

**Highlights**

- IDOR prevention
- Authentication pipeline
- Authorization middleware
- Validation-first architecture
- Discriminated union responses
- Secure-by-default server mutations

**Topics**

`Application Security` • `Next.js` • `Backend Design`

🔗 https://gist.github.com/symbiote-ux/0be5585f3ecfd314a385b41adaa74138

---

## ☁️ Cloud Infrastructure

### ☁️ Robust S3 / Cloudflare R2 Storage Provider

A production-grade abstraction over the AWS SDK v3 for **S3-compatible storage**, supporting Cloudflare R2 with presigned uploads, streaming, intelligent caching, and secure downloads.

**Highlights**

- Presigned uploads
- Cloudflare R2 support
- AWS SDK v3 abstraction
- Partial object streaming
- Intelligent cache policies
- Storage provider interface

**Topics**

`AWS` • `Cloudflare R2` • `Object Storage` • `Cloud Architecture`

🔗 https://gist.github.com/symbiote-ux/920f0ebccb7f1e854a040d5c114478a8

---

### 📦 Direct-to-Cloud Upload Architecture (ADR)

An Architecture Decision Record (ADR) explaining the migration from traditional multipart uploads to **direct browser-to-cloud uploads** using S3 Presigned URLs and Cloudflare R2.

**Highlights**

- Direct browser uploads
- Serverless optimization
- Zero-memory uploads
- Upload finalization workflow
- Lifecycle cleanup strategy
- Bandwidth cost optimization

**Topics**

`Architecture Decision Records` • `Cloud Storage` • `Serverless` • `Performance`

🔗 https://gist.github.com/symbiote-ux/45cc7fd169670050047b9d494932c27d

---

## 🏛️ Backend Architecture

### 📂 Polymorphic Upload Finalization Engine

A Strategy Pattern implementation for scalable upload processing that routes different upload types to dedicated handlers while keeping business logic modular and extensible.

**Highlights**

- Strategy Pattern
- Intent-based routing
- Zod validation
- Async resource cleanup
- Open/Closed Principle
- Extensible architecture

**Topics**

`Design Patterns` • `SOLID` • `Backend Architecture`

🔗 https://gist.github.com/symbiote-ux/8b03fe521200e8842dcafa80a927ebd0

---

### 🔌 Generic OAuth Connector Plugin Architecture

A scalable Registry Pattern for managing OAuth integrations such as Google, Meta, Slack, and other third-party providers through reusable connector plugins.

**Highlights**

- Registry Pattern
- Plugin architecture
- OAuth abstraction
- Token encryption
- Connector lifecycle management
- Scalable third-party integrations

**Topics**

`Design Patterns` • `OAuth` • `Backend Architecture` • `Extensibility`

🔗 https://gist.github.com/symbiote-ux/f379868de5281b0fe2d105f7ae25b0e4

---

## 🚀 Developer Experience

### ⚡ next-secure-action

A production-ready framework for building secure, type-safe **Next.js Server Actions** with minimal boilerplate. It combines authentication, validation, structured outputs, logging, and multi-tenant support into a reusable middleware abstraction.

**Highlights**

- Generic authentication providers
- Type-safe middleware
- Structured outputs
- Multi-tenant support
- Validation-first execution
- Production-safe error handling

**Topics**

`Developer Experience` • `Next.js` • `TypeScript` • `Security`

🔗 https://gist.github.com/symbiote-ux/25c60a3d3bcbc703f682897a5a36655d

# 🌐 Connect

* 🌍 Website: https://trackye.com
* 💼 LinkedIn: https://linkedin.com/in/chauhansaurabh14
* 🌐 Portfolio: https://founder.trackye.com
* 📧 Email: [founder@trackye.com](mailto:founder@trackye.com)
* 📧 Personal Email: [saurabh.chauhan.dev.js@gmail.com](mailto:saurabh.chauhan.dev.js@gmail.com)

---

> **Building AI-native software that transforms business knowledge into intelligent systems.**
