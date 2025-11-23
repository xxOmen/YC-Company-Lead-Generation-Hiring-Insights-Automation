
# 🚀 YC Lead Generation & Hiring Insights Automation  
**MIT License**

An intelligent, end-to-end **Lead Generation & Hiring Intelligence System** built for targeting **Y Combinator (YC) companies**, powered by **N8N**, **HTML**, **Google Sheets**, and API-driven enrichment.

This project automates everything — from **company filtering to founder discovery to hiring insights** — without needing any paid CRM or prospecting tool.

## 🧩 Overview
When a user selects their preferences (e.g., company size, remote-only), the system automatically:

1. Pulls the latest list of **Y Combinator companies**  
2. Filters them by **size, remote policy, and category**  
3. Extracts **founder names**, **LinkedIn profiles**, and company details  
4. Checks whether the company is **currently hiring**  
5. Fetches available **job roles** like Head of Marketing, Sales, Engineering, etc.  
6. Sends all enriched results into **Google Sheets** for clean reporting  

## ⚙️ System Workflow
Below is the automation flow built in N8N, integrating the YC API, LinkedIn enrichment, Google Sheets, and conditional logic for full lead generation automation 👇
![Workflow screenshot](https://raw.githubusercontent.com/xxOmen/YC-Company-Lead-Generation-Hiring-Insights-Automation/main/Workflow.png)


## 🎬 Demo Video
🎥 **Watch the Full Automation Demo:**  
👉 [Click here to view the demo](https://drive.google.com/file/d/12VM9dR3X4_2E6tWzH-CtY2XsaE-dvfp8/view?usp=sharing)
*(The demo shows the full workflow — filter selection → data extraction → founder insights → hiring signals → sheet output.)*

## 🧠 Tech Stack
| Technology | Purpose |
|-----------|----------|
| **HTML + CSS** | User input form |
| **Google Sheets** | Lead database |
| **N8N Workflow** | Automation engine |
| **API Nodes** | Fetch & enrich data |
| **Web Scraping** | Supplemental data |
| **AI Logic (optional)** | Smart enrichment |

## 🧾 Key Google Sheets Formulas
```excel
=ARRAYFORMULA(TRIM(CLEAN(A2:A)))
=IF(D2="","NO DATA",IF(D2>0,"HIRING","NOT HIRING"))
=FILTER(Data!A:G, Data!G:G="HIRING")
```

## 📁 Project Structure
/root  
  ├── html-form/  
  ├── n8n-workflow/  
  ├── google-sheets/  
  └── README.md
