## MLOps Security Lifecycle (Research View)

This diagram models security risks and controls across a traditional machine learning lifecycle, emphasizing training integrity and deployment protection.

```mermaid
flowchart LR

%% =====================
%% MLOps Pipeline
%% =====================
subgraph MLOps_Pipeline
D[Data Sources]
DP[Data Processing]
T[Model Training]
VAL[Model Validation]
REG[Model Registry]
DEP[Deployment Service]
end

D --> DP --> T --> VAL --> REG --> DEP

%% =====================
%% Risks
%% =====================
subgraph Risks
R1[Data Poisoning]
R2[Dataset Leakage]
R3[Model Tampering]
R4[Model Extraction]
end

%% =====================
%% Controls
%% =====================
subgraph Security_Controls
C1[Data Sanitization]
C2[Secure Training Environment]
C3[Model Integrity Checks]
C4[Access Control & Monitoring]
end

%% Risk Mapping
R1 --> C1
R2 --> C1
R3 --> C3
R4 --> C4

%% Control Placement
C1 --> DP
C2 --> T
C3 --> VAL
C4 --> REG
C4 --> DEP
```
