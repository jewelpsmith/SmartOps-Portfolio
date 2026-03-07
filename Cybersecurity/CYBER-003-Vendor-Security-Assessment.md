# 🔐 CYBER-003: Third Party Vendor Security Assessment Checklist

**Built by:** Jewel Smith, PMP | M.S. Cybersecurity Management & Policy  
**Classification:** ⚠️ SAMPLE TEMPLATE — For Portfolio Demonstration Only  
**Last Updated:** December 2024  
**Category:** Vendor Security and Third Party Risk  
**Aligned With:** NIST SP 800-161 | ISO 27001 | SOC 2 Framework

---

## 🛠️ Tools Used

![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white)
![Perplexity](https://img.shields.io/badge/Perplexity-1FB8CD?style=for-the-badge&logo=perplexity&logoColor=white)
![ChatGPT](https://img.shields.io/badge/ChatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)
![PowerPoint](https://img.shields.io/badge/PowerPoint-B7472A?style=for-the-badge&logo=microsoft-powerpoint&logoColor=white)

---

## 💡 Purpose and Context

Your security is only as strong as the weakest 
link in your vendor chain.

That is not a metaphor. Some of the most damaging 
security incidents in recent history were not 
the result of direct attacks on the target 
organization. They were the result of attackers 
compromising a vendor, contractor, or software 
provider who had trusted access to the target's 
systems and using that access as the entry point.

Organizations invest significantly in securing 
their own environments and then hand trusted 
access to dozens of third parties without 
applying anything close to the same scrutiny. 
This checklist exists to close that gap.

It is designed to be completed for every Tier 1 
vendor before access is granted and reviewed 
annually thereafter. It covers the full range 
of security controls that a vendor handling 
sensitive data or systems access should have 
in place; governance, technical controls, 
data handling, incident response, and compliance.

A vendor that cannot answer these questions 
clearly and completely is not ready to be 
a trusted partner regardless of how competitive 
their pricing is or how well the sales conversation went.

---

## 📋 Assessment Overview
```
VENDOR SECURITY ASSESSMENT
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Vendor Name:           [Vendor Name]
Vendor Website:        [URL]
Service Provided:      [Description of service]
Vendor Tier:           Tier 1 (required) / Tier 2 (recommended)
Assessment Date:       [Date]
Assessor Name:         [Name and Title]
Previous Assessment:   [Date or "First Assessment"]
Assessment Method:     Questionnaire / Interview / Documentation Review / All Three

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

VENDOR PRIMARY CONTACTS
Security Contact:      [Name; Title; Email]
Technical Contact:     [Name; Title; Email]
Account Manager:       [Name; Title; Email]
```

---

## SECTION 1: Vendor Organization and Governance

This section establishes whether the vendor 
has the organizational foundation to manage 
security seriously; not just as a checkbox 
but as an actual business priority.

---

### 1.1 Security Leadership
```
Does the vendor have a dedicated security function?

  ☐ Yes; dedicated CISO or equivalent role
  ☐ Yes; security function within IT department
  ☐ No; security managed informally
  ☐ Outsourced to managed security service provider

If yes, who is responsible for security at this vendor?
Name and Title: [response]

How long has this person been in the role?
[response]

Notes: [assessor observations]
```

---

### 1.2 Security Policies and Documentation

| Policy or Document | Exists | Last Reviewed | Provided to Us |
|---|---|---|---|
| Information Security Policy | ☐ Yes ☐ No | [Date] | ☐ Yes ☐ No |
| Acceptable Use Policy | ☐ Yes ☐ No | [Date] | ☐ Yes ☐ No |
| Data Classification Policy | ☐ Yes ☐ No | [Date] | ☐ Yes ☐ No |
| Incident Response Plan | ☐ Yes ☐ No | [Date] | ☐ Yes ☐ No |
| Business Continuity Plan | ☐ Yes ☐ No | [Date] | ☐ Yes ☐ No |
| Vendor Management Policy | ☐ Yes ☐ No | [Date] | ☐ Yes ☐ No |
| Data Retention and Disposal Policy | ☐ Yes ☐ No | [Date] | ☐ Yes ☐ No |

**Assessor Notes:**
[Observations about the quality, currency, and 
completeness of documentation provided]

---

### 1.3 Security Certifications and Audits

Independent certification is one of the strongest 
indicators of a vendor's security maturity because 
it means an external party has verified their 
controls against a recognized standard.
```
CERTIFICATION STATUS

SOC 2 Type II
  Status:       ☐ Current  ☐ Expired  ☐ In Progress  ☐ Not Pursued
  Report Date:  [Date]
  Scope:        [What systems and services are covered]
  Provided:     ☐ Yes  ☐ No  ☐ Summary Only

ISO 27001
  Status:       ☐ Certified  ☐ In Progress  ☐ Not Pursued
  Certifying Body: [Name]
  Expiry Date:  [Date]
  Provided:     ☐ Yes  ☐ No

PCI DSS (if applicable)
  Status:       ☐ Compliant  ☐ In Progress  ☐ Not Applicable
  Last Assessment: [Date]

HITRUST (if applicable)
  Status:       ☐ Certified  ☐ Not Applicable

Most Recent External Security Audit
  Date:         [Date]
  Conducted By: [Name of auditing firm]
  Findings:     ☐ No significant findings
                ☐ Findings with remediation completed
                ☐ Open findings (detail required)
  Open Findings: [List any open findings]
```

---

## SECTION 2: Technical Security Controls

This section evaluates whether the vendor has 
the technical controls in place to protect 
the systems and data that will be accessible 
through this vendor relationship.

---

### 2.1 Access Control
```
IDENTITY AND ACCESS MANAGEMENT

Does the vendor enforce Multi-Factor Authentication?
  ☐ Yes; required for all staff on all systems
  ☐ Yes; required for privileged accounts only
  ☐ Optional; not enforced
  ☐ No

How is access to our data and systems controlled?
  ☐ Role-based access control (RBAC)
  ☐ Individual account provisioning
  ☐ Shared accounts (flag as HIGH RISK)
  ☐ Other: [describe]

How quickly are access permissions revoked 
when an employee leaves the vendor?
  ☐ Same day; automated process
  ☐ Within 24 hours; manual process
  ☐ Within 1 week
  ☐ No defined timeline (flag as HIGH RISK)

Does the vendor conduct regular access reviews?
  ☐ Yes; quarterly
  ☐ Yes; annually
  ☐ No defined review cycle

Are privileged accounts managed separately 
from standard user accounts?
  ☐ Yes; privileged access management (PAM) in place
  ☐ Yes; informal separation
  ☐ No
```

---

### 2.2 Data Protection
```
ENCRYPTION STANDARDS

Data at Rest Encryption:
  ☐ AES-256 or equivalent
  ☐ AES-128
  ☐ Encryption present but standard unknown
  ☐ Not encrypted (flag as CRITICAL RISK)

Data in Transit Encryption:
  ☐ TLS 1.3
  ☐ TLS 1.2
  ☐ TLS 1.1 or below (flag as HIGH RISK)
  ☐ Not encrypted (flag as CRITICAL RISK)

Key Management:
  ☐ Formal key management program with rotation schedule
  ☐ Keys managed but no formal rotation schedule
  ☐ No formal key management

Where will our data be stored?
  Location:     [Country or region]
  Environment:  ☐ Cloud  ☐ On-premises  ☐ Both
  Cloud Provider (if applicable): [Name]
  Data Residency Guarantee: ☐ Yes  ☐ No
```

---

### 2.3 Network and Infrastructure Security

| Control | In Place | Details |
|---|---|---|
| Firewall and network segmentation | ☐ Yes ☐ No | [Details] |
| Intrusion detection or prevention system | ☐ Yes ☐ No | [Details] |
| Endpoint detection and response (EDR) | ☐ Yes ☐ No | [Details] |
| Vulnerability scanning program | ☐ Yes ☐ No | [Frequency] |
| Penetration testing program | ☐ Yes ☐ No | [Last date; frequency] |
| Security information and event management (SIEM) | ☐ Yes ☐ No | [Details] |
| DDoS protection | ☐ Yes ☐ No | [Details] |
| Web application firewall (if applicable) | ☐ Yes ☐ No | [Details] |

---

### 2.4 Logging and Monitoring
```
Does the vendor maintain security logs of 
activity on systems that access our data?
  ☐ Yes; comprehensive logging with defined retention
  ☐ Yes; partial logging
  ☐ No

How long are security logs retained?
  ☐ 12 months or more
  ☐ 6 to 12 months
  ☐ Less than 6 months
  ☐ Unknown

Can the vendor provide logs relevant to our 
data in the event of a security incident?
  ☐ Yes; within 24 hours
  ☐ Yes; timeline undefined
  ☐ No

Is there continuous monitoring of security events?
  ☐ Yes; 24 hours a day 7 days a week
  ☐ Yes; business hours only
  ☐ No
```

---

## SECTION 3: Data Handling and Privacy

---

### 3.1 Data Processing and Storage
```
What categories of our data will this vendor 
process or store?
  ☐ Personally Identifiable Information (PII)
  ☐ Financial data
  ☐ Health information (PHI)
  ☐ Intellectual property or trade secrets
  ☐ Employee data
  ☐ Customer data
  ☐ Operational data only; no sensitive categories

What is the minimum data necessary for this 
vendor to perform their contracted service?
[Describe the minimum data set required]

Does the vendor sub-process our data with 
any fourth parties?
  ☐ No; all processing is internal
  ☐ Yes; list of sub-processors provided
  ☐ Yes; list of sub-processors not provided (flag as HIGH RISK)

Sub-Processors (if applicable):
[List names and what they process]
```

---

### 3.2 Data Retention and Disposal
```
What is the vendor's data retention period 
for our data?
  Period: [Timeframe]
  Policy Document: ☐ Provided  ☐ Not Provided

How is our data disposed of at contract end?
  ☐ Secure deletion with certificate provided
  ☐ Secure deletion without certificate
  ☐ Return of data to us before deletion
  ☐ No defined disposal process (flag as HIGH RISK)

What is the timeline for data disposal 
after contract termination?
  ☐ Within 30 days
  ☐ Within 60 days
  ☐ Within 90 days
  ☐ No defined timeline
```

---

## SECTION 4: Incident Response and Business Continuity

---

### 4.1 Incident Response Capabilities

This section is critically important. When a 
vendor experiences a security incident that 
affects our data, how quickly and effectively 
they respond directly impacts our organization. 
A vendor with a weak incident response capability 
is a high-risk vendor regardless of how strong 
their preventive controls are.
```
Does the vendor have a formal incident 
response plan?
  ☐ Yes; tested within the last 12 months
  ☐ Yes; not tested recently
  ☐ No formal plan

How will the vendor notify us if a security 
incident affects our data or systems?
  ☐ Within 24 hours of discovery
  ☐ Within 48 hours of discovery
  ☐ Within 72 hours of discovery
  ☐ No defined notification timeline (flag as CRITICAL RISK)

Notification Method: [Email / Phone / Both]
Notification Contact: [Name and role at vendor]

Has the vendor experienced any security incidents 
in the past 3 years?
  ☐ No incidents
  ☐ Yes; details provided
  ☐ Yes; details not provided (flag as HIGH RISK)
  ☐ Declined to answer (flag as HIGH RISK)

If yes, describe the incidents and outcomes:
[Vendor response]

Assessor Evaluation of Response:
[Were the incidents handled appropriately? 
What does the response tell us about their 
security culture and capabilities?]
```

---

### 4.2 Business Continuity and Availability
```
What is the vendor's committed uptime SLA 
for services we depend on?
  SLA: [Percentage]
  Measurement Period: [Monthly / Annual]
  Historical Uptime (last 12 months): [Percentage]

Does the vendor have a documented business 
continuity plan?
  ☐ Yes; tested within the last 12 months
  ☐ Yes; not tested recently
  ☐ No

What is the vendor's Recovery Time Objective 
(RTO) for critical systems?
  RTO: [Timeframe]

What is the vendor's Recovery Point Objective 
(RPO) for our data?
  RPO: [Timeframe]

How frequently is our data backed up?
  ☐ Continuous or real-time
  ☐ Daily
  ☐ Weekly
  ☐ No defined backup schedule
  
Are backups stored separately from primary systems?
  ☐ Yes; geographically separate location
  ☐ Yes; separate logical environment
  ☐ No
```

---

## SECTION 5: Staff and Training

---

### 5.1 Personnel Security
```
Does the vendor conduct background checks 
on employees with access to our data?
  ☐ Yes; all employees
  ☐ Yes; employees with privileged access only
  ☐ No

What security training do vendor employees receive?
  ☐ Annual security awareness training; tracked
  ☐ Security training at hire only
  ☐ No formal security training (flag as HIGH RISK)

How does the vendor handle employees who 
violate security policies?
[Vendor response]
```

---

## SECTION 6: Contract and Compliance Requirements

Before this assessment is complete, confirm 
the following contractual security requirements 
are addressed in the vendor contract. Forward 
to Legal for review before execution.
```
CONTRACT SECURITY REQUIREMENTS CHECKLIST

☐ Data Processing Agreement (DPA) or Data Handling 
  Agreement included and signed

☐ Incident notification requirement included; 
  vendor must notify us within 24 hours of any 
  security incident affecting our data

☐ Right to audit clause included for Tier 1 vendors

☐ Sub-processor disclosure and approval requirement included

☐ Data return and deletion requirements at contract 
  end clearly specified

☐ Security standards the vendor must maintain 
  throughout the contract specified

☐ Breach liability and indemnification terms 
  reviewed and approved by Legal

☐ Service Level Agreement (SLA) with defined 
  uptime and response time commitments included

☐ Security assessment right included; we may 
  request updated security information annually
```

---

## SECTION 7: Assessment Scoring and Recommendation

### 7.1 Scoring Summary

Rate each section based on responses collected:

| Section | Max Score | Score Achieved | Percentage | Rating |
|---|---|---|---|---|
| 1. Governance | 20 | | | 🟢 🟡 🔴 |
| 2. Technical Controls | 30 | | | 🟢 🟡 🔴 |
| 3. Data Handling | 20 | | | 🟢 🟡 🔴 |
| 4. Incident Response | 20 | | | 🟢 🟡 🔴 |
| 5. Staff and Training | 10 | | | 🟢 🟡 🔴 |
| **TOTAL** | **100** | | | |
```
SCORING GUIDE

85 to 100:  🟢 APPROVED
            Vendor meets security requirements. 
            Proceed with onboarding per SOP-005.

70 to 84:   🟡 CONDITIONAL APPROVAL
            Vendor meets most requirements but 
            has identified gaps. Proceed only with 
            documented remediation commitments and 
            timeline from vendor. Review in 90 days.

Below 70:   🔴 DO NOT APPROVE
            Vendor does not meet minimum security 
            requirements. Do not proceed until 
            significant improvements are demonstrated 
            and reassessment is completed.
```

### 7.2 Critical Risk Flags

Any of the following findings results in automatic 
DO NOT APPROVE regardless of overall score:
```
☐ Data not encrypted at rest or in transit
☐ Shared accounts used for access to our systems
☐ No defined incident notification timeline
☐ Security incidents declined to disclose
☐ No formal data disposal process
☐ No security awareness training for staff
☐ Active unresolved high or critical audit findings
```

### 7.3 Final Recommendation
```
ASSESSMENT CONCLUSION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Vendor:               [Vendor Name]
Assessment Date:      [Date]
Assessor:             Jewel Smith, PMP | M.S. Cybersecurity
Overall Score:        [Score] out of 100
Critical Flags:       [Number] identified

RECOMMENDATION:
  ☐ APPROVED — Proceed with onboarding
  ☐ CONDITIONAL APPROVAL — Proceed with conditions below
  ☐ DO NOT APPROVE — Reassess after remediation

CONDITIONS (if applicable):
1. [Condition]: [Vendor commitment]: [Deadline]
2. [Condition]: [Vendor commitment]: [Deadline]

NEXT REVIEW DATE: [Date; typically 12 months]

Assessor Signature: ___________________________
Operations Manager Approval: __________________
IT Security Lead Approval: ____________________

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## 📎 Related Documents

SOP-005: Vendor Management Procedure  
SOP-006: Risk Assessment Procedure  
CYBER-001: Security Awareness Training Guide  
CYBER-002: Cybersecurity Risk Assessment Template  
DASHBOARD-003: Cybersecurity Risk Dashboard
