# ⚡ AI Factory CI/CD: Worker AI ➔ GitHub ➔ AWS Production Cloud

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-brightgreen)](https://cosmosanalytics.github.io/AWS/)
[![AWS Production Cloud](https://img.shields.io/badge/AWS-Production%20Cloud-orange)](https://aws.amazon.com/)
[![Amazon Bedrock](https://img.shields.io/badge/Amazon%20Bedrock-Claude%203.5%20Sonnet-blueviolet)](https://aws.amazon.com/bedrock/)
[![AWS Step Functions](https://img.shields.io/badge/AWS%20Step%20Functions-State%20Machine-pink)](https://aws.amazon.com/step-functions/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

An interactive, browser-native 3-tier fractal studio modeling an autonomous CI/CD delivery pipeline from **Worker AI Cognition** to **GitHub Actions DevSecOps (S&OP)** to **AWS Production Cloud (Company)** with the complete 20-page **Human Intervention UI (HUI)**.

👉 **Live Interactive Canvas**: [https://cosmosanalytics.github.io/AWS/](https://cosmosanalytics.github.io/AWS/)

---

## 🏛️ 3-Tier Architecture Mapping

```mermaid
flowchart TD
  subgraph L3["☁️ Level 3: AWS Production Cloud (Company Equivalent)"]
    subgraph Row1["1. Production Ingress & Compute"]
      aws_edge["Route 53 DNS & CloudFront CDN"] --> aws_alb["Application Load Balancer (ALB)"]
      aws_alb --> aws_ecs["Amazon ECS Fargate Cluster"]
    end

    subgraph Row2["2. AI Foundation & Serverless Tools"]
      aws_alb -->|Agent Invocation| aws_sf["AWS Step Functions<br/>(State Machine Orchestrator)"]
      aws_sf -->|Prompt & Inference| aws_bedrock["Amazon Bedrock (FM)<br/>(Claude 3.5 Sonnet / Guardrails)"]
      aws_bedrock -->|Tool Execution| aws_lambda["AWS Lambda Tool Runners<br/>(Serverless Workers)"]
    end

    subgraph Row3["3. Observability, Vector RAG & Persistent Storage"]
      aws_bedrock -->|Semantic Search| aws_opensearch["OpenSearch Serverless<br/>(Vector RAG Database)"]
      aws_lambda -->|Transactions & State| aws_aurora["Aurora PostgreSQL & S3 Data Lake"]
      aws_ecs -->|Metrics & Alarms| aws_obs["CloudWatch & EventBridge"]
      aws_sf -->|Execution Traces| aws_obs
    end
  end

  subgraph L2["🐙 Level 2: GitHub CI/CD Pipeline (S&OP Equivalent)"]
    gh_pr["Pull Request #42 Gate"] --> gh_review["AI Code Review Agent"]
    gh_review --> gh_sec["CodeQL & Trivy Security Scan"]
    gh_sec --> gh_ci["Automated CI Test Matrix (48/48)"]
    gh_ci --> gh_gate{{"🛡️ Production Human Gate (Gate Node)"}}
    gh_gate --> gh_cd["AWS ECS & Bedrock Deploy (Canary)"]
  end

  subgraph L1["🧠 Level 1: Worker AI Dev Mind (Worker Equivalent)"]
    w_arch["Software Architect Agent"] --> w_coder["Implementation Agent (Groq LPU)"]
    w_coder --> w_tester["Test Engineer Agent (Pyodide)"]
    w_tester --> w_sec["Security & IAM Guard"]
    w_tester --> w_git["Git of Minds Synthesizer"]
  end

  L1 -->|PR Opening & Spec Commit| L2
  gh_cd -->|Approved Release & Container Image| L3
```

---

## 🎛️ Key Features & Human Intervention UI (HUI)

1. **3 Canonical Tiers**:
   - **Level 3: AWS Production Cloud**: Unified container compute (ECS Fargate, ALB, Route 53) and Generative AI Foundation stack (Bedrock, Step Functions, Lambda, OpenSearch Vector RAG, Aurora, S3, CloudWatch).
   - **Level 2: GitHub CI/CD & DevSecOps**: PR creation, AI code review, static analysis, Pyodide 48/48 unit tests, container builds, and **Human Gate**.
   - **Level 1: Worker AI Dev Mind**: Internal Society of Mind dialectical personas (Architect, Coder, Tester, Security Guard, Git Synthesizer).

2. **Human-in-the-Loop Governance**:
   - **Run Modes**: Instant switching between `Auto`, `Supervised` (halts at Human Gate), and `Step` (deterministic tick inspection).
   - **Live System State Badge**: `Waiting for you (1)`, `Running`, `Paused`, `EMERGENCY STOPPED`.
   - **Approvals Inbox with Multi-Tier Decision Cards**: Plain-English headline, why rationale, 4-cell impact grid (`$/latency/SLA/risk`), live Groq LPU rationale, and one-click `Approve & Deploy`, `Reject` (with chips), and `Batch Low-Risk`.
   - **Autonomy Policy Matrix**: Stage-by-stage `A / N / C / H` inline pill controls with hard cloud budget guardrails.
   - **Reversible Undo Ledger**: Time-windowed (30s) rollback with one-click instant state reversion.
   - **In-Browser AWS AI & Production Simulator**: Real-time ECS Fargate tasks, Blue/Green Canary traffic slider, Bedrock Foundation Model selector & Temperature Dial, Step Functions execution tracker, and live CloudWatch logs.

---

## 🚀 Quick Start

Open `index.html` in any modern web browser or visit the live deployment at [https://cosmosanalytics.github.io/AWS/](https://cosmosanalytics.github.io/AWS/).
Zero server setup or dependencies required.
