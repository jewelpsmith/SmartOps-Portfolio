# ⚡ AUTOMATION-003: Project Status Report Automation

**Built by:** Jewel Smith, PMP | M.S. Cybersecurity Management & Policy  
**Classification:** ⚠️ SAMPLE TEMPLATE — For Portfolio Demonstration Only  
**Last Updated:** February 2025  
**Category:** Project Management Automation  
**Status:** ✅ Active Workflow

---

## 🛠️ Tools Used

![Zapier](https://img.shields.io/badge/Zapier-FF4A00?style=for-the-badge&logo=zapier&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white)
![ChatGPT](https://img.shields.io/badge/ChatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)
![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)
![Slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white)
![Gamma](https://img.shields.io/badge/Gamma-6C63FF?style=for-the-badge&logoColor=white)
![Canva](https://img.shields.io/badge/Canva-00C4CC?style=for-the-badge&logo=canva&logoColor=white)

---

## 💡 The Problem This Solves

Status reporting is one of those tasks that every project 
manager knows is important but almost nobody enjoys doing. 
It takes time that could be spent on actual project work, 
it requires pulling data from multiple sources, and if 
you miss a week, stakeholders start asking questions.

The reality is that most of what goes into a weekly status 
report is already sitting in your project management tools. 
Tasks completed, blockers logged, milestones hit or missed; 
it is all there. The old process meant manually pulling 
that data, formatting it into a readable report, and 
sending it out every single week without fail.

This automation handles the data collection and distribution 
automatically every Friday afternoon. The Project Manager 
reviews, adds context where needed, and approves it. 
The whole process goes from 45 minutes down to about 
10 minutes of human review time.

---

## 🔄 Workflow Overview
```
TRIGGER                         ACTIONS
─────────────────────────────────────────────────────────────
Every Friday at 3:00 PM         1. Pull project data from Notion
(Scheduled Zapier trigger)      2. Compile data into report template
                           →    3. Send draft to Project Manager
                                4. PM reviews and approves via email
                                5. Final report distributed to stakeholders
                                6. Report archived in Google Sheets log
─────────────────────────────────────────────────────────────
Time saved per report: approximately 35 minutes
Annual time saved: approximately 30 hours per project
```

---

## 📋 Step by Step Workflow Build

### TRIGGER: Zapier Schedule — Every Friday at 3:00 PM

**Platform:** Zapier  
**App:** Schedule by Zapier  
**Trigger:** Every Week  
**Day:** Friday  
**Time:** 3:00 PM local time

This trigger fires automatically every Friday regardless 
of whether anyone remembers to run the report. Consistency 
is the entire point.

---

### ACTION 1: Notion — Pull Project Data

**App:** Notion  
**Action:** Find Database Items  
**Database:** Active Projects Tracker  
**Filter:** Status is not equal to "Completed" or "On Hold"

**Data Points Collected:**
- Project name and ID
- Project Manager assigned
- Current phase or sprint
- Tasks completed this week
- Tasks in progress
- Blockers or risks flagged
- Milestones due this week; hit or missed
- Budget status; on track, at risk, or over
- Overall project health; Green, Amber, or Red

---

### ACTION 2: Gmail — Send Draft to Project Manager

**App:** Gmail  
**Action:** Send Email  
**To:** {{Project Manager Email}}  
**Subject:** 📋 Weekly Status Report Draft — Week of {{Date}} — Action Required
```
Hi {{Project Manager Name}},

Your automated weekly status report draft is ready 
for review. Please review the data below, add any 
context or commentary needed, and reply with APPROVE 
to send it to stakeholders or REVISE with your edits.

────────────────────────────────────────
WEEKLY PROJECT STATUS REPORT
Week Ending: {{Friday Date}}
Prepared by: {{Project Manager Name}}, PMP
────────────────────────────────────────

PROJECT HEALTH SUMMARY

{{Project Name}}
Status:          {{Health: Green / Amber / Red}}
Current Phase:   {{Current Phase}}
Budget Status:   {{Budget Status}}

COMPLETED THIS WEEK
{{Tasks Completed This Week}}

IN PROGRESS
{{Tasks Currently In Progress}}

MILESTONES
Due This Week:   {{Milestones Due}}
Achieved:        {{Milestones Hit}}
Missed:          {{Milestones Missed}}

BLOCKERS AND RISKS
{{Blockers Flagged}}

PLANNED FOR NEXT WEEK
{{Tasks Planned Next Week}}

────────────────────────────────────────
Reply APPROVE to send this report to stakeholders.
Reply REVISE with your edits and the updated version 
will be sent on your behalf.

Report will auto-send at 5:00 PM if no response received.
────────────────────────────────────────

Operations Automation System
```

---

### ACTION 3: Zapier Email Parser — Detect Approval

**App:** Email Parser by Zapier  
**Trigger:** Incoming email reply containing "APPROVE"  
**Fallback:** If no reply by 5:00 PM, auto-send original draft

This step reads the Project Manager's reply. If it 
contains APPROVE the final distribution fires immediately. 
If it contains REVISE the edited content is used instead. 
If there is no reply by 5:00 PM the original draft sends 
automatically so stakeholders always receive their report 
on time regardless of how busy the PM's Friday afternoon gets.

---

### ACTION 4: Gmail — Distribute Final Report to Stakeholders

**App:** Gmail  
**Action:** Send Email  
**To:** {{Stakeholder Distribution List}}  
**Subject:** 📊 Weekly Project Status Report — Week of {{Date}}
```
Hi Team,

Please find below the weekly project status report 
for the week ending {{Friday Date}}.

════════════════════════════════════════
WEEKLY PROJECT STATUS REPORT
Week Ending: {{Friday Date}}
Project Manager: {{PM Name}}, PMP
════════════════════════════════════════

PROJECT HEALTH: {{Green / Amber / Red}}

{{Full Report Content}}

════════════════════════════════════════

Questions or concerns about any items in this report 
should be directed to {{PM Name}} at {{PM Email}}.

Next report will be distributed Friday {{Next Friday Date}}.

Regards,
{{PM Name}}
Project Management Office
```

---

### ACTION 5: Slack — Weekly Summary Post

**App:** Slack  
**Action:** Send Channel Message  
**Channel:** #project-updates
```
📊 WEEKLY STATUS REPORT DISTRIBUTED

Week of: {{Friday Date}}
Project Manager: {{PM Name}}
Overall Health: {{Green 🟢 / Amber 🟡 / Red 🔴}}

Summary: {{One sentence project status summary}}

Full report sent to stakeholder distribution list. 
Questions? Reach out to {{PM Name}} directly.
```

---

### ACTION 6: Google Sheets — Archive Report Log

**App:** Google Sheets  
**Action:** Create Spreadsheet Row  
**Sheet:** Status Report Archive

**Fields Logged:**
- Report Date: {{Friday Date}}
- Project Name: {{Project Name}}
- Health Status: {{Green / Amber / Red}}
- PM Approved: Yes or Auto-Sent
- Distributed To: {{Stakeholder Count}} recipients
- Blockers Count: {{Number of Blockers}}
- Milestones Hit: {{Count}}
- Milestones Missed: {{Count}}

This archive creates a running historical record of 
every project's weekly health over time. Invaluable 
for project retrospectives, client reporting, and 
identifying patterns in where projects tend to struggle.

---

## 🎨 Presentation Layer

For stakeholder-facing reports that need more visual 
polish than a plain email, the following tools are 
used to elevate the presentation:

**Gamma**
Used to convert the weekly status data into a clean, 
visually structured presentation that can be shared 
as a link or embedded in stakeholder portals. Takes 
approximately 5 minutes to generate from the report data.

**Canva**
Used for executive-level reporting where branded 
visual templates are required. Project health 
dashboards, milestone trackers, and budget status 
visuals are built in Canva and attached to the 
stakeholder distribution email monthly.

---

## 📊 ROI Summary

| Task | Before Automation | After Automation | Time Saved |
|---|---|---|---|
| Data collection from Notion | 20 minutes | 0 minutes | 20 minutes |
| Report formatting | 15 minutes | 0 minutes | 15 minutes |
| PM review and approval | 10 minutes | 10 minutes | 0 minutes |
| Distribution and Slack post | 5 minutes | 0 minutes | 5 minutes |
| Archive and logging | 5 minutes | 0 minutes | 5 minutes |
| **Total per report** | **55 minutes** | **10 minutes** | **45 minutes** |

Across a 12 month project with weekly reporting that 
is approximately 39 hours of manual work eliminated, 
100% reporting consistency regardless of how busy 
Fridays get, and a complete historical archive that 
previously did not exist.

---

## 🔐 Security Considerations

Project status reports often contain budget figures, 
resource information, and strategic details that are 
confidential to the organization.

Distribution lists are maintained and reviewed monthly 
to ensure only authorized stakeholders receive reports; 
Zapier connections authenticated via OAuth with 
quarterly access review; Google Sheets archive access 
restricted to Project Management Office members only; 
Slack posts contain summary information only with no 
sensitive financial or personnel data included; and 
Gamma and Canva outputs for executive reporting are 
shared via password protected links for sensitive projects.

---

## 🔧 How to Replicate This Workflow

1. Configure Active Projects database in Notion with 
   all required status fields
2. Set up Status Report Archive sheet in Google Sheets
3. Build Zap in Zapier; select Schedule as trigger
4. Configure weekly Friday 3:00 PM schedule
5. Add Notion action to pull active project data
6. Add Gmail action to send draft to Project Manager
7. Add Email Parser step to detect APPROVE response
8. Add Gmail action for stakeholder distribution
9. Add Slack action for channel summary post
10. Add Google Sheets action for archive logging
11. Test full workflow with sample project data
12. Turn Zap on and add to automation registry

---

## 📎 Related Documents

SOP-007: Project Kickoff Procedure  
SOP-006: Risk Assessment Procedure  
AUTOMATION-001: Employee Onboarding Workflow  
AUTOMATION-002: Shipment Delay Alert System
