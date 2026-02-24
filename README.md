# 🤖 AISEC — AI Security Governance Foundation

![AI Governance](https://img.shields.io/badge/AI-Governance-blue)
![Risk Architecture](https://img.shields.io/badge/Focus-Risk%20Architecture-red)
![Regulatory Alignment](https://img.shields.io/badge/Regulatory-EU%20AI%20Act%20Aware-green)
![Original Research](https://img.shields.io/badge/Status-Original%20Research-purple)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow)

---

## 📌 Overview

## Context

This repository contains independent technical explorations inspired by
my work in Information Security, focusing on securing AI/ML systems
deployed in production environments.

All implementations and analyses are personal learning and research
efforts and do not contain proprietary company information.

It bridges:

- AI system risk classification  
- Regulatory alignment (EU AI Act context, GDPR considerations)  
- Enterprise risk management (ERM) integration  
- Change and incident governance  
- Blue team AI security operations
- MITTRE ATLAS & OWASP LLM TOP 10 based Threat Analysis.
- Architectural undersanding of GenAI and MLops  

AISEC is intentionally designed as a living governance foundation.

---

## 📌 Research Context
This repository showcases **AISEC**, an original governance framework developed to address the critical security gap in AI/ML deployments. Focuses on "technology with impact," this project aligns technical threat modeling with real-world regulatory compliance, specifically the **EU AI Act**.

---

## 🏛️ Project Overview
The AISEC framework provides a multi-layered approach to AI security, moving from strategic policy to granular technical controls.

1.  **Strategic Governance**: High-level orchestration of AI policy and issue management.
2.  **Architectural Threat Modeling**: Deep-dive analysis of MLOps and GenAI/LLM pipelines.
3.  **Operational Risk Assessment**: Data-driven classification of third-party AI/ML tools.

---

## 🧠 1. Strategic Governance Mind Map
The **AISEC Mind Map** serves as the central orchestration layer, visualizing five critical pillars required to secure an enterprise AI environment.

<img width="749" height="287" alt="image" src="https://github.com/user-attachments/assets/af361e98-308b-464b-99c0-f326aeffafb9" />

### **Core Governance Pillars**
*   **Risk Management**: Focuses on **Insider Threat Mitigation** and **AI Supply Chain Security**.
*   **Blue Team Operations**: Active defense mechanisms and real-time adversarial detection.
*   **Governance Frameworks**: Policy baselines ensuring alignment with global standards (e.g., NIST AI RMF).
*   **Issue & Change Management**: Protocols for model drift, retraining, and incident response.

---

## 🏗️ 2. Architectural Threat Models
The following technical lifecycles are built using **Mermaid.js** for high-performance rendering. These diagrams visualize the intersection of technical threats and security controls.

### **A. MLOps Security Lifecycle**
Focuses on the classical machine learning pipeline, emphasizing data poisoning and model integrity.
> *View the `docs/mlops-security-analysis.md` file for the live-rendered Mermaid diagram.*

### **B. GenAI & LLM Security (Advanced RAG)**
A complex mapping of the **OWASP Top 10 for LLMs** onto a Retrieval-Augmented Generation architecture.
> *Includes specific mitigations for Prompt Injection (LLM01) and Excessive Agency (LLM06).*

---

## 📊 3. Interactive AI/ML Tool Risk Matrix
This module is a **functional, interactive dashboard** designed to quantify the risk of third-party AI tools.

<img width="653" height="369" alt="image" src="https://github.com/user-attachments/assets/e5eacc1d-36d5-454f-99fd-e6de703f7c9c" />

### **Interactive Navigation Instructions**
Unlike the static diagrams above, this matrix is fully interactive within the AISEC environment:
*   **Risk Wheel Exploration**: Click on any **Colored Dot** or **Quadrant** (T1-T3) on the "Risk Assessment Wheel" to filter tools by their criticality.
*   **Tool Deep-Dive**: Select the **"Tool Details"** buttons or specific tool labels (e.g., *Customer Data AI*) to view real-time scores for **Business Impact** and **Data Sensitivity**.
*   **Assessment Framework**: The matrix maps tools along the Y-axis (Strategic Impact) and X-axis (Data Sensitivity).

---

## 📂 Technical Stack
*   **Diagramming**: Mermaid.js for version-controlled architectural modeling.
*   **Visualization**: Custom interactive dashboards for risk classification.
*   **Documentation**: Markdown-based threat analysis and mitigation strategies.


---
© 2024 Ananya Kasiraj | AISEC Framework


