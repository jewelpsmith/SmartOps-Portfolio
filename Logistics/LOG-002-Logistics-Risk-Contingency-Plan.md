# 📦 LOG-002: Logistics Risk and Contingency Plan

**Built by:** Jewel Smith, PMP | M.S. Cybersecurity Management & Policy  
**Classification:** ⚠️ SAMPLE TEMPLATE — For Portfolio Demonstration Only  
**Last Updated:** December 2024  
**Category:** Logistics Risk Management  
**Review Cycle:** Bi-Annual  
**Aligned With:** NIST SP 800-161 | ISO 28000 | SOP-006 Risk Assessment

---

## 🛠️ Tools Used

![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white)
![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![ChatGPT](https://img.shields.io/badge/ChatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)
![Perplexity](https://img.shields.io/badge/Perplexity-1FB8CD?style=for-the-badge&logo=perplexity&logoColor=white)
![Zapier](https://img.shields.io/badge/Zapier-FF4A00?style=for-the-badge&logo=zapier&logoColor=white)
![PowerPoint](https://img.shields.io/badge/PowerPoint-B7472A?style=for-the-badge&logo=microsoft-powerpoint&logoColor=white)

---

## 💡 Purpose and Context

Logistics operations run on assumptions. We assume 
carriers will deliver on time, vendors will fulfill 
orders as promised, systems will stay online, and 
the supply chain will keep moving the way it moved 
yesterday. Most of the time those assumptions hold. 
When they do not, the organizations that recover 
fastest are the ones that planned for the possibility 
before it became a reality.

This contingency plan was built on two principles 
that I developed through graduate work in Cybersecurity 
Management and Policy and operational experience 
managing logistics environments.

The first principle is that supply chain disruptions 
are not purely operational events anymore. Ransomware 
attacks targeting logistics providers, data breaches 
exposing shipment manifests and customer information, 
and deliberate supply chain infiltration by bad actors 
are documented threats that require a security lens 
applied to operational planning. An organization 
that plans for carrier delays but not for a carrier's 
system being taken offline by a cyberattack is 
planning with incomplete information.

The second principle is that a contingency plan 
nobody has read is not a contingency plan. Every 
scenario in this document is written in plain 
language with specific actions, specific owners, 
and specific timelines so that when something 
goes wrong the team does not have to interpret 
a policy document under pressure. They just 
follow the plan.

---

## 📋 Plan Structure
```
LOGISTICS RISK AND CONTINGENCY PLAN
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

PART 1: Risk Landscape
PART 2: Carrier Disruption Contingencies
PART 3: Supplier and Inventory Contingencies
PART 4: Technology and System Failure Contingencies
PART 5: Cybersecurity and Supply Chain Attack Contingencies
PART 6: Natural Disaster and Force Majeure Contingencies
PART 7: Communication Protocols
PART 8: Plan Testing and Maintenance

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Plan Owner: Operations Manager
Maintained By: Jewel Smith, PMP
Last Tested: [Date]
Next Review: [Date]
Distribution: Operations Team; Logistics Coordinators; 
              IT Security; Leadership
```

---

## PART 1: Risk Landscape

### 1.1 Logistics Risk Categories

Understanding the categories of risk that affect 
logistics operations is the foundation of effective 
contingency planning. Each category requires 
different response strategies and involves 
different stakeholders.
```
RISK CATEGORY OVERVIEW

OPERATIONAL RISKS
Carrier capacity shortages; driver shortages; 
equipment failures; warehouse disruptions; 
port congestion; customs delays; fuel price 
spikes affecting carrier pricing and availability.

SUPPLIER RISKS
Vendor financial instability; production disruptions; 
quality failures; contract disputes; single-source 
dependency; geopolitical disruptions affecting 
supplier regions.

TECHNOLOGY RISKS
Transportation management system outages; 
tracking system failures; EDI communication 
failures; integration disruptions between 
carrier and internal systems.

CYBERSECURITY RISKS
Ransomware attack on carrier systems; data 
breach exposing shipment manifests or customer 
delivery information; business email compromise 
targeting payment or routing changes; supply 
chain infiltration via compromised vendor software.

ENVIRONMENTAL AND EXTERNAL RISKS
Natural disasters affecting transit routes 
or facilities; extreme weather disruptions; 
labor strikes at ports or carriers; regulatory 
changes affecting import or export requirements; 
pandemic or public health disruptions.
```

### 1.2 Risk Priority Matrix
```
LOGISTICS RISK PRIORITY ASSESSMENT
────────────────────────────────────────────────────────────────
RISK                          LIKELIHOOD   IMPACT   PRIORITY
────────────────────────────────────────────────────────────────
Primary carrier capacity loss    Medium      High    🔴 HIGH
Single-source supplier failure   Medium      High    🔴 HIGH
TMS system outage                Low         High    🟡 MEDIUM
Ransomware on carrier systems    Medium      High    🔴 HIGH
Port congestion or closure       Medium      Medium  🟡 MEDIUM
Extreme weather disruption       Medium      Medium  🟡 MEDIUM
Driver or labor strike           Low         High    🟡 MEDIUM
Customs or regulatory delay      Medium      Low     🟢 LOW
Fuel price spike                 High        Low     🟢 LOW
────────────────────────────────────────────────────────────────
```

---

## PART 2: Carrier Disruption Contingencies

### Scenario 2.1: Primary Carrier Capacity Shortage

**Trigger:** Primary carrier unable to accept 
shipments for 48 hours or more due to capacity 
constraints, equipment shortage, or operational issues.

**Impact:** Shipment delays affecting customer 
commitments and operational timelines.
```
IMMEDIATE RESPONSE (First 4 Hours)

Step 1: Logistics Coordinator confirms shortage 
        with carrier account manager in writing
Step 2: Assess volume affected; identify all 
        shipments scheduled in next 7 days
Step 3: Notify Operations Manager immediately
Step 4: Activate backup carrier list (see Section 2.4)
Step 5: Prioritize shipments by urgency and customer impact
Step 6: Communicate proactively with affected stakeholders
        before they ask; do not wait for complaints

ESCALATION
If shortage extends beyond 72 hours:
Operations Manager engages carrier at executive level
Legal reviews contract SLA obligations and remedies
Alternative carrier agreements activated for full volume
```

### Scenario 2.2: Primary Carrier System Outage

**Trigger:** Carrier's technology systems are 
offline affecting tracking, booking, or communication 
capabilities.

**Note:** This scenario increasingly overlaps 
with cybersecurity incidents. A carrier system 
outage in 2025 is as likely to be caused by 
a ransomware attack as by a technical failure. 
Treat the cause as unknown until confirmed and 
follow cybersecurity protocols in parallel with 
operational response.
```
IMMEDIATE RESPONSE

Step 1: Confirm outage with carrier; determine 
        if technology or security incident
Step 2: If security incident suspected; notify 
        IT Security immediately per SOP-003
Step 3: Switch to manual tracking and communication 
        protocols (phone and email confirmation)
Step 4: Increase check-in frequency with carrier 
        to every 2 hours until systems restored
Step 5: Document all manually confirmed shipment 
        statuses in backup tracking spreadsheet
Step 6: Assess whether shipments in transit are 
        at risk of delay due to system outage
Step 7: Notify stakeholders of communication 
        limitations and manual process in place

BACKUP TRACKING PROCEDURE
When carrier tracking portal is unavailable:
Use direct carrier phone contact for status updates
Log all updates in Emergency Tracking Log in Notion
Assign one coordinator per carrier during outage
Provide stakeholder updates every 4 hours minimum
```

### Scenario 2.3: Carrier Contract Termination or Failure

**Trigger:** Carrier relationship terminated for 
cause; carrier ceases operations; or carrier 
fails security assessment requiring immediate removal.
```
RESPONSE TIMELINE

Day 1:   Operations Manager confirms termination decision
         Legal notified; contract termination process initiated
         IT Security revokes carrier system access immediately
         Backup carrier capacity confirmed for full volume
         All in-transit shipments monitored to completion

Day 2:   Affected shipments rerouted to approved carriers
         Vendor registry updated; carrier moved to inactive
         Outstanding invoices reconciled; final payment held 
         pending resolution of any open claims

Day 7:   Transition fully complete
         Lessons learned documented
         Carrier scorecard finalized and archived
         Volume redistribution confirmed with backup carriers
```

### 2.4 Approved Backup Carrier Directory
```
BACKUP CARRIER LIST
Maintained By: Logistics Coordinator
Last Verified: [Date]
────────────────────────────────────────────────────────
CARRIER          TYPE     REGIONS      CONTACT       STATUS
────────────────────────────────────────────────────────
[Carrier A]      Ground   National     [Phone/Email]  Active
[Carrier B]      Air      National     [Phone/Email]  Active
[Carrier C]      LTL      Regional     [Phone/Email]  Active
[Carrier D]      FTL      National     [Phone/Email]  Active
[Carrier E]      Ocean    International [Phone/Email] Active
────────────────────────────────────────────────────────
All backup carriers must have current scorecard 
on file and minimum score of 75 to be on this list.
```

---

## PART 3: Supplier and Inventory Contingencies

### Scenario 3.1: Single-Source Supplier Failure

**Trigger:** Primary supplier unable to fulfill 
orders due to production disruption, financial 
failure, natural disaster, or contract termination.
```
PREVENTION FIRST

The best response to single-source supplier 
failure is to avoid single-source dependency 
wherever operationally feasible. For every 
critical supply category the organization should 
maintain at minimum:

  Primary Supplier:    ≥ 60% of volume
  Secondary Supplier:  ≥ 30% of volume
  Emergency Supplier:  Identified and vetted; 
                       ready to activate within 48 hours

Any critical supply category with only one 
approved supplier must be flagged in the 
risk register per SOP-006 and a secondary 
supplier qualification initiated within 90 days.

RESPONSE IF FAILURE OCCURS

Step 1: Confirm scope and duration with supplier
Step 2: Assess current inventory levels; calculate 
        how long existing stock covers demand
Step 3: Notify Operations Manager and relevant 
        stakeholders immediately
Step 4: Activate secondary or emergency supplier
Step 5: Adjust inbound logistics to support 
        new supply source
Step 6: Communicate impact and timeline to 
        affected internal and external stakeholders
Step 7: Document and update risk register
```

### Scenario 3.2: Inventory Shortage or Stockout
```
INVENTORY RISK THRESHOLDS

GREEN:   Inventory ≥ 30 days supply; no action required
AMBER:   Inventory 15 to 29 days supply; 
         accelerate replenishment; notify Operations Manager
RED:     Inventory below 15 days supply; 
         immediate escalation; emergency procurement initiated

EMERGENCY PROCUREMENT PROTOCOL
Operations Manager approval required
Emergency vendor list activated
Expedited shipping authorized up to [budget limit]
Stakeholders notified of potential impact and timeline
All emergency procurement documented for audit
```

---

## PART 4: Technology and System Failure Contingencies

### Scenario 4.1: Transportation Management System Outage

**Trigger:** TMS or primary logistics platform 
offline for more than 2 hours during business operations.
```
MANUAL OPERATIONS PROTOCOL

Activate emergency tracking spreadsheet in Google Sheets; 
link maintained in Notion emergency resources page.

Shipment Booking: Phone and email confirmation 
with carrier; document confirmation number and 
representative name for every booking.

Status Tracking: Direct carrier contact every 
4 hours for in-transit shipments; log all updates 
manually in emergency tracking spreadsheet.

Stakeholder Updates: Email updates every 4 hours 
to affected stakeholders; do not wait for system 
restoration to communicate.

Documentation: All manual transactions documented 
in real time; entered into TMS within 24 hours 
of system restoration.

SYSTEM RESTORATION CHECKLIST
All manual transactions entered into TMS
Tracking data verified against carrier records
Any discrepancies investigated and resolved
IT Security confirms outage was technical; 
not security-related before full restoration
```

---

## PART 5: Cybersecurity and Supply Chain Attack Contingencies

This section exists because cybersecurity threats 
to supply chains are no longer a future concern; 
they are a present reality. The 2020 SolarWinds 
attack, the 2021 Colonial Pipeline ransomware 
incident, and dozens of subsequent supply chain 
attacks have demonstrated that logistics and 
operations organizations are high-value targets 
and that attacks on vendors and carriers directly 
impact the organizations that depend on them.

### Scenario 5.1: Ransomware Attack on Carrier or Vendor

**Trigger:** Carrier or vendor reports ransomware 
attack affecting their systems; or carrier systems 
go offline in a pattern consistent with ransomware.
```
IMMEDIATE RESPONSE (First 2 Hours)

Step 1: Notify IT Security immediately; do not 
        wait for carrier to confirm it is ransomware
Step 2: IT Security assesses whether our systems 
        or data have been affected via carrier connection
Step 3: Suspend all electronic connections and 
        API integrations with affected carrier
Step 4: Switch to manual communication protocols; 
        phone only until further notice
Step 5: Activate backup carrier for all new shipments
Step 6: Assess in-transit shipments; confirm 
        physical location of all active shipments 
        via phone with carrier operations team
Step 7: Preserve all communication records; 
        this may become a legal or insurance matter

ONGOING RESPONSE

Do not restore electronic connections with 
affected carrier until IT Security confirms 
their systems are clean and our connection 
is safe to re-establish.

Require written security incident report 
from carrier covering: what happened; what 
data was affected; what was done; and what 
controls are now in place.

Assess carrier against security assessment 
checklist per CYBER-003 before restoring 
full relationship.

Operations Manager and Legal assess contract 
SLA implications and any notification obligations.
```

### Scenario 5.2: Business Email Compromise Targeting Logistics

**Trigger:** Suspicious email received requesting 
changes to carrier payment details, delivery 
addresses, or routing instructions. Or confirmed 
fraudulent payment or routing change discovered.
```
PREVENTION

This is one of the most financially damaging 
fraud scenarios in logistics and it works because 
it exploits normal operational workflows.

VERIFICATION RULE: Any request to change payment 
details, banking information, or delivery addresses 
received via email must be verified by phone 
using a number from our records; never a number 
provided in the suspicious email itself.

No exceptions. Not for urgency. Not for senior 
requestors. Not for vendors we have worked with 
for years. The attack specifically targets trusted 
relationships and urgent scenarios.

IF FRAUD IS DISCOVERED

Step 1: Stop any pending payment immediately; 
        contact Finance within minutes not hours
Step 2: Contact bank to attempt payment recall 
        if transfer has been initiated
Step 3: Notify IT Security and Operations Manager immediately
Step 4: Preserve all email communications; 
        do not delete anything
Step 5: Report to FBI Internet Crime Complaint 
        Center (IC3) and local law enforcement
Step 6: Notify Legal; assess disclosure obligations
Step 7: Follow SOP-003 Incident Response procedure
```

### Scenario 5.3: Shipment Data Breach

**Trigger:** Unauthorized access to shipment 
manifests, customer delivery information, or 
logistics system data confirmed or suspected.
```
RESPONSE

Step 1: Follow SOP-003 Incident Response 
        immediately; this is a security incident
Step 2: Identify what data was accessed and 
        whose information is affected
Step 3: Legal and Compliance assess notification 
        obligations; GDPR 72-hour clock starts 
        at discovery if EU data is involved
Step 4: Affected customers or recipients notified 
        per legal requirements and organizational policy
Step 5: Carrier or vendor involved assessed 
        per CYBER-003 security checklist
Step 6: IT Security reviews and hardens access 
        controls to logistics data
```

---

## PART 6: Natural Disaster and Force Majeure Contingencies

### Scenario 6.1: Weather or Natural Disaster Disruption
```
RESPONSE BY SEVERITY

MINOR DISRUPTION (1 to 2 days; localized area)
Monitor carrier updates actively
Communicate proactive delays to stakeholders
No rerouting required; resume normal operations 
when carrier confirms routes clear

MODERATE DISRUPTION (3 to 7 days; regional impact)
Operations Manager notified
Assess all shipments in affected region
Reroute critical shipments through unaffected carriers
Activate backup carriers for new shipments 
originating or destinating in affected area
Daily stakeholder updates until disruption resolved

MAJOR DISRUPTION (More than 7 days; widespread impact)
Executive leadership briefed
Emergency procurement and inventory review initiated
All available carrier capacity secured immediately
Customer and stakeholder communication plan activated
Force majeure clause assessment by Legal
Insurance notification initiated
Daily operations team stand-up until resolved
```

---

## PART 7: Communication Protocols

Effective communication during a logistics 
disruption prevents a manageable problem from 
becoming a crisis. The rule in every scenario 
is the same: communicate early, communicate 
factually, and do not make people chase you 
for information they need.

### 7.1 Internal Communication Chain
```
NOTIFICATION ORDER FOR ALL MAJOR DISRUPTIONS

1. Logistics Coordinator identifies disruption
2. Operations Manager notified within 30 minutes
3. IT Security notified if cybersecurity element present
4. Executive Leadership briefed within 2 hours 
   for HIGH or CRITICAL disruptions
5. Legal and Compliance notified if regulatory 
   implications exist
6. Finance notified if financial impact is material
```

### 7.2 External Stakeholder Communication
```
STAKEHOLDER UPDATE SCHEDULE BY DISRUPTION LEVEL

MINOR:    Single update when disruption identified; 
          follow-up when resolved
MODERATE: Updates every 24 hours until resolved; 
          immediate notification when resolved
MAJOR:    Updates every 4 to 8 hours; dedicated 
          point of contact assigned for stakeholder inquiries

COMMUNICATION PRINCIPLES

Lead with what you know; not what you do not know
Provide estimated resolution timeline even if uncertain; 
update it as information improves
Never promise a resolution date you cannot commit to
Always close the loop when the issue is resolved
Document all external communications for the record
```

---

## PART 8: Plan Testing and Maintenance

A contingency plan that has never been tested 
is a document; not a plan. Testing reveals gaps, 
builds team familiarity, and ensures that when 
a real disruption occurs the response is practiced 
rather than improvised.
```
TESTING SCHEDULE

Tabletop Exercise (bi-annual)
Facilitated discussion walking through 2 to 3 
scenarios from this plan with the full operations 
and logistics team. No live systems affected. 
Focus on decision-making, communication, and 
identifying gaps in the plan.

Carrier Backup Verification (quarterly)
Contact each backup carrier on the approved list 
to confirm current capacity, pricing, and contact 
information. Update the backup carrier directory. 
Remove any carriers that can no longer be activated 
within 48 hours.

Communication Protocol Test (annual)
Test the internal notification chain by simulating 
a disruption scenario and measuring time to 
notification at each level. Identify and address 
any gaps in contact information or escalation paths.

PLAN MAINTENANCE

Review triggered by: any activation of this plan; 
any significant change to carrier relationships 
or supply chain structure; any new cybersecurity 
threat intelligence relevant to logistics operations; 
and annual review regardless of other triggers.

Owner: Jewel Smith, PMP
Approval: Operations Manager
```

---

## 📎 Related Documents

SOP-002: Logistics and Shipment Tracking  
SOP-003: Incident Response Procedure  
SOP-005: Vendor Management Procedure  
SOP-006: Risk Assessment Procedure  
LOG-001: Carrier Performance Scorecard  
CYBER-002: Cybersecurity Risk Assessment Template  
CYBER-003: Third Party Vendor Security Assessment  
DASHBOARD-001: Operations KPI Dashboard
