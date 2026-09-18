# Data Ethics Case Study: Historical Bias in Automated Recruitment
--------------------------------------------
> **Notice:** Data Ethics Case Study © 2026 by Harish Senthilkumar is licensed under Creative Commons Attribution-NoDerivatives 4.0 International. To view a copy of this license, visit https://creativecommons.org/licenses/by-nd/4.0/
--------------------------------------------

**Author:** Harish Senthilkumar
**Date:** September 2026
**License:** CC-BY-4.0


## 1. Data Ethics Challenges Encountered/Identified
This case study examines two central data ethics issues:

* **Historical Bias in Training Sets (Deon Item 1.1 - Representation):** When models train on historical data, they learn to reproduce past societal biases and inequalities rather than objectively measuring present applicant merit.

* **Proxy Variable Discrimination (Deon Item 3.2 - Fairness & Auditability):** Simply removing explicit  demographic fields (such as gender or race) does not make a nodel neutral. Algorithms automatically identify correlated "proxy" features-such as specific phrasing, school names, or activities that indirectly encode protected attributes.

---

## 2. Real-World Case Analysis: Automated Resume Screening

### Problem Overview
In 2018, details and information showed up that Amazon abandoned on internal automated hiring enginine developed in 2014. The software scored software developers and other STEM candidates on a 1 to 5 star score scale to moderate recruitment.

### Operational Mechanism 
The machine model trained on resumes subitted to the company over a 10-year operation period. Because the technology sector had historically been dominated by males during this period, the training dataset consisted of large amount of male applicant profiles. This had a large bias.

## Problem Diagram:
    [ 10-Year Historical Resume Dataset ]
                     │
                     ▼
    [ Feature Extraction Engine ]
                     │
                     ▼
    [ Algorithmic Scoring Engine (1–5 Stars) ]
                     │
     ┌───────────────┴───────────────┐
     ▼                               ▼
     Male Applicants            Female Applicants
     Standard Evaluation  |     Systematic Proxy Penalty