---
title: Research
nav_order: 2
layout: default
---

```mermaid
flowchart LR
    I["[Input Data]"] --> M[Model]
    M -- Output --> O[output Stream]
    M -- Anomaly Score --> D{Anomaly > Threshold?}
    D -- No --> O
    D -- Yes --> S[Save Input Data]
    S --> MS[" (Main Store)"]
```