# MASTER PROMPT – AI TECH LEAD AGENT PLATFORM

You are a Senior Enterprise Software Architect, Staff Engineer, AI Agent Architect, Product Architect, UI/UX Architect, DevOps Architect, and Technical Lead.

Your task is to design and generate a complete production-ready enterprise platform named:

# AI Tech Lead Agent Platform

The platform acts as an Autonomous Resource Manager (RM) and Tech Lead (TL) assistant.

The system should automatically:

* Manage employees
* Track skills
* Assign stories/tasks
* Review completed work
* Update employee skill scores
* Recommend next stories
* Generate learning paths
* Send notifications
* Send emails
* Maintain activity history
* Provide dashboards for RM/TL and Employees
* Use AI Agents for autonomous decision-making

The platform must be modular, scalable, event-driven, API-first, and production-ready.

---

# PRIMARY BUSINESS PROBLEM

In software companies:

* Resource Managers manually assign work.
* Tech Leads manually review task allocation.
* Employees wait for new assignments.
* Skill tracking is manual.
* Learning progression is not structured.
* Story assignment is subjective.
* Managers spend too much time on operational activities.

The platform should automate the entire lifecycle.

---

# CORE AGENTIC WORKFLOW

Employee Registered

↓

Skill Profile Created

↓

RM/TL Creates Backlog

↓

AI Agent Evaluates Employees

↓

AI Agent Assigns Story

↓

Email Notification Sent

↓

Bell Notification Generated

↓

Employee Works On Story

↓

Employee Marks Story Completed

↓

AI Review Agent Reviews Submission

↓

Quality Score Generated

↓

Skill Matrix Updated

↓

Learning Path Updated

↓

Next Story Recommended

↓

New Assignment Generated

↓

Notifications Sent

↓

Repeat

---

# TECH STACK (STRICTLY FOLLOW)

Backend:

* Java 21
* Spring Boot 3.x
* Spring Security
* Spring Data JPA
* Spring Cloud

Frontend:

* ReactJS
* Lit Elements Web Components

Database:

* PostgreSQL

Event Streaming:

* Apache Kafka

AI:

* OpenAI APIs
* RAG Architecture
* MCP (Model Context Protocol)

Email:

* Java Mail Sender

Authentication:

* JWT Authentication

API:

* REST APIs

Containerization:

* Docker

Documentation:

* OpenAPI / Swagger

Build Tool:

* Maven

Do not use:

* Node Backend
* Python Backend
* MongoDB
* Redis
* ElasticSearch
* Any technology outside the approved stack

---

# ARCHITECTURE RULE

Every service must be a completely independent Spring Boot project.

Each service must:

* Have its own project folder
* Have its own database schema
* Have its own application.yml
* Have its own Dockerfile
* Have its own API layer
* Have its own Kafka consumers/producers
* Be deployable independently

No shared business logic between services.

Communication:

* REST APIs
* Kafka Events

---

# PROJECT STRUCTURE

root/

employee-service/

skill-service/

task-service/

assignment-service/

review-service/

learning-path-service/

notification-service/

agent-orchestrator-service/

analytics-service/

frontend/

documentation/

docker/

deployment/

---

# SERVICE 1

EMPLOYEE SERVICE

Responsibilities:

* Employee management
* Experience tracking
* Designation tracking
* Team mapping
* Availability tracking

Roles:

* Intern
* Fresher
* Junior Developer
* Software Engineer
* Senior Engineer
* Lead Engineer

APIs:

Create Employee

Update Employee

Delete Employee

Get Employee

Get Team Members

Get Available Employees

---

# SERVICE 2

SKILL SERVICE

Responsibilities:

Maintain employee skills.

Examples:

Java

Spring Boot

Kafka

PostgreSQL

React

Docker

Microservices

Store:

* Skill score
* Confidence score
* Last updated
* Improvement history

Generate skill matrix.

---

# SERVICE 3

TASK SERVICE

Responsibilities:

Manage stories/tasks.

Status:

Created

Assigned

In Progress

Completed

Rejected

Reviewed

Maintain:

* Complexity
* Technology
* Story Points
* Priority
* Due Date

---

# SERVICE 4

ASSIGNMENT SERVICE

Responsibilities:

Assign best story to best employee.

AI Assignment Criteria:

* Skill Match
* Experience
* Availability
* Current Workload
* Previous Quality Score
* Learning Goal

The assignment must be AI-driven.

No manual assignment logic.

---

# SERVICE 5

AI REVIEW SERVICE

Responsibilities:

Review completed work.

Inputs:

* Git Repository URL
* Pull Request
* Commit Link
* Uploaded Files

Review:

* Code Quality
* Security
* Design
* Naming Standards
* Architecture Standards
* Test Coverage

Output:

Review Score

Strengths

Weaknesses

Recommendations

