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
                     \/
    [ Feature Extraction Engine ]
                     │
                     \/
    [ Algorithmic Scoring Engine (1–5 Stars) ]
                     │
     ┌───────────────┴───────────────┐
     \/                               \/
     Male Applicants            Female Applicants
     Standard Evaluation  |     Systematic Proxy Penalty

The system learned that male and their attributes correlated highly with higher hiring rate. When researchers studied this and try to remove the obvious gender variables, the model got used to the environment by penalizing resumes that contained proxy indicators, like the word *"women's"* (e.g., *"women's chess club captain"*) or graduates of all-women colleges.

---

## 3. Author Analysis and Mitigation Framework

### Personal Reflection and Academic Citations
Removing all features such as gender or anything relative to gender doesn't make the model fair and can lead to a skew, because algorithms are built to find hidden patterns. Those gender featuures are necessary to make additional statistical pattern recognition. When obvious demographic fields are deleted, the model uses other clues like extracurriculars or education as proxy/substitute variable to replce the missing information.

Traditional software engineering and data science process errors cause immediate code breakdowns that are easy to spot because of the compiler, but historical dataset bias is completly invincible to that standard error log and it just automates with the remainign data(including human discrimination categories).

Because of these hidden factors and risks, machine learning engineers and technical statistician must execute through data audits, analysis, and fairness checks rather than treating algorithm as a default tool. AI systems should be treated as a back-up assistant rather than a go-to decision maker.

### Technical Safeguards and Applicable Recommendations
* **Pre-Training EDA:** Perform demographic audits on historical and past datasets to research representation gaps before selecting a appropriate model.
* **Counterfactual Testing:** Testing models by swapping proxy features like club or university names in test samples to ensure predictions remain common and equal.
* **Human-in-the-Loop:** Humans should always fact check the AI, need to learn to use automated tools only as an advisory tool rather than it having full control as an autonomous rejection algorithm.

---

## 4. References and Academic Citations

1. **Primary Investigative News Report:**  
   Dastin, J. (2018, October 10). *Amazon scraps secret AI recruiting tool that showed bias against women.* Reuters.  
   https://www.reuters.com/article/us-amazon-com-jobs-automation-insight-idUSKCN1MK08G/

2. **Academic Foundation on Algorithmic Disparate Impact:**  
   Barocas, S., & Selbst, A. D. (2016). *Big Data's Disparate Impact.* California Law Review, 104(3), 671–732.  
   https://www.californialawreview.org/print/big-datas-disparate-impact/

3. **Industry Ethics Standard:**  
   DrivenData. (n.d.). *Deon: An ethics checklist for data scientists.*  
   https://deon.drivendata.org/