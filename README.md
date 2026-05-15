<!-- Header -->
<h1 align="center">Vidhi Patel</h1>
<p align="center">
  MS Data Science · Northeastern University, Boston &nbsp;|&nbsp; Machine learning / NLP / Decision Intelligence
</p>
<p align="center">
  <a href="https://www.linkedin.com/in/vidhipatel2174/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:patel.vidhim@northeastern.edu"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" /></a>
</p>

<!-- Stack badges -->
<p align="center">
  <img src="https://img.shields.io/badge/Python-Expert-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black" />
  <img src="https://img.shields.io/badge/SQL-Advanced-003B57?style=flat-square&logo=sqlite&logoColor=white" />
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" />
</p>

---

I build ML systems that go beyond accuracy scores — framing models around decisions, costs, and business outcomes. 11+ months of industry experience across two internships, four end-to-end projects, and one full-stack production application.

Currently: MS Data Science at Northeastern

What I care about: making models that are useful to the humans who have to act on them — whether that's a cardiologist, a retention team, or a recruiting lead.

---

## Projects

### [AI Resume & JD Matcher](https://github.com/vidhi3839/Resume_to_Job_description_Matcher)
`NLP` `Transformer Fine-tuning` `Flask` `React` `MongoDB` `Gemini API`

Fine-tuned Sentence-BERT on 9,544 expert-labeled resume–JD pairs. The pretrained model scored R²=−6.15. After domain fine-tuning: R²=0.6964, CV R²=0.699 ± 0.003 — same architecture, different training data, 50x improvement. Shipped as a full production app: Flask REST API (7 endpoints, JWT auth), React candidate + recruiter dashboards, MongoDB + GridFS, Gemini PDF parsing at 94% accuracy.

> Key insight: domain adaptation matters more than model architecture. A powerful model trained on the wrong data is useless.

---

### [Retail Demand Forecasting & Price Optimisation](https://github.com/vidhi3839/Demand-Forecasting-and-Price-Optimisation)
`PyTorch` `Time Series` `Feature Engineering` `scipy`

4-layer DNN on 787K cleaned UCI retail transactions → R²=0.9513 on held-out temporal test set. Engineered 30 features (lag, rolling stats, cyclical encoding, per-product elasticity). Price optimisation via scipy.optimize simulated +25.8% revenue lift across 3,139 products. Bootstrap ensemble of 10 models quantifies prediction uncertainty — flags which products need human review before pricing decisions. Production thinking, not just a notebook metric.

---

### [Customer Churn Prediction — Decision Intelligence for Retention](https://github.com/vidhi3839/Customer-Churn-Analysis)
`Random Forest` `ROI Framework` `Cost-Benefit Analysis`

Reframed the problem around a 21:1 cost asymmetry ($2,101 CLV lost vs $100 to intervene). That changed the right metric from accuracy to recall, and changed which customers to target. RF: AUC=0.844, Recall=0.770. Top-15% risk targeting → 8.6:1 ROI, $903K value retained at $106K cost. Positive ROI even at 40% intervention effectiveness. Three actionable churn drivers surfaced: contract type (15x risk), tenure (4x in month 1–12), payment method (3x for electronic check).

---

### [Clinical Heart Disease Risk + MedGemma Zero-Shot Evaluation](https://github.com/vidhi3839/Clinical_Decision_Support_for_Heart_Disease_Risk_Assessment)
`Clinical ML` `Bootstrap Testing` `Streamlit` `MedGemma-4B` `HuggingFace`

Selected LR (91.7%, AUC=0.911) over XGBoost after a 1,000-sample bootstrap test confirmed the 6.7pp accuracy gap was statistical noise (p=0.975) — prioritising clinical interpretability for physician adoption. Exercise stress indicators (thal r=0.52) far outperform cholesterol (r=0.08) and fasting blood sugar (r=0.00), shifting clinical focus from metabolic screening to functional capacity.

**Independent research extension**: Evaluated Google MedGemma-4B zero-shot on 500 chest X-rays. Found 100% specificity but only 12.4% sensitivity for pneumonia — the model defaults to negative findings without fine-tuning. Identified three next research directions: few-shot prompting, LoRA fine-tuning, and cross-modality generalisation on MedGemma 1.5's CT/MRI capabilities.

---

### [Zero-Shot Evaluation of MedGemma-4B on Chest X-Ray Classification](https://github.com/vidhi3839/medgemma-chest-xray-evaluation)
`Medical AI` `HuggingFace` `PyTorch` `Zero-Shot` `Clinical Evaluation`

Independent research evaluating Google's MedGemma-4B on 500 chest X-rays without any
fine-tuning. Found a systematic sensitivity gap: 100% specificity but only 12.4% sensitivity
for pneumonia — the model defaults to negative findings out of the box. Built the full
evaluation pipeline independently: dataset prep, model loading, confusion matrix analysis,
results visualisation on T4 GPU. Findings connect directly to limitations noted in the
Med-Gemini paper (Saab et al., 2024).

Next directions: few-shot prompting, LoRA fine-tuning, cross-modality testing on
MedGemma 1.5's CT/MRI capabilities (released Jan 2026).

---

## Experience

**Data Science Intern** — Elecon Engineering (IT & Consulting Division), Jan–Jul 2025  
Built an end-to-end customer intelligence system on 100K+ transaction records and 20K+ unstructured B2B feedback comments. Three connected layers: NLP sentiment classifier (~85% F1, 88% negative recall), K-Means segmentation (8,200+ at-risk clients identified, Silhouette 0.38 → 0.58), LDA topic modelling (top 2 themes = 48% of all complaint volume). Power BI dashboard used in weekly client review meetings. Findings incorporated into Q3 client servicing roadmap.

**Data Analyst Intern** — Rishabh Software, May–Aug 2024  
SQL on 50–80K rows of delivery data. Surfaced quarter-end delay spikes (months 3 & 9) that directly changed the PM team's resource allocation plan. Automated 3 recurring Excel reports via Python (-30% manual effort). Built Power BI dashboards (6–8 KPI visuals, DAX) for weekly stakeholder reporting across leadership and client teams.

---

## Currently working on

- MS coursework at Northeastern: Advanced ML, Causal Inference, Data Engineering  
- Extending the MedGemma evaluation — few-shot prompting + LoRA fine-tuning experiments  
- Open to: Applied Scientist Intern · Product DS · Decision Scientist · Business DS · Research roles

---

## GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true&theme=default&hide_border=true&count_private=true" height="165" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_USERNAME&layout=compact&theme=default&hide_border=true&langs_count=6" height="165" />
</p>

<picture>
  <source media="(prefers-color-scheme: dark)"
    srcset="https://raw.githubusercontent.com/vidhi3839/vidhi3839/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)"
    srcset="https://raw.githubusercontent.com/vidhi3839/vidhi3839/output/github-snake.svg" />
  <img alt="contribution snake" src="https://raw.githubusercontent.com/vidhi3839/vidhi3839/output/github-snake.svg" />
</picture>

---

<p align="center">
  <a href="https://www.linkedin.com/in/vidhipatel2174/">LinkedIn</a> &nbsp;·&nbsp;
  <a href="mailto:patel.vidhim@northeastern.edu">Email</a> &nbsp;·&nbsp;
</p>
