# 📋 SOP-005: Vendor Management Procedure

**Document Owner:** Jewel Smith, PMP | M.S. Cybersecurity Management & Policy  
**Classification:** ⚠️ SAMPLE TEMPLATE — For Portfolio Demonstration Only  
**Version:** 1.2  
**Last Updated:** February 2025  
**Department:** Operations, Logistics and Procurement  
**Review Cycle:** Bi-Annual  
**Aligned With:** NIST SP 800-161 Supply Chain Risk Management

---

## 1. Purpose

Every vendor you bring into your organization is also bringing 
in their security posture, their processes, and their potential 
vulnerabilities. Most organizations spend enormous energy vetting 
internal employees but will onboard a vendor with nothing more 
than a signed contract and a handshake.

I created this SOP after seeing firsthand how vendor relationships 
that start without structure almost always create operational 
headaches down the line. Missed SLAs, inconsistent communication, 
invoices that do not match scopes of work, and in worst case 
scenarios, security incidents traced back to third-party access 
that nobody thought to revoke.

This document establishes a clear, repeatable process for how 
we identify, evaluate, onboard, manage, and when necessary 
offboard vendors. It is written for operations and procurement 
teams who need practical guidance, not just policy language. 
Every step here has a reason behind it, and that reason is almost 
always rooted in either protecting the organization or making 
sure vendors can actually deliver what they promised.

Good vendor management is not about being difficult to work with. 
It is about being clear, consistent, and professional so that 
vendor relationships actually serve the business instead of 
creating risk for it.

---

## 2. Scope

**This SOP applies to:**

All vendors, suppliers, contractors, and third-party service 
providers who meet ANY of the following criteria:

1. They have access to organizational systems, data, or facilities
2. They are paid from the organizational budget on a recurring basis
3. They provide services that directly impact operations or logistics
4. They handle, store, or transmit organizational or customer data
5. They are involved in the supply chain at any tier

**Vendor Tiers Covered:**
```
TIER 1: CRITICAL VENDORS
These vendors have direct access to sensitive systems or data.
A disruption or breach at their end directly impacts us.
Examples: Cloud providers, IT managed services, payroll processors

TIER 2: OPERATIONAL VENDORS  
Core to day-to-day operations but with limited system access.
Examples: Logistics carriers, facilities management, staffing agencies

TIER 3: STANDARD VENDORS
General goods and services with minimal operational dependency.
Examples: Office supplies, catering, printing services
```

**This SOP does NOT apply to:**

One-time purchases under $500 with no ongoing relationship, 
internal department-to-department service agreements, and 
emergency procurement handled under a separate emergency 
purchasing policy.

---

## 3. Vendor Lifecycle Overview
```
IDENTIFY → EVALUATE → APPROVE → ONBOARD → MANAGE → REVIEW → OFFBOARD
   ↑                                                              ↓
   └──────────────── Continuous Improvement Loop ────────────────┘
```

Every vendor goes through this lifecycle. No shortcuts, 
no exceptions for "preferred" vendors who have not been 
formally evaluated.

---

## 4. Roles and Responsibilities

**Procurement Lead**
Owns the vendor identification and evaluation process; 
maintains the vendor registry; coordinates contract execution.

**Operations Manager**
Approves Tier 1 and Tier 2 vendor relationships; reviews 
SLA performance quarterly; makes final offboarding decisions.

**IT Security**
Conducts security assessments for all Tier 1 vendors; 
manages and audits vendor system access; revokes credentials 
upon offboarding.

**Project Manager**
Tracks vendor deliverables against contract terms; escalates 
performance issues; maintains vendor communication logs.

**Legal and Compliance**
Reviews and approves all vendor contracts; ensures data 
handling agreements are in place; assesses regulatory 
implications of vendor relationships.

**Finance**
Manages vendor payment schedules; reconciles invoices 
against approved scopes of work; flags billing discrepancies.

---

## 5. Phase 1: Vendor Identification and Evaluation

