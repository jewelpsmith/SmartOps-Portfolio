# 🚨 SOP-003: Incident Response Procedure

**Document Owner:** Jewel Smith, PMP | M.S. Cybersecurity Management & Policy  
**Classification:** ⚠️ SAMPLE TEMPLATE — For Portfolio Demonstration Only  
**Severity Framework:** NIST SP 800-61 Rev. 2  
**CompTIA Security+ Aligned**  
**Version:** 2.1 | Last Updated: November 2024  
**Review Cycle:** Every 6 months, no exceptions

---

> 🔴 **This is a living document. If you are reading this during an active 
> incident, go straight to Section 5. Every second counts.**

---

## 1. Purpose

Security incidents do not announce themselves. They do not wait for 
business hours, they do not care about your project deadlines, and 
they do not give you time to figure things out on the fly.

I wrote this SOP because a slow, disorganized response to a security 
incident is almost as damaging as the incident itself. Data gets 
further compromised, evidence gets contaminated, stakeholders lose 
trust, regulatory fines follow, and careers end.

This document exists so that when something goes wrong, and 
eventually something always does, every single person on the 
response team knows exactly what to do, in what order, and who 
owns what. No confusion, no finger pointing, no wasted time.

What makes this different from a generic IR plan is the operational 
lens it is written through. Most incident response documentation is 
written by security engineers for security engineers. This one bridges 
security, operations, and project management because in the real 
world, incidents affect the entire organization, not just IT.

---

## 2. Scope

**What this covers:**

This procedure applies to ALL security incidents that affect the 
confidentiality, integrity, or availability of organizational systems, 
data, personnel, or operations. This includes but is not limited to:

→ Unauthorized access to systems, networks, or physical facilities  
→ Malware, ransomware, or any malicious code execution  
→ Data breaches involving PII, financial data, or trade secrets  
→ Denial of service attacks impacting business operations  
→ Insider threats, whether intentional or accidental  
→ Third-party and vendor security incidents that affect our environment  
→ Physical security incidents such as tailgating, stolen devices, or badge cloning  
→ Social engineering attacks including phishing, vishing, and pretexting  

**What this does NOT cover:**

→ Routine IT helpdesk issues such as password resets or software bugs  
→ Network outages caused by hardware failure with no security component  
→ Vendor service disruptions outside our control  

**The gray area rule:** When in doubt, treat it as an incident. 
It is always better to stand down a response than to discover 
you needed one and did not initiate it.

---

## 3. Know Your Team Before You Need Them
```
INCIDENT RESPONSE TEAM STRUCTURE
─────────────────────────────────────────────────────
ROLE                    OWNS                         
─────────────────────────────────────────────────────
IR Lead                 Overall response coordination
IT Security Analyst     Technical investigation       
Project Manager         Timeline, tasks, documentation
Operations Manager      Business continuity decisions 
Legal / Compliance      Regulatory reporting          
Communications Lead     Internal and external messaging 
─────────────────────────────────────────────────────
⚠️  All team members must be reachable 24/7 during P1/P2 incidents
```

---

## 4. Incident Severity: Know It, Use It
```
────────────────────────────────────────────────────────────────
 LEVEL    SEVERITY    EXAMPLE                      RESPONSE TIME
────────────────────────────────────────────────────────────────
  P1      CRITICAL    Active breach / ransomware   IMMEDIATE    
  P2      HIGH        Malware detected / data leak  < 1 hour    
  P3      MEDIUM      Suspicious activity           < 4 hours   
  P4      LOW         Failed logins / minor anomaly < 24 hours  
────────────────────────────────────────────────────────────────
When in doubt, escalate up and not down.
```

---

## 5. Response Phases

---

### 🔵 PHASE 1: PREPARATION
*Before the incident happens*

This phase never ends. Preparation is ongoing.

**What good preparation looks like:**

IR plan tested via tabletop exercise at least twice a year; all 
staff completing security awareness training with completion tracked 
and documented; logging and monitoring active across ALL systems; 
emergency contact list updated every 90 days; backup and recovery 
systems tested monthly; and legal and regulatory notification 
requirements documented and ready before they are ever needed.

**Red flags that preparation has lapsed:**

Last tabletop exercise was over 12 months ago; staff cannot name 
the IR Lead; backups have not been tested in over 30 days.

---

### 🟡 PHASE 2: IDENTIFICATION
*Something is wrong. Figure out what.*

