#### clinic-salary-automation
# Clinic Salary Automation System
> Automates messy attendance tracking and salary calculations using Google Sheets, Make.com, and ChatGPT. Built for a real multi-department clinic to reduce admin burden, improve payroll accuracy, and generate AI-powered summaries.

## Why I Built This

As someone helping manage a physical therapy, dental, and aesthetic clinic with my sisters, I experienced firsthand how time-consuming and error-prone it can be to manually track staff attendance and calculate salaries. So in order to reduce the workload and improve efficiency, 

I wanted to build a system that would:
- Streamline daily operations
- Reduce manual admin work through automation
- Ensure payroll accuracy across departments and shift types
- Save time for strategic decision-making and minimize human error
- Let me explore ChatGPT integration and no-code tools like Make.com in a real-world solution
- Convert messy, inconsistent time data into reliable insights

This wasn’t just a technical project — it was an operational challenge I chose to take on to improve our family-run clinic, and an opportunity to bring automation and AI into practical, small-business settings. This project became both a **practical solution** for the clinic and my **personal learning journey** in automation, systems thinking, and AI-powered reporting. 

This project also gave me the opportunity to:
- Apply and refine automation logic in real scenarios  
- Explore no-code platforms alongside AI integration
- Work directly with real operational data from a live clinic  
- Build a system that combines technical implementation with business impact
  
### Clinic Salary & Income Automation System
This project aims to automate the internal tracking of staff working hours, calculate monthly salaries, and summarize clinic income using Google Forms, Google Sheets, Make.com, N8N and ChatGPT. The automation helps to reduce manual tasks, increase transparency, and allow for quicker decision-making.

### Objective
- Automate the process of salary calculation for both medical and backend staff based on form-submitted working hours and commission rules.
- Summarize and report monthly and yearly income performance from patient service records.
- Use automation and AI tools to generate reports and summaries, reducing human error and administrative workload.

### Focus Areas
1. **Staff Salary Automation**
- Collect working hour submissions via Google Forms
- Different rules for different roles (e.g., hourly + commission)
- Automatically calculate salary totals
- Generate staff-specific monthly summaries
2. **Clinic Income Automation**
- Collect service income data (daily/monthly)
- Summarize income by staff, service type, or date
- Optionally use ChatGPT to generate a report like:
  > “In June, total clinic revenue was ฿84,200. Dr. A contributed ฿48,000 (57%).”
---
### Impact

- Saved 8+ hours/month of manual salary calculation
- Reduced human error in attendance-based payroll
- Built real-time, scalable backend for a growing clinic team
- Adaptable to other small-medium businesses needing HR automation

---
### System Architecture
> End-to-end data and automation flow using no-code and AI.
```mermaid
flowchart LR
    Form --> Sheets
    Sheets --> Make.com
    Make.com --> GPT
    GPT --> Gmail
    Make.com --> MonthlySummary

---

#### 5. **Add tags / badges** near the top (optional, but stylish):

```
markdown
![Status](https://img.shields.io/badge/status-in%20progress-yellow)
![Tech](https://img.shields.io/badge/tools-Make.com%20%7C%20ChatGPT%20%7C%20GoogleSheets-blue)

---
### Sample Data Structure

| Date | Name | Role | Start | End | Patients | Service | Income |
|------|------|------|-------|-----|----------|---------|--------|
| 2025-06-26 | Dr. A | Doctor | 09:00 | 12:00 | 5 | Consultation | 3,000 |
| 2025-06-26 | Staff B | Reception | 09:00 | 17:00 | – | – | – |
---

### Workflow 
1. Staff check in/out data is exported fingerprint time clocks in .csv format
2. Raw data stored in Google Sheets → transformed into monthly summaries
3. Make.com watches the sheet, calculates salary & OT based on rules, aggregates monthly income
4. ChatGPT summarizes results in prefered language used in the organization
5. Summarize, report or message sent to HR via email / LINE

### Tech Stack & Tools
- *Google Forms* – Input working hours & treatment info
- *Google Sheets* – Central data storage & calculations
- *Make.com* — no-code workflow automation
- *ChatGPT API* — summary generation
- *LINE* — automatic message delivery
- *Gmail* — automatic email delivery
- *[Optional] Google Apps Script* – Custom logic (e.g., timestamp, validation)
- *[Optional] Looker Studio* – Visual income dashboard

### Project Instructions

###  Data Privacy Note

> All datasets used in this repository are anonymized or simulated. No real personal, financial, or patient information is shared publicly in this project. The real implementation is deployed privately.


### Current Status
- [x] Project planning
- [x] Google sheet structure drafted
- [x] Sheet formulas tested
- [x] Make.com workflow operational
- [x] ChatGPT integration complete
- [ ] Income branch in development
- [ ] GitHub Pages site WIP

### 💡 What I Learned

- Designing scalable automation flows with Make.com
- Structuring logic for salary rules using formulas
- Integrating AI with business data for dynamic reports
- Communicating complex automation to others


---
#### .gitignore (Python-Based)
Your current `.gitignore` might look like this if you're using Python for any part of the automation:

