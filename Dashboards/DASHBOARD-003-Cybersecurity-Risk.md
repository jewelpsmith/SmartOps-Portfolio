# 📊 DASHBOARD-003: Cybersecurity Risk Dashboard

**Built by:** Jewel Smith, PMP | M.S. Cybersecurity Management & Policy  
**Classification:** ⚠️ SAMPLE TEMPLATE — For Portfolio Demonstration Only  
**Last Updated:** February 2025  
**Category:** Cybersecurity Operations  
**Status:** ✅ Active Template

---

## 🛠️ Tools Used

![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white)
![PowerPoint](https://img.shields.io/badge/PowerPoint-B7472A?style=for-the-badge&logo=microsoft-powerpoint&logoColor=white)
![Canva](https://img.shields.io/badge/Canva-00C4CC?style=for-the-badge&logo=canva&logoColor=white)
![Gamma](https://img.shields.io/badge/Gamma-6C63FF?style=for-the-badge&logoColor=white)
![Perplexity](https://img.shields.io/badge/Perplexity-1FB8CD?style=for-the-badge&logo=perplexity&logoColor=white)
![ChatGPT](https://img.shields.io/badge/ChatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)

---

## 💡 Why This Dashboard Exists

Cybersecurity risk is one of those areas where the 
absence of a visible problem gets mistaken for the 
absence of a problem. Nothing has gone wrong yet so 
everything must be fine. That assumption is exactly 
how organizations end up on the news.

I built this dashboard template during my graduate 
work in Cybersecurity Management and Policy because 
I kept seeing the same gap: organizations had security 
tools generating mountains of data but no clear way 
to communicate risk posture to the people making 
business decisions. Security teams spoke in technical 
language that leadership did not understand and 
leadership made decisions without understanding 
the security implications.

This dashboard bridges that gap. It translates 
technical security data into business-readable risk 
intelligence that an Operations Manager, a CFO, or 
a Board member can understand and act on without 
needing a cybersecurity degree.

It is grounded in the NIST Cybersecurity Framework 
and CompTIA Security+ principles; built to serve 
both technical teams who need operational detail 
and executive stakeholders who need strategic summary.

---

## 📋 Dashboard Structure
```
CYBERSECURITY RISK DASHBOARD
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

SECTION 1: EXECUTIVE RISK SUMMARY
SECTION 2: THREAT LANDSCAPE
SECTION 3: VULNERABILITY STATUS
SECTION 4: CONTROL EFFECTIVENESS
SECTION 5: INCIDENT METRICS
SECTION 6: COMPLIANCE STATUS

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Reporting Period: Monthly; distributed first Monday of month
Owner: IT Security; reviewed by Operations Manager
Distribution: Leadership Team; IT Security; Compliance
Aligned With: NIST CSF; CompTIA Security+ Framework
```

---

## SECTION 1: Executive Risk Summary

This section is written for leaders who need the 
full picture in 60 seconds. No jargon, no technical 
detail; just clear answers to the questions that matter.
```
EXECUTIVE RISK SUMMARY
Month: [Month Year]
══════════════════════════════════════════════════════════

OVERALL SECURITY POSTURE:    🟢 STRONG / 🟡 MODERATE / 🔴 WEAK

WHAT THIS MEANS IN PLAIN TERMS:
[2 to 3 sentence plain language summary of current 
security posture written for a non-technical audience. 
Example: Our security controls are performing well this 
month. One high-rated vulnerability was identified and 
is currently being patched. No security incidents 
occurred during this reporting period.]

KEY NUMBERS THIS MONTH
New Threats Identified:          __
Open Vulnerabilities:            __ (__ Critical; __ High; __ Medium)
Security Incidents:              __
Controls Passing Assessment:     __%
Compliance Items Overdue:        __

TOP RISK THIS MONTH:
[One sentence describing the single highest priority 
risk requiring leadership awareness or decision]

DECISION REQUIRED FROM LEADERSHIP: YES / NO
[If yes, describe what decision is needed and by when]

══════════════════════════════════════════════════════════
```

The executive summary is the most important section 
in this dashboard. It is written last, after all 
other sections are complete, and it reflects the 
full picture without requiring leadership to read 
every detail underneath it.

---

## SECTION 2: Threat Landscape

Understanding what threats are active in the current 
environment is the foundation of effective risk management. 
This section tracks threats relevant to the organization 
based on industry, geography, and operational profile.

**Current Threat Intelligence Summary**

Threat intelligence sourced from CISA alerts, industry 
ISACs, and current research via Perplexity and open 
source intelligence feeds. Updated monthly at minimum; 
updated immediately when a critical threat emerges.
```
ACTIVE THREAT CATEGORIES
Month: [Month Year]
──────────────────────────────────────────────────────────────
THREAT TYPE              CURRENT LEVEL    TREND    RELEVANCE
──────────────────────────────────────────────────────────────
Phishing and Social Eng. 🔴 HIGH          ↑        Direct
Ransomware               🔴 HIGH          ↑        Direct
Supply Chain Attacks     🟡 MEDIUM        →        Direct
Insider Threats          🟡 MEDIUM        →        Direct
DDoS Attacks             🟡 MEDIUM        ↓        Moderate
Zero-Day Exploits        🟡 MEDIUM        ↑        Moderate
Physical Security        🟢 LOW           →        Low
──────────────────────────────────────────────────────────────

RELEVANCE KEY
Direct:    This threat type has been used against 
           organizations in our industry this month
Moderate:  This threat type is active but less 
           targeted toward our industry currently
Low:       This threat type poses minimal risk 
           based on our current environment
```

**Threat Actor Profile**

Organizations in operations and logistics face a 
specific subset of threat actors whose motivations 
and methods shape the risk profile significantly.

Financially motivated criminal groups targeting 
supply chain data and payment systems represent 
the most consistent threat; nation-state actors 
targeting logistics infrastructure in geopolitically 
sensitive regions represent an elevated but lower 
probability risk; and insider threats from employees 
or contractors with excessive access privileges 
represent an often underestimated but highly 
impactful category.

---

## SECTION 3: Vulnerability Status

A vulnerability is a weakness. An exploited vulnerability 
is an incident. The gap between those two outcomes is 
how fast the organization identifies and patches.
```
VULNERABILITY SUMMARY
As of: [Date]
═══════════════════════════════════════════════════════════

OPEN VULNERABILITIES BY SEVERITY

🔴 CRITICAL    __   (Patch required within 24 hours)
🟠 HIGH        __   (Patch required within 7 days)
🟡 MEDIUM      __   (Patch required within 30 days)
🟢 LOW         __   (Patch required within 90 days)

TOTAL OPEN:    __

PATCHING PERFORMANCE
Patches Applied This Month:       __
Critical Patches On Time:         __%  (Target: 100%)
High Patches On Time:             __%  (Target: 95%)
Average Time to Patch (Critical): __ hours (Target: ≤ 24 hours)
Average Time to Patch (High):     __ days  (Target: ≤ 7 days)

SYSTEMS WITH OPEN CRITICAL VULNERABILITIES
[List affected system categories without exposing 
specific system names in this shareable template]

═══════════════════════════════════════════════════════════
```

**Vulnerability Age Tracking**

Vulnerabilities that age past their patching window 
without resolution represent a deliberate acceptance 
of risk that must be documented and approved per 
SOP-006 Risk Assessment. No critical or high 
vulnerability should exceed its patching window 
without written approval from the Operations Manager 
and IT Security Lead.

| Severity | Patching Window | Items Overdue | Oldest Item |
|---|---|---|---|
| Critical | 24 hours | — | — hours |
| High | 7 days | — | — days |
| Medium | 30 days | — | — days |
| Low | 90 days | — | — days |

---

## SECTION 4: Control Effectiveness

Security controls only protect the organization if 
they are working as intended. This section tracks 
whether the controls in place are actually doing 
their job or just existing on paper.

**NIST CSF Function Coverage**
```
NIST CYBERSECURITY FRAMEWORK ASSESSMENT
Month: [Month Year]
────────────────────────────────────────────────────────────
FUNCTION        CONTROLS    PASSING    FAILING    COVERAGE
────────────────────────────────────────────────────────────
IDENTIFY        __          __         __         __%
PROTECT         __          __         __         __%
DETECT          __          __         __         __%
RESPOND         __          __         __         __%
RECOVER         __          __         __         __%
────────────────────────────────────────────────────────────
OVERALL         __          __         __         __%
────────────────────────────────────────────────────────────
Target coverage: ≥ 90% across all functions
```

**Key Control Status**

| Control | Status | Last Tested | Next Review |
|---|---|---|---|
| Multi-Factor Authentication | ✅ Active | [Date] | [Date] |
| Endpoint Detection and Response | ✅ Active | [Date] | [Date] |
| Email Security and Filtering | ✅ Active | [Date] | [Date] |
| Data Loss Prevention | 🟡 Partial | [Date] | [Date] |
| Network Segmentation | ✅ Active | [Date] | [Date] |
| Backup and Recovery | ✅ Active | [Date] | [Date] |
| Security Awareness Training | 🟡 In Progress | [Date] | [Date] |
| Privileged Access Management | 🔴 Needs Work | [Date] | [Date] |
| Vendor Access Controls | ✅ Active | [Date] | [Date] |
| Incident Response Plan | ✅ Current | [Date] | [Date] |

**Status Key**

✅ Active: Control is implemented and functioning as designed  
🟡 Partial: Control is partially implemented or has known gaps  
🔴 Needs Work: Control is not implemented or is failing assessment  

---

## SECTION 5: Incident Metrics

Past incidents are the most reliable predictor of 
future incidents if patterns are not identified and 
addressed. This section tracks incident history to 
surface those patterns before they repeat.
```
INCIDENT SUMMARY
Month: [Month Year]  |  Year to Date
══════════════════════════════════════════════════════════

                        THIS MONTH    YEAR TO DATE
Total Incidents:            __              __
P1 Critical:                __              __
P2 High:                    __              __
P3 Medium:                  __              __
P4 Low:                     __              __

Avg Detection Time:         __ hours        __ hours
Avg Containment Time:       __ hours        __ hours
Avg Resolution Time:        __ hours        __ hours
Incidents Caused by Phishing:  __%
Incidents Caused by Credentials: __%
Incidents Caused by Unpatched Systems: __%

══════════════════════════════════════════════════════════
```

**Incident Trend Analysis**

Month over month incident trend tells a more important 
story than any single month's numbers. An organization 
whose incident count is declining while detection time 
is improving is building genuine security maturity. 
An organization whose numbers look stable but whose 
incidents are getting more severe has a different 
kind of problem.

| Month | Total | P1/P2 | Avg Detection | Avg Resolution |
|---|---|---|---|---|
| [Month -5] | — | — | — hrs | — hrs |
| [Month -4] | — | — | — hrs | — hrs |
| [Month -3] | — | — | — hrs | — hrs |
| [Month -2] | — | — | — hrs | — hrs |
| [Month -1] | — | — | — hrs | — hrs |
| [Current] | — | — | — hrs | — hrs |

Full incident detail maintained per SOP-003 
Incident Response Procedure.

---

## SECTION 6: Compliance Status

Compliance is not the same as security but failing 
compliance creates legal, financial, and reputational 
risk that leadership needs visibility into alongside 
technical risk.
```
COMPLIANCE CALENDAR STATUS
As of: [Date]
──────────────────────────────────────────────────────────────
REQUIREMENT          FRAMEWORK    DUE DATE    STATUS    OWNER
──────────────────────────────────────────────────────────────
Annual Risk Assessment  NIST      [Date]      ✅ Done   [Name]
Security Awareness Trng Internal  [Date]      🔄 Active [Name]
Access Control Audit    NIST      [Date]      ⚠️ Due    [Name]
IR Tabletop Exercise    Internal  [Date]      🔴 Late   [Name]
Vendor Security Review  ISO 27001 [Date]      ✅ Done   [Name]
Backup Recovery Test    Internal  [Date]      ✅ Done   [Name]
GDPR Data Audit         GDPR      [Date]      🔄 Active [Name]
──────────────────────────────────────────────────────────────

STATUS KEY
✅ Done:    Completed on time
🔄 Active:  Currently in progress; on schedule
⚠️ Due:     Due within 30 days; action needed now
🔴 Late:    Past due date; immediate escalation required
```

**Compliance Risk Statement**

Any item marked Late represents an active compliance 
risk that must be reported to Legal and Compliance 
immediately. Depending on the regulatory framework 
involved, overdue compliance items can trigger audits, 
fines, or mandatory reporting requirements that 
escalate significantly the longer they remain unresolved.

---

## 🎨 Visualization and Presentation Options

**For monthly security team review**
Maintain the full dashboard in Notion with linked 
databases for vulnerabilities, incidents, and 
compliance items. Team updates their sections 
throughout the month; dashboard reflects live status.

**For leadership briefing**
Use Gamma to generate a clean executive version 
focusing on Sections 1, 4, and 6 only. Plain language, 
visual indicators, no technical detail. Distribute 
as shareable link or PDF.

**For board level reporting**
Build in PowerPoint using branded template with 
one slide per section. Use Canva for any custom 
visual elements such as risk heat maps or trend 
charts. Keep it to 8 slides maximum.

**For regulatory or audit purposes**
Export full dashboard from Excel with all supporting 
data included. Maintain version history with date 
stamps on all entries. This becomes your evidence 
package if ever questioned by a regulator or auditor.

---

## 🔐 Data Handling and Classification

This dashboard contains sensitive security intelligence 
that could itself become a target if it fell into 
the wrong hands.

Full dashboard classified as CONFIDENTIAL; distribution 
restricted to authorized leadership and security 
personnel only; executive summary version classified 
as INTERNAL for broader leadership distribution; 
no vulnerability details or incident specifics 
shared outside secure channels; Notion dashboard 
access restricted to IT Security and Operations 
leadership; exported versions stored in secured 
drive with access logging enabled; and printed 
copies handled per the organization's physical 
document security policy.

---

## 📎 Related Documents

SOP-003: Incident Response Procedure  
SOP-006: Risk Assessment Procedure  
DASHBOARD-001: Operations KPI Dashboard  
DASHBOARD-002: Project Health Dashboard
