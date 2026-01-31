# Multi-Platform Social Media Automation using n8n

## 📌 Overview
This project showcases a **production-grade automation workflow built using n8n** to streamline content publishing across multiple social media platforms. The automation eliminates manual posting by handling scheduling, approval logic, AI-assisted caption generation, and API-based publishing in a reliable, scalable, and maintainable way.

The workflow is designed to run in a **self-hosted n8n environment** and demonstrates real-world automation patterns such as conditional routing, fallback logic, and execution logging.

---

## 🎯 Key Features
- Automated posting to **Facebook, Instagram, LinkedIn, and X**
- **Cron-based scheduling** with timezone-aware execution
- **Google Sheets–based approval and control layer**
- AI-generated captions with platform-specific parsing
- Conditional logic to avoid workflow dead-ends
- Error handling, retries, and execution logging
- Self-hosted, Docker-based deployment

---

## 🧩 Workflow Architecture
Schedule Trigger
↓
Read Approval Sheet
↓
IF Approved Content Exists?
├─ Yes → Use Approved Content
└─ No → Topic Picker → AI Caption Generation
↓
Merge
↓
Multi-Platform Posting (APIs)
↓
Update Sheet with Status & Timestamp

---

## 🛠️ Tech Stack
- **Automation:** n8n (self-hosted)
- **Deployment:** Docker
- **APIs:** Facebook Graph API, LinkedIn API, Instagram Graph API
- **AI:** OpenAI API
- **Data Store:** Google Sheets
- **Logic:** JavaScript (n8n expressions)
- **Scheduling:** Cron triggers

---

## 📂 Repository Structure
/workflows
└── n8n_multiplatform_social_automation.json
/docs
└── workflow-overview.md
└── setup-guide.md
README.md


---

## 🚀 How to Use
1. Import the workflow JSON file into your n8n instance
2. Configure credentials for:
   - Google Sheets
   - Social media platform APIs
   - OpenAI (optional)
3. Update schedule triggers according to your timezone
4. Activate the workflow to start automated posting

---

## ⚠️ Important Notes
- API credentials and tokens are **not included** for security reasons
- This repository is intended for **portfolio and demonstration purposes**
- Platform API permissions must be configured correctly for posting

---

## 📈 Use Cases
- Social media automation for brands and creators
- Content marketing operations
- Approval-driven publishing workflows
- Automation engineering portfolios
- Low-code workflow orchestration demonstrations

---

## 🧠 What This Project Demonstrates
- Real-world n8n workflow design and orchestration
- API integration and OAuth handling
- Conditional logic and merge patterns
- Error-safe, production-ready automation
- Scalable and maintainable workflow architecture

---

## 📜 License
MIT License

---

## 👤 Author
**Sandeep Kothapalli**  
Automation Engineer | n8n Specialist  

GitHub: https://github.com/<your-username>
LinkedIn: https://www.linkedin.com/in/<your-profile>


