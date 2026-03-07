# 📋 SOP-002: Logistics & Shipment Tracking Procedure

**Document Owner:** Jewel Smith, PMP  
**Classification:** ⚠️ SAMPLE TEMPLATE — For Portfolio Demonstration Only  
**Version:** 2.0  
**Last Updated:** January 2025  
**Department:** Operations & Logistics  
**Review Cycle:** Quarterly  
**Aligned With:** Supply Chain Security Framework | NIST SP 800-53

---

## 1. Purpose

Shipments getting lost, delayed, or mishandled is not just an 
operational inconvenience, it's a financial liability and a 
security risk. Sensitive goods, confidential manifests, and 
vendor contracts move through our supply chain every single day, 
and without a structured tracking process, things fall through 
the cracks fast.

This SOP exists because I've seen what happens when logistics 
runs on tribal knowledge and verbal updates. Miscommunication, 
missed deliveries, finger-pointing when things go wrong. This 
document creates ONE source of truth for how every shipment 
is handled — from the moment an order is placed to the moment 
it's signed, sealed, and closed out in the system.

The goal is simple: every shipment tracked, every exception 
documented, every stakeholder informed — automatically, 
consistently, and securely.

---

## 2. Scope

This procedure covers the full lifecycle of all inbound and 
outbound shipments processed through the Operations & Logistics 
department. This includes:

- **Domestic and international freight** — air, ground, and sea
- **High-value and time-sensitive shipments** requiring elevated monitoring
- **Vendor-managed shipments** where third-party carriers are involved
- **Returns and reverse logistics** — often overlooked but equally important
- **Cross-departmental shipments** between internal locations or warehouses

This SOP does NOT cover:

- Personal mail or non-business deliveries
- Digital or software deliveries
- Internal document transfers handled by courier services 
  under separate agreements

Any shipment that touches our supply chain and involves 
external vendors, carriers, or customers falls under this SOP. 
No exceptions.

---

## 3. Roles & Responsibilities

| Role | Responsibility | Escalation Authority |
|---|---|---|
| Logistics Coordinator | Own shipment from creation to closure | No |
| Operations Manager | Approve high-value shipments over $10K | Yes |
| IT Security | Maintain and audit tracking system access | Yes |
| Project Manager | Monitor SLA compliance and report KPIs | No |
| Vendor/Carrier | Provide real-time updates and POD | No |
| Finance | Reconcile shipping costs and invoices | No |

---

## 4. Security Considerations (CMP Framework)

Supply chain data is a high-value target. Shipment manifests, 
vendor contracts, and customer delivery information are all 
sensitive assets that require deliberate protection:

**Data Classification**
- All shipment records classified as INTERNAL — minimum
- High-value or government shipments classified as CONFIDENTIAL
- PII of recipients must be masked in shared tracking dashboards

**Access Controls**
- System access granted on strict **least privilege** basis
- Role-based access control (RBAC) enforced across all platforms
- Vendor portal access reviewed and audited every 90 days
- Terminated employees revoked within 24 hours — no exceptions

**Vendor Security**
- All third-party carriers must sign a **Data Handling Agreement**
- Vendor credentials managed through secure key management system
- Annual security assessment required for Tier 1 vendors
- Any vendor data breach must be reported to IT Security within 2 hours

**Breach Protocol**
- Any unauthorized access to shipment data treated as security incident
- Escalate immediately to IT Security and Operations Manager
- Follow SOP-003 Incident Response procedure
- Regulatory reporting assessed within 24 hours by Legal/Compliance

---

## 5. Shipment Lifecycle Procedure

### Phase 1: Order Initiation
**Trigger:** Purchase order received and approved

- [ ] Verify PO details against vendor contract
- [ ] Confirm inventory availability with warehouse
- [ ] Select carrier based on cost, timeline, and security tier
- [ ] Generate unique Shipment ID in tracking system
- [ ] Assign dedicated Logistics Coordinator
- [ ] Trigger automated stakeholder notification via Zapier
- [ ] Set SLA deadline in project management system (Notion/Jira)

**Expected Duration:** Same business day as PO approval

---

### Phase 2: Pre-Shipment Preparation
**Trigger:** Carrier confirmed and pickup scheduled

