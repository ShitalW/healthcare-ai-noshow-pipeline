# Healthcare Patient Retention & AI Follow-Up Pipeline

## 📌 Project Overview
Hospitals and private clinics experience significant revenue loss when patients miss critical follow-up care appointments. This project combines *Data Analytics* and *AI Automation* to identify high-risk patient demographics and automatically deploy empathetic, personalized email notifications to reduce hospital "no-show" rates.

---

## 📊 Phase 1: Data Analytics & Insights
- *The Dataset:* Processed a real-world medical dataset of 110,000+ patient appointment histories.
- *Data Engineering:* Utilized Google Sheets data filters to remove negative age outliers (-1) and engineered a binary data column (No_Show_Numeric) to standardize mathematical metrics.
- *Key Insight:* Built a dynamic Power BI dashboard proving that patient age group is a powerful predictor of missed appointments (younger patients miss significantly more appointments), while gender factors show no statistical correlation.

### Power BI Trend Analytics
![Power BI Analytics](1_powerbi_chart.png)

### Custom Risk-Flag Engineering Logic
![Spreadsheet Engineering](2_sheets_formula.png)

---

## ⚙️ Phase 2: System Architecture & AI Automation
- *The Trigger Engine:* Connected a Google Sheets database to a Make.com event listener to monitor real-time patient check-ins.
- *AI Integration:* Implemented custom prompt templates utilizing advanced language models (GPT-5.4 mini) to dynamically ingest individual patient metadata (ID, age, specific neighborhood clinic location) into text scripts.
- *Production Delivery:* Wired an active Gmail API node to dynamically deliver the tailored, empathetic notification drafts directly to the user's inbox channel.

### Workflow Automation Map
![Make.com Automation Map](3_make_automation.png)

### Final Production Email Verification
![Final Production Email](4_email_output.png)

---

## 🛠️ Tools & Technologies Used
- *Data Engineering:* Google Sheets (Logical array filtering, IF/AND conditional statements)
- *Business Intelligence:* Power BI Desktop (Data formatting, Line & Clustered column charts)
- *Workflow Automation:* Make.com iPaaS integration environment
- *Artificial Intelligence:* Generative AI Text Models (Dynamic Prompt Engineering)
- *Communication APIs:* Gmail Developer Node Integrations
