## MLOps Security Lifecycle (Research View)

This diagram models security risks and controls across a traditional machine learning lifecycle, emphasizing training integrity and deployment protection.

```mermaid
flowchart TD

%% ===== PIPELINE (Light Grey) =====
subgraph MLOps_Pipeline
D[Data Sources]
DP[Data Processing]
T[Model Training]
VAL[Validation]
DEP[Deployment]
end

D --> DP --> T --> VAL --> DEP

%% ===== RISKS (Light Pink) =====
R1[Data Poisoning]
R2[Dataset Leakage]
R3[Model Tampering]
R4[Model Extraction]

%% ===== CONTROLS (Light Green) =====
C1[Data Sanitization]
C2[Secure Training]
C3[Integrity Checks]
C4[Access Control]

%% Connections
R1 --> DP
R2 --> DP
R3 --> VAL
R4 --> DEP

C1 --> DP
C2 --> T
C3 --> VAL
C4 --> DEP

%% ===== ACCESSIBLE COLORS =====
%% Using light fills with dark strokes for high contrast in Dark Mode
classDef pipeline fill:#E5E4E2,color:#000,stroke:#333,stroke-width:2px;
classDef risk fill:#FFB6C1,color:#000,stroke:#333,stroke-width:2px;
classDef control fill:#BDFFA4,color:#000,stroke:#333,stroke-width:2px;
classDef highlight fill:#FFFFC5,color:#000,stroke:#333,stroke-width:2px;

class D,DP,T,VAL,DEP pipeline;
class R1,R2,R3,R4 risk;
class C1,C2,C3,C4 control;

```
