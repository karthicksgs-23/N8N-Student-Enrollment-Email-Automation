# Student Enrollment Email Automation (n8n + Google Sheets + Gmail)

An automated workflow built with [n8n](https://n8n.io/) that reads student enrollment records from a Google Sheet, validates and formats individual data summaries, and sends personalized notification emails using the Gmail API.

---

## Workflow Architecture

```text
[Schedule Trigger] 
        │
        ▼
[Google Sheets: Read Rows]
        │
        ▼
[Code (JavaScript): Format & Filter]
        │
        ▼
[Gmail: Send Email]
