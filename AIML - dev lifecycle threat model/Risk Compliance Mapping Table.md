Intrinsic & Output Risks (EU AI Act + NIST AI RMF Alignment)

| Risk                        | Regulation Mapping            | Security Controls                        | Impact   | Likelihood |
| --------------------------- | ----------------------------- | ---------------------------------------- | -------- | ---------- |
| Unauthorized Surveillance   | EU AI Act (High Risk), GDPR   | DPIA, consent controls                   | Critical | Low        |
| Model Extraction            | OWASP LLM-06, NIST AI RMF     | Watermarking, encryption                 | High     | Medium     |
| Training Data Poisoning     | NIST AI RMF                   | Data validation, anomaly detection       | High     | Low        |
| Prompt Injection            | OWASP LLM-02                  | Input validation, prompt constraints     | Medium   | Medium     |
| Sensitive Output Disclosure | GDPR Art. 5, 32               | PII detection, privacy filters           | Critical | Medium     |
| Deepfake Misuse             | EU AI Act (Unacceptable Risk) | Watermarking, content detection          | Critical | Medium     |
| Bias & Discrimination       | EU AI Act High Risk           | Fairness testing, inclusive datasets     | Medium   | High       |
| AI-Generated Exploit Code   | OWASP LLM-07                  | Restrict code gen, behavioral monitoring | High     | Low        |

  Risk Scoring Model
  AI Risk Score = (Business Impact × Data Sensitivity) × Likelihood

  Bussiness Impact scale:

  | Score | Impact Level | Description                                     | Example AI Scenario              |
| ----- | ------------ | ----------------------------------------------- | -------------------------------- |
| 1     | Low          | Minor operational disruption                    | Temporary chatbot outage         |
| 2     | Moderate     | Limited service degradation                     | RAG index corruption             |
| 3     | High         | Major service disruption or financial loss      | Model API abuse causing downtime |
| 4     | Severe       | Regulatory violation or major financial loss    | GDPR breach via AI output        |
| 5     | Critical     | Strategic damage, lawsuits, reputational crisis | AI-driven mass data exposure     |

Data Sensitivity Scale
| Score | Data Type        | Description                                          |
| ----- | ---------------- | ---------------------------------------------------- |
| 1     | Public           | Public documents, marketing text                     |
| 2     | Internal         | Non-sensitive internal documentation                 |
| 3     | Confidential     | Business plans, internal reports                     |
| 4     | Sensitive        | Customer data, financial records                     |
| 5     | Highly Sensitive | PII, health data, biometric data, regulated datasets |

Likelihood Scale
| Score | Likelihood     | Description                                |
| ----- | -------------- | ------------------------------------------ |
| 1     | Rare           | Requires advanced capability, low exposure |
| 2     | Possible       | Some exposure exists                       |
| 3     | Likely         | Public-facing or weak controls             |
| 4     | Highly Likely  | Known active exploitation                  |
| 5     | Almost Certain | Frequently exploited pattern               |

Risk Score Interpretation

Maximum Score = (5 × 5) × 5 = 125

| Score Range | Risk Level | Action                           |
| ----------- | ---------- | -------------------------------- |
| 1–20        | Low        | Monitor                          |
| 21–50       | Moderate   | Mitigate within roadmap          |
| 51–80       | High       | Immediate control implementation |
| 81–125      | Critical   | Executive-level escalation       |

