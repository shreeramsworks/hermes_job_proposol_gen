# 🚀 AI Job Proposal Generator for Hermes

This project enables Hermes to generate personalized, professional freelance proposals from a job URL.

The proposal must be created by understanding the client's requirements, matching them with the freelancer's profile and previous work, and writing a proposal that accurately reflects the freelancer's experience.

---

# Prerequisites

Before using this project, make sure Python is installed.

Download Python from:

https://python.org/downloads/

During installation, enable **Add Python to PATH**.

---

# Install Required Package

This project uses **Scrapling** to extract job information from freelance platforms.

Install it by running:

```bash
pip install scrapling
```

Verify the installation:

```bash
python -c "import scrapling"
```

If the command finishes without any errors, the installation is successful.

---

# Project Structure

```
job_proposal_generator/
│
├── SKILL.md
├── README.md
│
├── scripts/
│   └── proposal_generator.py
│
└── references/
    ├── profile.md
    └── workflows.csv
```

Do not rename or move these files.

---

# Files Provided

Two files will be provided with this project.

## profile.md

This file contains the freelancer's complete professional profile.

Use this file to understand:

- who the freelancer is
- professional background
- experience
- skills
- technologies
- certifications
- services
- industries
- work history
- achievements
- client reviews
- technical expertise
- any other professional information contained in the document

Read the complete file before generating any proposal.

Treat everything inside this file as the primary source of truth for the freelancer.

Never assume information that does not exist in this file.

---

## workflows.csv

This file contains the freelancer's completed projects and portfolio.

Read the entire file.

Analyze every project and use it to identify work that is relevant to the client's requirements.

Whenever possible, reference projects from this file to demonstrate previous experience.

Do not reference projects that are unrelated to the job.

Only use information available in this file.

---

# How Hermes Must Generate Proposals

Whenever a user provides a job URL, Hermes must follow the process below.

## Step 1

Scrape the complete job posting using Scrapling.

Extract every available detail including the title, description, budget, skills, responsibilities, technologies, deliverables, client requirements and any additional information available on the page.

Do not continue until the job has been completely analyzed.

---

## Step 2

Read the uploaded **profile.md** file.

Understand the freelancer's background, technical skills, services, experience, industries, certifications, strengths and overall professional profile.

This information will be used throughout the proposal.

---

## Step 3

Read the uploaded **workflows.csv** file.

Analyze every project.

Determine which projects are the closest match to the client's requirements.

Use only relevant projects.

Ignore unrelated work.

---

## Step 4

Compare the client's requirements against both files.

Identify:

- matching technologies
- matching industries
- matching business problems
- matching services
- matching experience
- matching portfolio projects

Use this comparison to build the proposal.

---

## Step 5

Create a proposal that demonstrates a clear understanding of the client's problem.

The proposal must explain why the freelancer is a good fit by using real experience found in **profile.md** and **workflows.csv**.

Do not invent experience, projects, certifications or achievements.

Do not make assumptions that are not supported by the provided files.

---

# Proposal Requirements

Every proposal should:

- be personalized for the specific job
- directly address the client's requirements
- reference relevant previous work when appropriate
- demonstrate understanding of the business problem
- explain the proposed approach
- maintain a professional and natural writing style
- be concise, confident and easy to read
- avoid generic AI-generated wording
- be ready to submit without additional editing

---

# Important Rules

- Always scrape the job before writing.
- Always read **profile.md** completely.
- Always read **workflows.csv** completely.
- Always use both files when generating the proposal.
- Never skip any step.
- Never invent information.
- Never exaggerate experience.
- Never mention projects that do not exist in the portfolio.
- Never use generic proposal templates.
- Every proposal must be written specifically for the provided job.

---

# Final Task

After reading this document, create a complete Hermes skill in **SKILL.md**.

The generated skill must:

- use Scrapling to scrape the job posting
- read and analyze `profile.md`
- read and analyze `workflows.csv`
- compare the job requirements with the freelancer's experience
- identify the most relevant portfolio projects
- generate personalized proposals based only on the provided information
- follow the complete workflow and rules described in this document
- produce professional proposals that are accurate, truthful, and ready for submission
