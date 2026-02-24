1️⃣ Lifecycle-Based Threat Analysis
🔹 Data Collection & Preprocessing
| Threat                           | Description                                        | Root Cause                           | Affected Components         | Mitigation                                                      | Impact   | Likelihood |
| -------------------------------- | -------------------------------------------------- | ------------------------------------ | --------------------------- | --------------------------------------------------------------- | -------- | ---------- |
| Data Poisoning (RAG Poisoning)   | Malicious data injected into training or RAG index | Unverified data sources              | Training data, RAG pipeline | Validate sources, isolate ingestion pipeline, monitor anomalies | High     | Medium     |
| Data Bias                        | Biased datasets produce discriminatory outputs     | Lack of fairness constraints         | Training dataset            | Diverse datasets, fairness testing                              | Medium   | High       |
| Sensitive Information Disclosure | AI exposes confidential or proprietary data        | Weak encryption, poor access control | Logs, outputs, UI           | Anonymization, encryption, privacy layers                       | Critical | Medium     |
| Weak Cryptographic Protections   | No encryption at rest/in transit                   | Poor key management                  | Model files, storage        | Strong encryption standards, secure key management              | High     | Medium     |

🔹 Training Phase
| Threat                  | Description                                                    | Root Cause                   | Affected Components | Mitigation                                        | Impact | Likelihood |
| ----------------------- | -------------------------------------------------------------- | ---------------------------- | ------------------- | ------------------------------------------------- | ------ | ---------- |
| Model Poisoning         | Hidden backdoors or biased behavior introduced during training | Unverified training data     | Training pipeline   | Secure training environment, integrity validation | High   | Medium     |
| Supply Chain Attack     | Compromised pre-trained models or libraries                    | Third-party dependency risks | CI/CD, containers   | Hash verification, secure CI/CD, SAST/DAST        | High   | Medium     |
| Backdoor Introduction   | Malicious trigger behavior embedded                            | No adversarial testing       | Model weights       | Red teaming, adversarial evaluation               | High   | Medium     |
| Insecure Configurations | Over-permissive APIs                                           | Default insecure settings    | Deployment infra    | Harden defaults, RBAC, MFA                        | High   | Medium     |

🔹 Deployment & Inference
| Threat           | Description                                 | Root Cause                    | Affected Components  | Mitigation                               | Impact   | Likelihood |
| ---------------- | ------------------------------------------- | ----------------------------- | -------------------- | ---------------------------------------- | -------- | ---------- |
| Prompt Injection | Malicious inputs manipulate model behavior  | Lack of input validation      | Chat interface, APIs | Structured prompting, input filtering    | Medium   | Medium     |
| Model Theft      | Attackers steal model weights               | No encryption, open downloads | Model files          | Encryption, watermarking, access control | High     | Medium     |
| API Abuse        | Rate limit bypass, excessive extraction     | Weak auth, no monitoring      | API gateway          | Rate limiting, logging, key security     | High     | Medium     |
| Data Leakage     | Sensitive output exposure                   | No output filtering           | Model responses      | PII detection, differential privacy      | Critical | Medium     |
| Hallucinations   | Model generates false but plausible content | No fact-checking              | Output layer         | RAG, fact-checking modules, HITL         | High     | Medium     |

🔹 Monitoring & Maintenance

| Threat                     | Description                     | Root Cause              | Affected Components | Mitigation                         | Impact   | Likelihood |
| -------------------------- | ------------------------------- | ----------------------- | ------------------- | ---------------------------------- | -------- | ---------- |
| Unauthorized Model Updates | Malicious model version changes | Weak version control    | Model registry      | Git versioning, signed releases    | High     | Low        |
| Shadow AI                  | Unauthorized AI deployment      | No governance inventory | Internal tools      | AI inventory, governance framework | Critical | Low        |
| Lack of Logging            | No traceability of decisions    | No monitoring           | Logging systems     | Real-time monitoring, audit trails | High     | Medium     |
| DoS / Resource Exhaustion  | API overload                    | No rate limiting        | Compute resources   | Request throttling                 | High     | Medium     |