Updated Skill Scores

---

# SERVICE 6

LEARNING PATH SERVICE

Responsibilities:

Generate growth roadmap.

Example:

Java Basics

↓

Spring Boot

↓

REST APIs

↓

Security

↓

Kafka

↓

Microservices

↓

Cloud

AI should automatically recommend next learning objectives.

---

# SERVICE 7

NOTIFICATION SERVICE

Responsibilities:

Generate notifications.

Channels:

Email

In-App Notification

Bell Notifications

Notification Types:

Task Assigned

Task Completed

Review Completed

Learning Recommendation

Manager Announcement

Notification Center required.

Read/Unread support required.

---

# SERVICE 8

AGENT ORCHESTRATOR SERVICE

This is the brain of the platform.

Responsibilities:

Autonomous decision making.

Agents:

Assignment Agent

Review Agent

Learning Agent

Skill Analysis Agent

Recommendation Agent

Notification Agent

Manager Insight Agent

The orchestrator must use:

OpenAI

RAG

MCP

Agent workflow execution

This service coordinates all services.

---

# SERVICE 9

ANALYTICS SERVICE

Responsibilities:

Manager reporting.

Reports:

Employee Productivity

Task Completion Rate

Skill Growth

Learning Progress

Assignment Distribution

Top Performers

Promotion Readiness

Risk Employees

Intern Progress

Fresher Progress

Team Performance

---

# RAG REQUIREMENTS

Create enterprise-grade RAG.

Knowledge Sources:

Company Guidelines

Coding Standards

Development SOPs

Architecture Documents

Learning Material

Review Guidelines

Store embeddings.

Support semantic search.

Provide context to AI agents.

---

# MCP REQUIREMENTS

Implement MCP integration layer.

Provide tools:

Employee Lookup Tool

Task Lookup Tool

Skill Lookup Tool

Assignment Tool

Review Tool

Notification Tool

Learning Tool

Analytics Tool

Agents must communicate using MCP-compatible tool interfaces.

---

# RM / TL DASHBOARD

Features:

Overview Cards

Employee Utilization

Assignments

Pending Reviews

Skill Gaps

Team Analytics

Notifications Bell

Recent Activities

AI Recommendations

AI Insights Panel

Team Performance Graphs

Employee Growth Tracking

Assignment Approvals

Learning Progress

Dark/Light Theme

Responsive Design

---

# EMPLOYEE DASHBOARD

Features:

My Tasks

My Assignments

My Reviews

My Learning Path

My Skill Matrix

My Progress

Notifications Bell

Activity Timeline

AI Suggestions

Performance Score

Achievement Tracking

Dark/Light Theme

Responsive Design

---

# SECURITY REQUIREMENTS

Implement:

JWT Authentication

Role-Based Access Control

Roles:

ADMIN

RM

TECH_LEAD

EMPLOYEE

Secure APIs.

Secure AI endpoints.

Protect sensitive employee information.

---

# EMAIL REQUIREMENTS

All email configurations must come from .env.

Examples:

MAIL_HOST

MAIL_PORT

MAIL_USERNAME

MAIL_PASSWORD

MAIL_FROM

System must work immediately after developer provides values.

---

# OPENAI REQUIREMENTS

All OpenAI settings must come from .env.

Examples:

OPENAI_API_KEY

OPENAI_MODEL

OPENAI_EMBEDDING_MODEL

OPENAI_BASE_URL

No hardcoded values.

---

# DATABASE REQUIREMENTS

All PostgreSQL values must come from .env.

Examples:

POSTGRES_HOST

POSTGRES_PORT

POSTGRES_DB

POSTGRES_USER

POSTGRES_PASSWORD

No hardcoded values.

---

# KAFKA REQUIREMENTS

All Kafka values must come from .env.

Examples:

KAFKA_BOOTSTRAP_SERVERS

KAFKA_GROUP_ID

KAFKA_TOPIC_PREFIX

No hardcoded values.

---

# ENVIRONMENT RULE

Any configuration that can vary between environments must be externalized.

Use .env only.

No secrets in code.

No hardcoded credentials.

Application must boot successfully after developer fills .env values.

---

# CODE GENERATION REQUIREMENTS

Generate:

* Complete folder structure
* Complete backend services
* Complete frontend
* Database schemas
* Entity models
* DTOs
* Controllers
* Services
* Repositories
* Kafka producers
* Kafka consumers
* OpenAI integrations
* RAG implementation
* MCP implementation
* Notification engine
* Email engine
* Dockerfiles
* Docker Compose
* Swagger documentation
* Sample data
* README
* Deployment guide

Generate enterprise-grade code with clean architecture, SOLID principles, design patterns, production readiness, scalability, maintainability, and complete documentation.

The final output should be a fully functional enterprise project that can be cloned, configured using only .env values, built, and run successfully.
