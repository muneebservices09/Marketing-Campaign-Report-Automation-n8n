# 📊 Marketing-Campaign-Report-Automation-n8n

![n8n](https://img.shields.io/badge/Workflow-n8n-FF6C37?style=flat&logo=n8n&logoColor=white)
![OpenAI](https://img.shields.io/badge/AI-GPT--4o-412991?style=flat&logo=openai&logoColor=white)
![Slack](https://img.shields.io/badge/Alerts-Slack-4A154B?style=flat&logo=slack&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Data-Google_Sheets-34A853?style=flat&logo=googlesheets&logoColor=white)
![Google Drive](https://img.shields.io/badge/Docs-Google_Drive-4285F4?style=flat&logo=googledrive&logoColor=white)

---

## 📺 Project Demo
Experience the autonomous journey from raw data ingestion to executive document delivery.

https://www.loom.com/share/d99db33a23dc47e0840b0327ad7c1cf7

---

## 🚀 The Solution: Autonomous Marketing Intelligence
In fast-paced marketing environments, manual reporting is a significant drain on resources. This project is a **Fully Autonomous Marketing Reporting Pipeline** that transforms raw campaign data into professional, executive-level reports. 

The system operates as a 24/7 data analyst: it monitors campaign performance in **Google Sheets**, utilizes **OpenAI** to synthesize insights and recommendations, generates perfectly formatted **Google Docs**, and delivers real-time notifications via **Slack**. This ensures that stakeholders stay informed with zero manual effort. 🤖📈✨

---

## 📊 Business Impact & Engineering Outcomes
This automation is engineered to maximize marketing team efficiency and data visibility:

*   **⏱️ 100% Time Reclaimed:** Eliminates the several hours typically spent every week manually aggregating data and drafting performance summaries.
*   **🧠 AI-Driven Insights:** Goes beyond simple numbers by using GPT-4o to identify trends, outliers, and strategic "Next Steps" for campaign optimization.
*   **🛠️ Zero-Format Friction:** Automatically converts complex Markdown analysis into styled HTML and then into a structured Google Doc, ensuring every report looks identical and professional.
*   **🛡️ Robust Monitoring:** Implements a dual-channel Slack logic—Stakeholders get the "Success" report link, while the Technical team gets diagnostic "Error" alerts if data sources are malformed.

---

## ✅ Problems Solved
- **🛑 Reporting Inconsistency:** No more rushed or skipped reports; the system triggers on a strict weekly schedule without fail. ⏳
- **🛑 Data Integrity Issues:** Includes a "Data Quality Gate" that validates Google Sheets input before triggering the AI, preventing "Garbage-In, Garbage-Out" reporting. 🎯
- **🛑 Notification Fatigue:** Replaces long email threads with clean, actionable Slack summaries containing direct links to the generated documents. 💬
- **🛑 Manual Document Filing:** Automatically organizes reports within a specific Google Drive hierarchy for easy historical access and audits. 📂

---

## 🖼️ System Architecture

### Workflow Orchestration (Marketing Intelligence Pipeline)
The master blueprint of the automation logic—from scheduled data ingestion to multi-channel reporting and error handling.
<div align="center">
  <img src="https://raw.githubusercontent.com/Muneeb20019/n8n-Slack-Marketing-Automation/main/n8n-slack%20workflow.png" width="100%" alt="n8n Marketing Workflow Architecture" style="border-radius:10px; box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);"/>
</div>

---

## 🧠 Core Technical Pillars

### 1. 🔍 Automated Ingress & Validation (Google Sheets)
The workflow acts as a data watchdog. It retrieves weekly campaign metrics via the **Google Sheets API**. Before processing, a specialized node validates the data rows; if the source is empty or invalid, the workflow intelligently diverts to an **Error Routing Path** to alert the admin.

### 2. 🤖 AI Content Synthesis (OpenAI GPT-4o)
The core "Analyst" is a custom-prompted OpenAI agent. It processes raw metrics (Clicks, Spend, Conversions, ROI) to generate:
- **Executive Summaries:** High-level performance overviews.
- **Structured Data Tables:** Formatted Markdown tables for clear comparison.
- **Actionable Recommendations:** Strategic advice based on current week trends. 🧠🔍

### 3. 📄 Dynamic Document Persistence (Google Drive)
To provide a permanent record, the system utilizes a high-fidelity conversion process:
- **Markdown-to-HTML:** A JavaScript node transforms AI output into styled HTML.
- **Automatic Doc Conversion:** The **Google Drive API** ingests the HTML and converts it into a natively formatted Google Doc with proper headings, tables, and spacing. 💻📑

### 4. 📢 Dual-Channel Slack Communication
The system utilizes **Slack** as the primary notification hub:
- **Stakeholder Channel:** Sends a "Success" message with a report summary and a direct link to the Google Doc.
- **Diagnostic Channel:** If the pipeline fails (API timeout or Data error), a detailed diagnostic alert is sent to an internal channel for immediate troubleshooting. 📡🛠️

---

## 🛠️ Technical Stack
| Layer | Technology |
| :--- | :--- |
| **🔄 Automation** | **n8n** (State Management & Orchestration) |
| **🧠 AI Brain** | **OpenAI GPT-4o** (Insight Generation & Summarization) |
| **💰 Data Source** | **Google Sheets API** (Campaign Metrics Repository) |
| **💾 Storage** | **Google Drive API** (Autonomous Doc Generation) |
| **📢 Communication** | **Slack API** (Success/Error Reporting Hub) |
| **📜 Scripting** | **JavaScript / Node.js** (Data Transformation & HTML Rendering) |

---

## ✍️ Author
**Muneeb Ali Khan**
- **GitHub:** [@Muneeb20019](https://github.com/Muneeb20019)
- **LinkedIn:** [Muneeb Ali Khan](https://www.linkedin.com/in/muneeb-ali-khan-2a1675365)

---

## 📜 License
This project is licensed under the MIT License.
