a/f:\hermis agent\skills\productivity\job_proposal_generator\README.md → b/f:\hermis agent\skills\productivity\job_proposal_generator\README.md
@@ -1,138 +1,536 @@
-# 🚀 Job Proposal Generator — Setup Guide
-
-A Hermes Agent skill that generates **tailored Upwork/freelancing proposals** from a job URL. Scrapes the job, matches your portfolio, and outputs a professional proposal.
-
----
-
-## 📁 What's in the folder
-
-```
-job_proposal_generator/
-├── SKILL.md                        # Hermes skill file (don't touch)
-├── README.md                       # This file
-├── scripts/
-│   └── proposal_generator.py       # Main script (don't touch)
-└── references/
-    ├── profile.json                 # ← YOU EDIT: your freelance profile
-    └── workflows.csv                # ← YOU EDIT: your portfolio projects
-```
-
----
-
-## ✅ Step 1: Install scrapling
-
-Open **Terminal** (Command Prompt) and run:
-
-```cmd
-pip install scrapling
-```
-
-If you don't have Python, download it from [python.org](https://python.org) first.
-
----
-
-## 📝 Step 2: Edit your profile
-
-Open **`references/profile.json`** in any text editor (Notepad is fine).
-
-Replace the placeholder values with **your** information:
+# 🚀 Job Proposal Generator for Hermes Agent
+
+Generate **tailored Upwork/freelancing proposals** from a job URL — automatically.
+
+**How it works:** You give a job URL → it scrapes the posting → matches your profile + portfolio → generates a professional proposal.
+
+---
+
+## 📦 What You Need to Provide
+
+Before starting, prepare these **2 files** with your information:
+
+### 1. Your Profile (`profile.json`)
+
+Create a file called `profile.json` with your freelance details:
 
 ```json
 {
   "name": "Your Name",
-  "title": "AI Automation Expert | n8n Developer",
+  "title": "Your Title (e.g. AI Automation Expert | n8n Developer)",
   "hourly_rate": 15,
-  "status": "Rising Talent on Upwork",
+  "status": "Your Status (e.g. Rising Talent, Top Rated)",
   "identity_verified": true,
   "location": "Your City, Country",
-  "experience_years": 5,
-  "background": "5+ years building automation workflows",
+  "timezone": "UTC+5:30",
+  "specializations": [
+    "Your main skill 1",
+    "Your main skill 2"
+  ],
   "tech_stack": {
     "automation_platforms": ["n8n", "Make.com", "Zapier"],
     "ai_llms": ["Claude", "OpenAI GPT"],
-    "integrations": ["REST APIs", "Webhooks"],
+    "integrations": ["REST APIs", "Webhooks", "HubSpot"],
     "databases": ["PostgreSQL", "Supabase"],
     "programming": ["JavaScript", "Python"]
… omitted 646 diff line(s) across 1 additional file(s)/section(s)
