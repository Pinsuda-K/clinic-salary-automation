#### clinic-salary-automation
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

### Tech Stack
- **Google Forms** – Input working hours & treatment info
- **Google Sheets** – Central data storage & calculations
- **Make.com / n8n** – Workflow automation
- **ChatGPT API (OpenAI)** – Income summary generation
- **[Optional] Google Apps Script** – Custom logic (e.g., timestamp, validation)
- **[Optional] Looker Studio** – Visual income dashboard
---
### Sample Data Structure

| Date | Name | Role | Start | End | Patients | Service | Income |
|------|------|------|-------|-----|----------|---------|--------|
| 2025-06-26 | Dr. A | Doctor | 09:00 | 12:00 | 5 | Consultation | 3,000 |
| 2025-06-26 | Staff B | Reception | 09:00 | 17:00 | – | – | – |
---

### Workflow (High-Level)
1. Therapist or staff submits Google Form
2. Data updates Google Sheet
3. Make.com/n8n scenario runs:
   - Calculates salary based on rules
   - Aggregates monthly income
   - (Optional) Uses GPT to summarize insights
4. Report or message sent via email / LINE


###  Data Privacy Note

> All datasets used in this repository are anonymized or simulated. No real personal, financial, or patient information is shared publicly in this project. The real implementation is deployed privately.


### Current Status
- [x] Project planning
- [x] Google Form structure drafted
- [ ] Sample salary rule table
- [ ] Basic automation test in Make.com
- [ ] Integration with ChatGPT (pending)
- [ ] Summary report prototype

### What I'm Learning
- Automation design with Make.com
- Structuring logic-based salary calculations
- Integrating AI tools for business reporting
- Building modular and scalable workflows

---
#### .gitignore (Python-Based)
Your current `.gitignore` might look like this if you're using Python for any part of the automation:

