# ⚡ AUTOMATION-002: Shipment Delay Alert System

**Built by:** Jewel Smith, PMP | M.S. Cybersecurity Management & Policy  
**Classification:** ⚠️ SAMPLE TEMPLATE — For Portfolio Demonstration Only  
**Last Updated:** January 2025  
**Category:** Logistics Operations Automation  
**Status:** ✅ Active Workflow

---

## 🛠️ Tools Used

![Zapier](https://img.shields.io/badge/Zapier-FF4A00?style=for-the-badge&logo=zapier&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)
![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)
![Slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white)
![ChatGPT](https://img.shields.io/badge/ChatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)
![Perplexity](https://img.shields.io/badge/Perplexity-1FB8CD?style=for-the-badge&logo=perplexity&logoColor=white)

---

## 💡 The Problem This Solves

In logistics, a delayed shipment that nobody knows about 
is far more damaging than a delayed shipment that is being 
actively managed. Customers escalate, operations stall, 
and the team spends more time explaining what happened 
than fixing it.

The old way meant someone checking a tracking spreadsheet 
manually, noticing a delay, sending an email, updating 
Notion, then posting in Slack. By the time all of that 
happened, the delay had already become a crisis.

This automation monitors shipment statuses continuously 
and fires alerts the moment a delay threshold is crossed. 
The right people are notified immediately, the incident 
is logged automatically, and the operations team can 
focus on resolving the issue rather than chasing information.

---

## 🔄 Workflow Overview
```
TRIGGER                        ACTIONS
────────────────────────────────────────────────────────────
Google Sheets row updated:     1. Evaluate delay severity level
Status column changes to       2. Send tiered alert email to 
"Delayed" or "Exception"  →       logistics coordinator
                               3. Post alert in Slack #logistics
                               4. Log exception in Notion tracker
                               5. If P1: escalate to Ops Manager
                               6. Schedule follow-up reminder
────────────────────────────────────────────────────────────
Average response time improvement: from 4 hours to under 15 minutes
```

---

## 📋 Step by Step Workflow Build

### TRIGGER: Google Sheets — Shipment Status Updated

**Platform:** Zapier  
**App:** Google Sheets  
**Trigger Event:** Updated Spreadsheet Row  
**Sheet:** Active Shipment Tracker  
**Condition:** Status column value equals "Delayed" OR "Exception"

**Tracker Columns Used:**
Shipment ID; Carrier; Origin; Destination; Expected Delivery; 
Current Status; Delay Reason; Assigned Coordinator; 
Customer or Stakeholder; Priority Level (P1 to P4)

---

### ACTION 1: Zapier Filter — Evaluate Severity

**App:** Zapier Filter  
**Condition:** Only continue if Status contains "Delayed" or "Exception"

This filter prevents the workflow from firing on routine 
status updates like "In Transit" or "Out for Delivery" 
and ensures alerts only go out when they genuinely need to.

---

### ACTION 2: Gmail — Tiered Alert Email

**App:** Gmail  
**Action:** Send Email  
**To:** {{Assigned Coordinator Email}}  
**CC (P1 only):** {{Operations Manager Email}}

**Subject:** 🚨 Shipment Alert: {{Shipment ID}} — {{Current Status}} — {{Priority Level}}
```
Hi {{Coordinator Name}},

This is an automated alert for the following shipment 
exception requiring your immediate attention:

SHIPMENT DETAILS
Shipment ID:        {{Shipment ID}}
Carrier:            {{Carrier}}
Origin:             {{Origin}}
Destination:        {{Destination}}
Expected Delivery:  {{Expected Delivery}}
Current Status:     {{Current Status}}
Delay Reason:       {{Delay Reason}}
Priority Level:     {{Priority Level}}

REQUIRED ACTIONS BASED ON PRIORITY LEVEL

P1 (Critical): Contact carrier immediately; escalate to 
Operations Manager within 30 minutes; assess rerouting options.

P2 (High): Contact carrier within 1 hour; update stakeholder 
on new estimated delivery; log actions in Notion.

P3 (Medium): Contact carrier within 4 hours; update 
shipment tracker with resolution notes.

P4 (Low): Monitor and update tracker; notify stakeholder 
if delay exceeds 24 hours.

Log all actions taken in the Notion Shipment Exception Tracker.

Operations Automation System
```

---

### ACTION 3: Slack — Logistics Channel Alert

**App:** Slack  
**Action:** Send Channel Message  
**Channel:** #logistics-operations
```
🚨 SHIPMENT EXCEPTION ALERT

Shipment ID: {{Shipment ID}}
Status: {{Current Status}}
Priority: {{Priority Level}}
Carrier: {{Carrier}}
Expected Delivery: {{Expected Delivery}}
Delay Reason: {{Delay Reason}}
Assigned To: {{Coordinator Name}}

Action required per SOP-002. All updates to be logged 
in Notion Exception Tracker. 📋
```

---

### ACTION 4: Notion — Log Exception

**App:** Notion  
**Action:** Create Page in Database  
**Database:** Shipment Exception Tracker

**Fields Auto-Populated:**
- Exception ID: AUTO
- Shipment ID: {{Shipment ID}}
- Date Flagged: {{Today}}
- Carrier: {{Carrier}}
- Status at Flag: {{Current Status}}
- Delay Reason: {{Delay Reason}}
- Priority Level: {{Priority Level}}
- Assigned Coordinator: {{Coordinator Name}}
- Resolution Status: Open
- Resolution Notes: (to be completed manually)
- Date Resolved: (to be completed manually)

Every exception gets a permanent record regardless of 
how it resolves. This data feeds monthly KPI reporting 
and carrier performance reviews.

---

### ACTION 5: Zapier Filter and Gmail — P1 Escalation

**App:** Zapier Filter  
**Condition:** Only continue if Priority Level equals "P1"

**App:** Gmail  
**Action:** Send Email  
**To:** {{Operations Manager Email}}  
**Subject:** 🔴 URGENT ESCALATION: P1 Shipment Exception — {{Shipment ID}}
```
Hi {{Operations Manager Name}},

A Priority 1 shipment exception has been detected and 
requires your immediate attention.

Shipment ID:    {{Shipment ID}}
Carrier:        {{Carrier}}
Destination:    {{Destination}}
Expected:       {{Expected Delivery}}
Status:         {{Current Status}}
Delay Reason:   {{Delay Reason}}
Coordinator:    {{Coordinator Name}}

{{Coordinator Name}} has been notified and should be 
contacting the carrier now. Please confirm you have 
visibility and advise on any business continuity 
decisions that need to be made.

Full exception log is in Notion: [link to tracker]

Operations Automation System
```

---

### ACTION 6: Zapier Delay — Follow-up Reminder

**App:** Zapier Delay  
**Delay:** 4 hours for P1/P2; 24 hours for P3/P4

**App:** Gmail  
**Action:** Send Reminder Email  
**To:** {{Coordinator Email}}  
**Subject:** Follow-up Required: Shipment Exception {{Shipment ID}}
```
Hi {{Coordinator Name}},

This is your automated follow-up reminder for 
Shipment Exception {{Shipment ID}}.

Please confirm the following:

Is this exception resolved? If yes, update the 
status in Google Sheets and log resolution notes in Notion.

Is this exception still active? If yes, provide 
a status update to stakeholders and confirm next steps.

Has this been escalated appropriately based on 
the priority level guidelines in SOP-002?

Operations Automation System
```

---

## 📊 ROI Summary

| Metric | Before Automation | After Automation |
|---|---|---|
| Average detection to notification time | 2 to 4 hours | Under 15 minutes |
| Manual steps per exception | 6 to 8 steps | 0 steps |
| Exception documentation rate | ~60% | 100% |
| Stakeholder satisfaction with updates | Variable | Consistent |
| P1 escalation time | 1 to 2 hours | Under 30 minutes |

---

## 🔐 Security Considerations

Shipment data contains vendor information, delivery 
addresses, and in some cases client PII; all of which 
require deliberate protection throughout this workflow.

Zapier connections authenticated via OAuth and reviewed 
quarterly; shipment tracker access restricted by role 
in Google Sheets; Notion exception tracker access limited 
to Operations and Logistics team members only; P1 escalation 
emails sent to monitored management inboxes exclusively; 
and no sensitive shipment data posted in public Slack channels.

Reference SOP-002 Logistics and Shipment Tracking and 
SOP-003 Incident Response for related procedures.

---

## 🔧 How to Replicate This Workflow

1. Set up Active Shipment Tracker in Google Sheets 
   with all required columns
2. Create Shipment Exception database in Notion
3. Build Zap in Zapier; select Google Sheets as trigger
4. Configure trigger: Updated Row with status filter
5. Add Filter step for Delayed or Exception status values
6. Add Gmail action for coordinator alert email
7. Add Slack action for logistics channel notification
8. Add Notion action for exception logging
9. Add second Filter step for P1 only escalation
10. Add Gmail action for Operations Manager escalation
11. Add Delay step followed by follow-up reminder email
12. Test with sample delayed shipment row
13. Turn Zap on and document in automation registry

---

## 📎 Related Documents

SOP-002: Logistics and Shipment Tracking Procedure  
SOP-003: Incident Response Procedure  
AUTOMATION-001: Employee Onboarding Workflow  
AUTOMATION-003: Project Status Report Automation