- [ ] Incident detected via alert, monitoring tool, or user report
- [ ] Initial triage performed within 15 minutes of detection
- [ ] Severity level assigned: P1, P2, P3, or P4
- [ ] IR Lead notified; P1 and P2 require immediate phone call, not email
- [ ] Incident ticket opened with timestamp, reporter, and initial findings
- [ ] Affected systems, users, and data assets identified
- [ ] Preserve all logs and do NOT clear or restart systems yet

**Document everything from this moment forward.**  
Time stamps, actions taken, who was notified, and what was observed.  
If it is not written down, it did not happen.

---

### 🟠 PHASE 3: CONTAINMENT
*Stop the bleeding.*

**Short-term containment (first 30 minutes):**
- [ ] Isolate affected systems and disconnect from network if necessary
- [ ] Disable compromised user accounts immediately
- [ ] Block malicious IPs, domains, or email senders
- [ ] Capture forensic image of affected systems before any changes
- [ ] Notify Operations Manager and assess business continuity impact

**Long-term containment (ongoing until eradication):**
- [ ] Implement temporary workarounds to maintain operations
- [ ] Increase monitoring across adjacent systems
- [ ] Brief leadership with facts only; no speculation
- [ ] Assess whether regulatory notification is required (see Section 7)
- [ ] Engage Legal and Compliance for P1 and P2 incidents; this is non-negotiable

---

### 🔴 PHASE 4: ERADICATION
*Kill it completely.*

- [ ] Root cause identified and fully documented
- [ ] All malware, backdoors, and unauthorized access removed
- [ ] Compromised credentials reset across ALL affected systems
- [ ] Vulnerabilities patched and verified by IT Security before proceeding
- [ ] Third-party forensics engaged for P1 incidents
- [ ] Clean bill of health confirmed before moving to recovery

**Do not rush this phase.**  
An incomplete eradication leads to reinfection, and every hour 
spent here saves days of cleanup later.

---

### 🟢 PHASE 5: RECOVERY
*Bring it back, carefully.*

- [ ] Systems restored from verified clean backups
- [ ] Restoration done in stages and not all at once
- [ ] Enhanced monitoring active for minimum 30 days post-recovery
- [ ] Users re-credentialed with MFA enforced
- [ ] Normal operations confirmed by Operations Manager
- [ ] Final stakeholder communication sent: clear, factual, and no blame

---

### ⚪ PHASE 6: LESSONS LEARNED
*The phase most teams skip. Do not.*

Post-incident review must happen within **72 hours** of closure.

**Discussion framework:**
1. What happened and when?
2. How was it detected?
3. What did we do well?
4. What slowed us down?
5. What needs to change?
6. Who owns the action items?

Output: Updated IR plan, additional training if needed, and a 
final incident report submitted to leadership within 5 business days.

---

## 6. AI Tools in Incident Response

Used carefully and deliberately:

**Claude AI:** Drafting incident reports, stakeholder communications,  
and post-incident documentation quickly and clearly

**Notion:** Real-time incident timeline tracking, task assignment,  
and team coordination during active response

**Zapier:** Pre-built automated alerts to escalate based on  
monitoring triggers before human review

**NotebookLM:** Organizing regulatory requirements, compliance  
frameworks, and legal notification thresholds

⚠️ **Critical rule:** Never paste incident details, system data,  
or PII into public AI tools during an active incident.  
Use enterprise-licensed versions only.

---

## 7. Regulatory Notification Requirements

| Regulation | Trigger | Notification Window |
|---|---|---|
| GDPR | PII of EU residents affected | 72 hours to supervisory authority |
| HIPAA | PHI breach affecting 500+ individuals | 60 days to HHS |
| PCI DSS | Cardholder data compromised | Immediately to card brands |
| State Laws | Varies by state | Typically 30 to 72 hours |

*Legal and Compliance owns this section. IR Lead coordinates.*

---

## 8. Lessons From Real Incidents

> "The number one reason incident response fails is not technical. 
> It is communication. Teams that talk clearly and frequently 
> during a crisis recover faster every single time."

Common mistakes this SOP is designed to prevent:

✗ Waiting too long to escalate  
✗ Restarting systems before capturing forensic evidence  
✗ Notifying external parties before internal leadership  
✗ Assuming containment equals eradication  
✗ Skipping the lessons learned phase  
✗ Using personal devices or unsecured channels during response  

---

## 9. Revision History

| Version | Date | Author | What Changed |
|---|---|---|---|
| 1.0 | June 2024 | Jewel Smith | Initial draft |
| 2.0 | September 2024 | Jewel Smith | Added regulatory section and AI tools |
| 2.1 | November 2024 | Jewel Smith | Revised severity framework and expanded scope |
