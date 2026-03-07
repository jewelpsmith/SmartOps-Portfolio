# 🔐 CYBER-002: Cybersecurity Risk Assessment Template

**Built by:** Jewel Smith, PMP | M.S. Cybersecurity Management & Policy  
**Classification:** ⚠️ SAMPLE TEMPLATE — For Portfolio Demonstration Only  
**Last Updated:** November 2024  
**Category:** Cybersecurity Risk Management  
**Aligned With:** NIST SP 800-30 Rev. 1 | NIST CSF | CompTIA Security+

---

## 🛠️ Tools Used

![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white)
![Perplexity](https://img.shields.io/badge/Perplexity-1FB8CD?style=for-the-badge&logo=perplexity&logoColor=white)
![ChatGPT](https://img.shields.io/badge/ChatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)
![PowerPoint](https://img.shields.io/badge/PowerPoint-B7472A?style=for-the-badge&logo=microsoft-powerpoint&logoColor=white)

---

## 💡 Purpose and Context

A risk assessment that sits in a folder and gets 
updated once a year because someone in compliance 
asked for it is not a risk assessment. It is a 
document that creates the illusion of risk management 
without providing any of the actual protection.

A real cybersecurity risk assessment is a living 
process that informs decisions, prioritizes resources, 
and gives leadership an honest picture of where 
the organization is exposed and what it is doing 
about it.

This template was developed drawing from graduate 
coursework in Cybersecurity Management and Policy 
combined with practical experience managing 
operational risk in environments where security 
and operational continuity are deeply connected. 
It follows the NIST SP 800-30 risk assessment 
methodology while incorporating operational 
and project management context that purely 
technical frameworks often miss.

The template is designed to be completed by a 
team; not by a single person sitting alone with 
a spreadsheet. Risk identification improves 
significantly when multiple perspectives are 
in the room and the people closest to the 
systems and processes are given space to speak.

---

## 📋 Assessment Overview
```
CYBERSECURITY RISK ASSESSMENT
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Organization:          [Organization Name]
Assessment Scope:      [Systems, processes, locations in scope]
Assessment Lead:       [Name and Title]
Assessment Team:       [List team members and roles]
Assessment Period:     [Start Date] to [End Date]
Previous Assessment:   [Date of last assessment or "First Assessment"]
Regulatory Context:    [Applicable frameworks and regulations]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## PART 1: Establish Context

### 1.1 Organization Profile

Before identifying a single risk, the assessment 
team must agree on the organizational context 
that shapes how risks are evaluated and prioritized.

**Mission and Critical Functions**

What does this organization exist to do and 
what functions are so critical that their 
disruption would constitute a serious impact 
on the organization's ability to operate?
```
Primary Mission: [describe in 2 to 3 sentences]

Critical Functions:
1. [Function name]: [why it is critical and what 
   systems or processes support it]
2. [Function name]: [why it is critical]
3. [Function name]: [why it is critical]
```

**Information Assets Inventory**

Risk cannot be assessed without knowing what 
is at risk. Complete the following for all 
significant information assets within scope.

| Asset ID | Asset Name | Asset Type | Data Classification | Business Owner | Current Location |
|---|---|---|---|---|---|
| AST-001 | [Name] | System / Data / Process | Public / Internal / Confidential / Restricted | [Name] | [On-prem / Cloud / Hybrid] |
| AST-002 | | | | | |
| AST-003 | | | | | |

**Regulatory and Compliance Requirements**

List all applicable regulatory frameworks, 
compliance requirements, and contractual 
obligations that shape the organization's 
security requirements.
```
FRAMEWORK          APPLICABILITY          KEY REQUIREMENTS
NIST CSF           [High / Medium / Low]  [Brief description]
GDPR               [High / Medium / Low]  [Brief description]
HIPAA              [High / Medium / Low]  [Brief description]
PCI DSS            [High / Medium / Low]  [Brief description]
SOC 2              [High / Medium / Low]  [Brief description]
[Other]            [High / Medium / Low]  [Brief description]
```

### 1.2 Risk Appetite Statement

The risk appetite statement is the single most 
important context document for the assessment. 
It defines how much risk the organization is 
willing to accept and therefore how findings 
will be interpreted and what responses are required.
```
RISK APPETITE STATEMENT
[Organization Name] — [Assessment Date]

OVERALL RISK APPETITE: Conservative / Moderate / Aggressive

DEFINITION:
[2 to 3 sentences describing the organization's 
general philosophy toward cybersecurity risk. 
Example: We maintain a moderate risk appetite 
for operational risks that enable business growth 
and a conservative risk appetite for risks affecting 
customer data, regulatory compliance, or business continuity.]

RISK TOLERANCE BY CATEGORY:

Customer and Employee Data:    ZERO TOLERANCE
Financial Systems:             LOW TOLERANCE
Operational Systems:           MODERATE TOLERANCE
Internal Communications:       MODERATE TOLERANCE
Public-Facing Systems:         LOW TOLERANCE
Third-Party Integrations:      MODERATE TOLERANCE
```

---

## PART 2: Threat Identification

### 2.1 Threat Source Catalog

Threats come from different sources with different 
motivations, capabilities, and methods. Identifying 
the relevant threat sources for this specific 
organization shapes which risks deserve the most attention.
```
THREAT SOURCE ASSESSMENT

EXTERNAL THREATS
─────────────────────────────────────────────────────────────
SOURCE              MOTIVATION       CAPABILITY   RELEVANCE
─────────────────────────────────────────────────────────────
Criminal Groups     Financial gain   High         🔴 High
Nation-State        Espionage        Very High    🟡 Medium
Hacktivists         Ideology         Medium       🟢 Low
Script Kiddies      Notoriety        Low          🟡 Medium
Competitors         Advantage        Medium       🟡 Medium
─────────────────────────────────────────────────────────────

INTERNAL THREATS
─────────────────────────────────────────────────────────────
SOURCE              MOTIVATION       CAPABILITY   RELEVANCE
─────────────────────────────────────────────────────────────
Malicious Insider   Financial/Anger  High         🟡 Medium
Negligent Employee  None             Low          🔴 High
Contractor          Varies           Medium       🟡 Medium
Former Employee     Varies           Medium       🟡 Medium
─────────────────────────────────────────────────────────────

ENVIRONMENTAL THREATS
─────────────────────────────────────────────────────────────
SOURCE              EXAMPLES                     RELEVANCE
─────────────────────────────────────────────────────────────
Natural Disasters   Flooding, fire, earthquake   [Assess locally]
Power Disruption    Outages, surges              🟡 Medium
Infrastructure      ISP failures, cloud outages  🟡 Medium
─────────────────────────────────────────────────────────────
```

### 2.2 Threat Event Catalog

For each threat source identified as High or 
Medium relevance, document the specific threat 
events that source could initiate against this organization.

| Threat ID | Threat Source | Threat Event | Attack Vector | Target Asset |
|---|---|---|---|---|
| THR-001 | Criminal Groups | Phishing for credentials | Email | User accounts |
| THR-002 | Criminal Groups | Ransomware deployment | Email / RDP | All systems |
| THR-003 | Negligent Employee | Accidental data disclosure | Email / Cloud | Confidential data |
| THR-004 | Criminal Groups | Supply chain compromise | Third-party software | Core systems |
| THR-005 | Malicious Insider | Unauthorized data exfiltration | Internal access | Restricted data |
| THR-006 | [Add threats] | | | |

---

## PART 3: Vulnerability Assessment

### 3.1 Vulnerability Identification

Vulnerabilities are weaknesses that threat actors 
can exploit. They exist in technology, processes, 
and people; all three categories must be assessed.

**Technical Vulnerabilities**
```
TECHNICAL VULNERABILITY SCAN SUMMARY
Scan Date: [Date]
Scanning Tool: [Tool used]
Systems Scanned: [Number and types]

FINDINGS SUMMARY
Critical:  __
High:      __
Medium:    __
Low:       __
Total:     __

TOP 5 TECHNICAL VULNERABILITIES
1. [Vulnerability description] — Affected Systems: [list]
2. [Vulnerability description] — Affected Systems: [list]
3. [Vulnerability description] — Affected Systems: [list]
4. [Vulnerability description] — Affected Systems: [list]
5. [Vulnerability description] — Affected Systems: [list]
```

**Process Vulnerabilities**

Process vulnerabilities are gaps in how work 
is done that create security exposure. These 
rarely show up in a technical scan but are 
often exploited in real attacks.

| Process Area | Vulnerability Identified | Evidence or Observation |
|---|---|---|
| Access Management | Terminated employees not revoked within 24 hours | HR offboarding process has no IT notification step |
| Patch Management | No formal patch schedule exists | Systems showing 90+ day old patches |
| Vendor Management | No security assessment before onboarding | 3 Tier 1 vendors with no security review on file |
| Incident Response | IR plan not tested in 18 months | Last tabletop exercise date in documentation |
| Data Handling | Sensitive data shared via personal email | Observed in email audit sample |

**Human Vulnerabilities**

Human vulnerabilities reflect gaps in knowledge, 
behavior, or awareness that increase organizational 
risk regardless of technical controls in place.
```
SECURITY AWARENESS ASSESSMENT

Security Awareness Training Completion Rate:    __%
Last Phishing Simulation Click Rate:            __%
MFA Adoption Rate:                              __%
Password Policy Compliance Rate:                __%
Reported Phishing Attempts (last 90 days):      __
Unreported Incidents Discovered in Review:      __

OBSERVATIONS:
[2 to 3 sentences describing the general state 
of security awareness across the organization 
based on the data above]
```

---

## PART 4: Risk Determination

### 4.1 Risk Rating Methodology

Each risk is rated on two dimensions: likelihood 
and impact. The combination produces an overall 
risk score that determines prioritization and 
required response timeline.

**Likelihood Scale**
```
RATING    SCORE    DEFINITION
──────────────────────────────────────────────────────────
Rare        1      Requires highly specific conditions; 
                   no known exploitation of this type 
                   in our industry recently
Unlikely    2      Possible but not expected; some 
                   historical precedent in the industry
Possible    3      Could occur; similar incidents 
                   documented in comparable organizations
Likely      4      Expected to occur at some point; 
                   active threat activity observed
Almost      5      Expected to occur; currently being 
Certain            actively exploited in the wild
──────────────────────────────────────────────────────────
```

**Impact Scale**
```
RATING        SCORE    BUSINESS IMPACT
──────────────────────────────────────────────────────────────
Negligible      1      Minimal disruption; resolved quickly 
                       with no lasting effect on operations, 
                       finances, or reputation
Minor           2      Some disruption; manageable with 
                       existing resources; limited customer 
                       or regulatory impact
Moderate        3      Significant disruption; dedicated 
                       response required; potential 
                       regulatory notification; moderate 
                       financial impact
Major           4      Serious operational impact; regulatory 
                       action likely; significant financial 
                       impact; reputational damage possible
Catastrophic    5      Business continuity threatened; 
                       regulatory penalties; severe financial 
                       impact; lasting reputational damage
──────────────────────────────────────────────────────────────
```

**Risk Score Matrix**
```
              IMPACT →
              1         2         3         4         5
           Negligible  Minor   Moderate   Major  Catastrophic
L  5           5        10       15        20        25
I  4           4         8       12        16        20
K  3           3         6        9        12        15
E  2           2         4        6         8        10
L  1           1         2        3         4         5
↑

SCORE RANGE    RISK LEVEL    RESPONSE REQUIRED
1 to 4         🟢 LOW        Monitor; review annually
5 to 9         🟡 MEDIUM     Treat within 90 days
10 to 16       🟠 HIGH       Treat within 30 days
17 to 25       🔴 CRITICAL   Immediate treatment required
```

### 4.2 Risk Register

| Risk ID | Threat Event | Vulnerability Exploited | Likelihood | Impact | Score | Level | Current Controls | Control Effectiveness |
|---|---|---|---|---|---|---|---|---|
| RSK-001 | Phishing for credentials | Low security awareness | 5 | 4 | 20 | 🔴 CRITICAL | Security awareness training | Low; 60% completion rate |
| RSK-002 | Ransomware deployment | Unpatched systems | 4 | 5 | 20 | 🔴 CRITICAL | Antivirus; backups | Medium |
| RSK-003 | Unauthorized data exfiltration | Excessive access privileges | 3 | 4 | 12 | 🟠 HIGH | RBAC policy | Medium |
| RSK-004 | Supply chain compromise | No vendor security assessment | 3 | 4 | 12 | 🟠 HIGH | Vendor contracts | Low |
| RSK-005 | Accidental data disclosure | No DLP controls | 4 | 3 | 12 | 🟠 HIGH | Email policy training | Low |
| RSK-006 | [Add risk] | | | | | | | |

---

## PART 5: Risk Treatment Plan

### 5.1 Treatment Strategy Selection

For each risk in the register, one of four 
treatment strategies is selected based on 
the risk level, cost of treatment, and 
alignment with organizational risk appetite.
```
AVOID:     Eliminate the risk by changing plans or processes
MITIGATE:  Reduce likelihood or impact through controls
TRANSFER:  Shift financial consequence via insurance or contracts
ACCEPT:    Document and approve; typically for LOW risks only

ACCEPTANCE AUTHORITY
LOW risks:      Department Lead approval
MEDIUM risks:   Operations Manager approval
HIGH risks:     Executive Sponsor approval
CRITICAL risks: Executive Sponsor and Legal sign-off required
```

### 5.2 Risk Treatment Register

| Risk ID | Risk Level | Treatment Strategy | Treatment Actions | Owner | Due Date | Residual Risk | Approved By |
|---|---|---|---|---|---|---|---|
| RSK-001 | 🔴 CRITICAL | Mitigate | Mandatory phishing simulation quarterly; security awareness training completion to 100%; MFA enforcement | IT Security | [30 days] | 🟡 MEDIUM | [Name] |
| RSK-002 | 🔴 CRITICAL | Mitigate | Implement formal patch management schedule; critical patches within 24 hours; automated patch reporting | IT Security | [30 days] | 🟡 MEDIUM | [Name] |
| RSK-003 | 🟠 HIGH | Mitigate | Access review and right-sizing within 60 days; privileged access management implementation; quarterly access audits | IT Security | [30 days] | 🟢 LOW | [Name] |
| RSK-004 | 🟠 HIGH | Mitigate | Implement vendor security assessment per SOP-005; all Tier 1 vendors assessed within 90 days | Operations | [60 days] | 🟢 LOW | [Name] |
| RSK-005 | 🟠 HIGH | Mitigate | Implement DLP controls; update data handling training; email audit quarterly | IT Security | [60 days] | 🟡 MEDIUM | [Name] |

---

## PART 6: Executive Summary

The executive summary is written last and 
presented first. It translates the full 
assessment into plain language that leadership 
can act on without reading every section.
```
EXECUTIVE SUMMARY
[Organization Name] Cybersecurity Risk Assessment
[Assessment Date]
Prepared by: [Name], PMP | M.S. Cybersecurity Management & Policy
════════════════════════════════════════════════════════════

OVERALL RISK POSTURE: 🔴 HIGH RISK / 🟡 MODERATE RISK / 🟢 LOW RISK

SUMMARY:
[3 to 4 sentences describing the overall security posture 
in plain language. What is the headline finding? What is 
the most important thing leadership needs to understand 
about the organization's current risk exposure?]

KEY FINDINGS:
1. [Most critical finding with plain language business impact]
2. [Second most critical finding]
3. [Third most critical finding]

IMMEDIATE ACTIONS REQUIRED (Next 30 Days):
1. [Action]: [Owner]: [Expected outcome]
2. [Action]: [Owner]: [Expected outcome]
3. [Action]: [Owner]: [Expected outcome]

DECISIONS REQUIRED FROM LEADERSHIP:
1. [Decision needed]: [Context]: [Deadline]
2. [Decision needed]: [Context]: [Deadline]

INVESTMENT REQUIRED:
Estimated cost to treat CRITICAL and HIGH risks: $[range]
Estimated cost of NOT treating these risks: $[range]
Recommendation: [1 sentence recommendation]

════════════════════════════════════════════════════════════
Next assessment scheduled: [Date]
Assessment Lead: [Name]
```

---

## PART 7: Assessment Methodology Notes

### Why This Template Follows NIST SP 800-30

NIST SP 800-30 is the federal standard for 
conducting information security risk assessments 
and is widely recognized as the most rigorous 
and credible framework for this type of work. 
Using it as the foundation ensures the assessment 
methodology can withstand scrutiny from auditors, 
regulators, and security professionals regardless 
of their background or preferred framework.

The template intentionally bridges NIST 800-30 
with operational and project management context 
because real organizations do not operate in 
purely technical environments. The people, 
processes, and projects that make an organization 
run are just as much a part of the risk landscape 
as the technology stack and a risk assessment 
that ignores them is incomplete by definition.

### Limitations of This Assessment

No risk assessment is perfect and this one 
is no exception. Risk assessments reflect 
the information available at the time they 
are conducted; new threats emerge, systems 
change, and people change roles. The findings 
here represent a point-in-time snapshot that 
should be treated as the beginning of an 
ongoing risk management conversation rather 
than a definitive and permanent statement 
of the organization's risk posture.

Treat this assessment as a living document. 
Review it when significant changes occur, 
update the risk register as treatments are 
completed, and conduct a full reassessment 
on the schedule defined in the assessment overview.

---

## 📎 Related Documents

SOP-003: Incident Response Procedure  
SOP-006: Risk Assessment Procedure  
DASHBOARD-003: Cybersecurity Risk Dashboard  
CYBER-001: Security Awareness Training Guide  
CYBER-003: Third Party Vendor Security Assessment Checklist
