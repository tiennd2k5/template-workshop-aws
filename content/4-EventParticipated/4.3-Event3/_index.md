---
title: "Event 3: FCAJ x Agentic AI Build Week"
date: 2026-07-30
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# Event 3: AWS FCAJ Agent Forge - Deepdive

- **Event Name:** AWS FCAJ Agent Forge - Deepdive
- **Date & Time:** August 1, 2026
- **Role:** Attendee
- **Event Photo & Slide Drive:** [Google Drive Folder](https://drive.google.com/drive/folders/1YAY4dXyeaCeSQIU3Hhz6TrnyQM_x0ShV?usp=sharing)

---

## Agenda & Key Presentation Topics

During the first day of the workshop, the session focused on the concepts behind **production-ready Agentic AI systems** rather than only building simple AI demos.

The main topics covered included:

- Introduction to **Agentic AI** and the differences between AI assistants, deterministic agents, autonomous agents, and multi-agent systems.
- Understanding the role of **Model Context Protocol (MCP)** and **Agent-to-Agent (A2A)** communication for connecting AI agents with external tools and services.
- Overview of **Strands Agents SDK** and **Kiro IDE**, demonstrating how AI-assisted development can accelerate the process of building production-ready applications.
- Introduction to **Amazon Bedrock AgentCore**, AWS's platform for deploying, managing, and operating AI agents in production environments.
- Deep dive into the three core AgentCore services:
  - **AgentCore Runtime**
  - **AgentCore Identity**
  - **AgentCore Gateway**

---

## Key Learning Outcomes

### 1. Agentic AI is more than an LLM chatbot

The presentation explained that an Agentic AI system is composed of multiple components, including:

- Foundation models
- Memory
- Knowledge bases
- External tools
- Planning and reasoning
- Guardrails and observations

Unlike a traditional chatbot, an AI agent is capable of planning tasks, interacting with tools, and executing multiple actions autonomously to achieve a goal. :contentReference[oaicite:0]{index=0}

---

### 2. Production AI requires more than prompt engineering

One of the main messages of the session was that creating an AI demo is relatively easy, while deploying an AI agent into production introduces many additional challenges such as:

- Security
- Identity management
- Tool connectivity
- Memory
- Observability
- Evaluation
- Governance

Amazon Bedrock AgentCore is designed to address these production concerns by providing managed services for agent deployment and operation. :contentReference[oaicite:1]{index=1}

---

### 3. Amazon Bedrock AgentCore Runtime

The Runtime service provides a secure, serverless execution environment for AI agents.

Important capabilities include:

- Deploying agents built with different frameworks.
- Automatic scaling without infrastructure management.
- Long-running agent sessions.
- Session isolation using dedicated microVMs.
- Integration with other AgentCore services such as Memory, Identity, Browser, Gateway, and Observability. :contentReference[oaicite:2]{index=2} :contentReference[oaicite:3]{index=3}

---

### 4. AgentCore Identity

The Identity component manages authentication and authorization for AI agents.

The presentation explained the distinction between:

- **Inbound authentication**, which verifies whether a user is allowed to invoke an agent.
- **Outbound authentication**, which enables the agent to securely access external APIs and services on behalf of the user.

The concept of the **Workload Access Token (WAT)** was introduced, allowing an agent to securely carry both its own identity and the user's identity when invoking downstream resources. :contentReference[oaicite:4]{index=4}

---

### 5. AgentCore Gateway

As AI agents interact with many APIs and MCP servers, managing these integrations individually becomes difficult.

AgentCore Gateway provides:

- A unified entry point for tools and APIs.
- MCP-compatible tool integration.
- Fine-grained authorization.
- Request and response transformation.
- Monitoring and governance for tool access.

This architecture simplifies communication between agents and enterprise services while improving security and maintainability. :contentReference[oaicite:5]{index=5}

---



