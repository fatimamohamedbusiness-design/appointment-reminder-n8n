# 4. Appointment Reminder Automation
### n8n + Google Sheets + Gmail

## What It Does
Reads upcoming appointments from a Google Sheet and automatically sends reminder emails to clients 24 hours before their appointment — with zero manual work.

**Use cases:** Clinics, beauty salons, gyms, consultants, tutors

## Workflow
```
Schedule Trigger (runs daily) → Read Google Sheets → Filter Tomorrow's Appointments → Send Reminder Email to Each Client → Update Status in Sheet
```

## Google Sheet Structure
Your sheet needs these columns:
| Column | Example |
|--------|----------|
| Client Name | Ahmed Hassan |
| Email | ahmed@email.com |
| Phone | 0100-000-0000 |
| Service | Consultation |
| Appointment Date | 2025-06-15 |
| Time | 10:00 AM |
| Status | Confirmed |
| Reminder Sent | No → auto-updated to Yes |

## Setup
1. Import `workflow.json` into n8n
2. Connect Gmail credentials
3. Connect Google Sheets — paste your appointments sheet ID
4. Set the Schedule Trigger to run daily at 9:00 AM
5. Activate

## Tools
- [n8n](https://n8n.io) · Google Sheets · Gmail API

---
Built by **Fatma Mohamed** — Business Automation Specialist | [LinkedIn](https://linkedin.com/in/fatmamohamed-remot)