### Step 1.1: Business Need Confirmation

Before reaching out to a single vendor, the requesting 
department must document the following:

- What specific need or gap is this vendor filling?
- Why cannot this be handled internally?
- What is the estimated budget and contract duration?
- Which tier does this vendor likely fall into?
- Who internally will own this vendor relationship?

This step exists because too many vendor relationships are 
initiated reactively. Someone needs something fast, they find 
a vendor, sign a contract, and six months later nobody 
remembers why we hired them or what they were supposed to deliver.

### Step 1.2: Market Research and Candidate Identification

Procurement Lead identifies a minimum of three candidate 
vendors for any Tier 1 or Tier 2 engagement. Single-source 
justification must be documented and approved by the 
Operations Manager if fewer than three candidates exist.

Research should cover:

- Company background, financial stability, and years in operation
- Client references; minimum two verifiable references required
- Industry certifications relevant to the service being provided
- Any public records of legal disputes, data breaches, or regulatory violations
- Online reputation and industry standing

### Step 1.3: Security Assessment (Tier 1 Vendors)

IT Security conducts a formal security assessment covering:

**Technical Controls Review**
Does the vendor have documented security policies? Are they 
audited against recognized frameworks such as SOC 2, ISO 27001, 
or NIST? What encryption standards do they use for data at rest 
and in transit?

**Access Requirements Review**
What specific access does this vendor need? Is that access 
the minimum necessary to perform their function? How will 
their access be monitored and logged?

**Incident History Review**
Has this vendor experienced any security incidents in the 
past three years? How did they respond? What changes did 
they make afterward?

A vendor that cannot answer these questions clearly is 
not ready to be a Tier 1 partner regardless of how 
competitive their pricing is.

### Step 1.4: Vendor Scorecard

Each candidate is scored across the following dimensions:

| Evaluation Criteria | Weight | Score (1 to 5) | Weighted Score |
|---|---|---|---|
| Technical Capability | 25% | | |
| Security Posture | 25% | | |
| Pricing and Value | 20% | | |
| References and Reputation | 15% | | |
| Communication and Responsiveness | 15% | | |
| **TOTAL** | **100%** | | |

Minimum passing score for Tier 1 vendors is 3.5 weighted average. 
Tier 2 and 3 vendors require a minimum of 3.0.

---

## 6. Phase 2: Approval and Contract Execution

### Step 2.1: Approval Requirements by Tier
```
TIER 1: Operations Manager + Legal + IT Security sign-off required
TIER 2: Operations Manager approval required
TIER 3: Procurement Lead approval sufficient
```

### Step 2.2: Required Contract Components

Every vendor contract must include the following before execution:

**Non-Negotiable Clauses:**
- Scope of work with specific, measurable deliverables
- Service Level Agreement (SLA) with defined response and resolution times
- Data Handling Agreement covering classification, storage, and disposal
- Right to audit clause for Tier 1 vendors
- Incident notification requirement; vendor must notify us within 24 hours 
  of any security incident that could affect our data or operations
- Termination for cause provisions with clear trigger conditions
- Liability and indemnification terms reviewed by Legal

**Contract Duration Guidelines:**
Tier 1 vendors: Maximum initial term of 12 months with structured renewal review; 
Tier 2 vendors: Maximum initial term of 24 months; 
Tier 3 vendors: As appropriate to the service.

---

## 7. Phase 3: Vendor Onboarding

### Step 3.1: Onboarding Checklist

- [ ] Vendor added to official Vendor Registry with tier classification
- [ ] Primary and secondary contacts documented for both sides
- [ ] IT Security provisions access; scope limited to what contract specifies
- [ ] Vendor signs Acceptable Use Policy before any system access is granted
- [ ] Kickoff meeting scheduled within 5 business days of contract execution
- [ ] Communication cadence established: weekly, bi-weekly, or monthly 
      depending on tier and engagement type