- [ ] Generate and verify all shipping documentation:
  - Bill of Lading (BOL)
  - Commercial Invoice (international only)
  - Packing List
  - Customs Declaration (if applicable)
  - Certificate of Origin (if applicable)
- [ ] Confirm packaging meets carrier and compliance standards
- [ ] Label shipment with tracking ID and handling instructions
- [ ] Upload all documents to secure shipment folder
- [ ] Confirm pickup window with carrier — get confirmation number
- [ ] Set automated tracking check-ins (every 4 hours for P1 shipments)

**Expected Duration:** 24-48 hours before pickup

---

### Phase 3: In-Transit Monitoring
**Trigger:** Carrier confirms pickup and tracking number issued

- [ ] Log tracking number and carrier contact in system immediately
- [ ] Monitor tracking updates at defined intervals:
  - P1 (Critical): Every 2 hours
  - P2 (High Value): Every 4 hours
  - P3 (Standard): Once daily
- [ ] Document every status change in shipment record
- [ ] Flag delays exceeding 2 hours from expected milestones
- [ ] Escalate critical delays to Operations Manager within 1 hour
- [ ] Communicate proactive updates to stakeholders — don't wait for them to ask
- [ ] If shipment goes dark (no updates for 6+ hours) — initiate carrier trace immediately

**Expected Duration:** Varies by shipment type and distance

---

### Phase 4: Delivery & Closure
**Trigger:** Carrier marks shipment as "Out for Delivery"

- [ ] Alert receiving party 2 hours before expected delivery
- [ ] Confirm Proof of Delivery (POD) received and signed
- [ ] Inspect delivery for damage or quantity discrepancies
- [ ] If discrepancy found — photograph, document, and escalate immediately
- [ ] Update shipment status to "Delivered" in tracking system
- [ ] Reconcile shipping costs against invoice
- [ ] Archive all documentation in secure, organized folder structure
- [ ] Close shipment ticket and send closure notification to stakeholders
- [ ] Log final KPI metrics for reporting

**Expected Duration:** Within 24 hours of delivery confirmation

---

## 6. Exception Handling

| Exception | Action | Escalation |
|---|---|---|
| Shipment delayed 2+ hours | Document and notify stakeholders | No |
| Shipment delayed 24+ hours | Initiate carrier trace, assess rerouting | Operations Manager |
| Shipment lost | File carrier claim, activate contingency plan | Operations Manager + Legal |
| Delivery damaged | Document with photos, file claim within 48 hours | Operations Manager |
| Unauthorized access to shipment | Follow SOP-003 Incident Response | IT Security immediately |

---

## 7. AI Tools Used in This Process

| Tool | Specific Use Case |
|---|---|
| Excel / Google Sheets | Live shipment tracking dashboard with conditional alerts |
| Zapier | Automated stakeholder notifications at each phase trigger |
| Claude AI | Drafting exception reports and carrier dispute letters |
| NotebookLM | Organizing carrier contracts and compliance documentation |
| Notion | Project board for managing multiple concurrent shipments |

---

## 8. Key Performance Indicators (KPIs)

| KPI | Target | Measurement Frequency |
|---|---|---|
| On-Time Delivery Rate | ≥ 95% | Weekly |
| Shipment Exception Rate | ≤ 3% | Weekly |
| Average Exception Resolution Time | ≤ 4 hours | Per incident |
| Documentation Accuracy Rate | 100% | Per shipment |
| Carrier Claim Resolution Time | ≤ 30 days | Per claim |
| Stakeholder Satisfaction Score | ≥ 4.5/5 | Monthly survey |

---

## 9. Compliance & References

- NIST SP 800-53: System & Communications Protection (SC Family)
- C-TPAT (Customs-Trade Partnership Against Terrorism) Guidelines
- Company Data Handling Agreement (Vendor Version 2.1)
- Company Supply Chain Security Policy
- GDPR Article 32 — Security of Processing (for EU shipments)

---

## 10. Document Revision History

| Version | Date | Author | Changes |
|---|---|---|---|
| 1.0 | September 2024 | Jewel Smith | Initial draft |
| 2.0 | January 2025 | Jewel Smith | Added security controls, exception handling, AI tools section |