- [ ] Vendor deliverables entered into project management system with due dates
- [ ] Finance sets up vendor in payment system with approved payment terms
- [ ] Vendor provided with escalation contacts on our side

### Step 3.2: Kickoff Meeting Agenda

1. Introductions and relationship overview
2. Scope of work walkthrough; confirm shared understanding
3. SLA review; make sure vendor fully understands consequences of missed targets
4. Communication protocols and reporting requirements
5. Security and data handling expectations
6. Questions and open items; documented and assigned before end of meeting

---

## 8. Phase 4: Ongoing Vendor Management

### Performance Monitoring by Tier

**Tier 1 Vendors:** Monthly SLA review, quarterly business review 
with Operations Manager present, annual security reassessment, 
and continuous monitoring of system access logs by IT Security.

**Tier 2 Vendors:** Quarterly SLA review, bi-annual performance 
check-in, and annual contract review.

**Tier 3 Vendors:** Annual review unless performance issues arise.

### Issue Escalation Process
```
LEVEL 1: Minor issue or single missed SLA target
         Project Manager addresses directly with vendor contact
         
LEVEL 2: Repeated SLA misses or communication breakdown
         Operations Manager engaged; formal written notice issued
         
LEVEL 3: Material breach of contract or security incident
         Legal engaged; potential contract termination assessed
         Operations Manager and IT Security notified immediately
```

### Vendor Performance Documentation

Every significant vendor interaction should be logged. This includes 
SLA performance data, escalations, contract amendments, and 
compliments or complaints received from internal stakeholders. 

If a vendor dispute ever reaches a legal level, the organization 
with better documentation almost always has the stronger position.

---

## 9. Phase 5: Vendor Offboarding

Offboarding is where most organizations drop the ball. A vendor 
relationship ends and system access lingers for months, invoices 
keep coming, and nobody is quite sure who was supposed to handle 
the transition. This phase exists to make sure that does not happen.

### Offboarding Triggers

- Contract end date reached without renewal
- Termination for cause following material breach
- Vendor going out of business or being acquired
- Organizational decision to bring service in-house
- Vendor failing security reassessment

### Offboarding Checklist

- [ ] Formal written notice sent per contract termination terms
- [ ] Transition plan documented and agreed upon with vendor
- [ ] IT Security revokes ALL vendor system access on or before last day
- [ ] All organizational data returned or confirmed deleted by vendor
- [ ] Final invoice reconciled and approved before final payment
- [ ] Vendor removed from active Vendor Registry; moved to archived status
- [ ] Lessons learned documented; what worked, what did not, 
      would we work with this vendor again
- [ ] Internal stakeholders notified of vendor change and transition plan

**Access revocation is not optional and not flexible on timing.**  
IT Security must confirm revocation in writing before offboarding 
is considered complete.

---

## 10. AI Tools Used in Vendor Management

**Notion:** Vendor registry management, performance tracking dashboards, 
and kickoff meeting documentation

**Claude AI:** Drafting vendor communications, RFP templates, 
performance review summaries, and escalation notices

**NotebookLM:** Organizing vendor contracts, SLAs, and compliance 
documentation into searchable knowledge bases

**Excel and Google Sheets:** Vendor scorecards, SLA tracking, 
and cost comparison analysis

**Zapier:** Automated SLA deadline reminders, contract renewal 
alerts sent 90 days before expiration, and onboarding task notifications

---

## 11. Compliance and References

NIST SP 800-161: Supply Chain Risk Management Practices  
ISO 28000: Supply Chain Security Management  
GDPR Article 28: Processor and Sub-Processor Requirements  
Company Acceptable Use Policy  
Company Data Classification Policy  
Company Procurement Policy  

---

## 12. Revision History

| Version | Date | Author | Summary of Changes |
|---|---|---|---|
| 1.0 | August 2024 | Jewel Smith | Initial draft |
| 1.1 | November 2024 | Jewel Smith | Added vendor scorecard and tier framework |
| 1.2 | February 2025 | Jewel Smith | Expanded offboarding section and AI tools |
