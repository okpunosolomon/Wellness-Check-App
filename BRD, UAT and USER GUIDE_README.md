
# 🩺 Wellness Check Application – BRD, UAT & User Guide  
**Client: SOL Ltd** | Consultant: **Solomon Okpuno**  

---

## 📘 1. Business Requirements Document (BRD)

### 🧩 Project Title  
**Wellness Check Application – Enhancing Patient Safety & Supervisor Escalation with Power Platform**

---

### 🧠 Executive Summary  
SOL Ltd identified a critical need to streamline **wellness assessments** performed by nurses and carers. The previous paper-based workflow led to **delayed escalations**, **inconsistent recording**, and **missed compliance checks**.

The **Wellness Check App**, built on Microsoft Power Platform, enables digital recording of patient vitals, **auto-triggered supervisor escalation**, and **real-time monitoring** using Power Automate, Dataverse, and Microsoft Teams/Outlook.

---

### 🎯 Business Objectives

| Objective | Description | Expected Outcome |
|----------|-------------|------------------|
| Digitise wellness assessments | Replace paper-based data collection | More accurate records |
| Automate escalations | Alert supervisors when vitals are abnormal | Faster clinical response |
| Maintain audit trails | Track actions by system, carer, supervisor | Compliance and traceability |
| Support remote approvals | Allow approvals via Teams or Outlook | Improve decision speed |
| Enable KPI tracking | Provide insights on escalation frequency | Quality and performance reviews |

---

### 👥 Stakeholders

| Role | Name / Department | Responsibility |
|------|-------------------|----------------|
| Sponsor | Head of Clinical Operations | Strategic Oversight |
| Clinical Lead | Lead Nurse / Matron | Workflow Design |
| Users | Carers & Nurses | Data entry, assessment |
| Supervisors | Team Leads | Escalation approvals |
| Consultant | Solomon Okpuno | Delivery, automation, documentation |

---

### ❌ Current Challenges

- Inconsistent recording of wellness checks  
- Delays in escalation for abnormal vitals  
- Lack of supervisor traceability  
- No audit trail or escalation logs  

---

### ✅ Proposed Solution

> A Power Platform-based application with **automated escalation flows**, real-time alerting, and full traceability.

#### 🔧 Key Components:
- **Model-Driven App:** Nurses submit wellness check forms  
- **Power Automate:** Detect abnormal thresholds → escalate  
- **Teams & Email:** Supervisors respond to alerts  
- **Dataverse:** All actions logged with timestamps  
- **Dashboards:** Track escalations and response time  

#### 🖼️ Solution Process Map  
![Wellness Check Process Map](https://github.com/okpunosolomon/Wellness-Check-App/blob/main/visuals/Process%20Map.png?raw=true)

---

### 📦 Scope

**In Scope**
- Vitals recording (temperature, BP, pulse)  
- Threshold-based escalation logic  
- Teams/email notifications  
- Supervisor approvals and rejections  
- Action audit trail

**Out of Scope**
- Patient diagnosis  
- Integration with EHR (Phase 2)

---

### 📈 Success Metrics

- 80% reduction in manual delays  
- 100% escalation traceability  
- Supervisor response time < 10 min  
- Zero missed policy breaches  

---

### 🛡️ Risk & Mitigation

| Risk | Mitigation |
|------|------------|
| Carer non-compliance | Add reminder flow logic |
| Missed escalations | Enable retry and fallback |
| Workflow errors | Pre-prod testing + alert on failure |

---

### ✍️ Sign-Off Table

| Role | Name | Signature |
|------|------|-----------|
| Project Sponsor |  |  |
| Clinical Lead |  |  |
| Consultant | Solomon Okpuno | ✅ |

---

## ✅ 2. User Acceptance Testing (UAT)

### 🎯 Purpose  
To ensure the solution aligns with business requirements before go-live.

---

### 🧪 UAT Test Scenarios

| ID | Scenario | Steps | Expected Result | Status |
|----|----------|-------|-----------------|--------|
| UAT-001 | Submit a Wellness Check | Carer records vitals | Assessment saved | ✅ |
| UAT-002 | Normal Vitals | Vitals within threshold | No escalation triggered | ✅ |
| UAT-003 | Abnormal Vitals | Carer enters critical BP | Supervisor notified | ✅ |
| UAT-004 | Supervisor Approval | Supervisor approves via Teams | Status updated in app | ✅ |
| UAT-005 | Supervisor Rejection | Supervisor rejects case | Status updated as "Rejected" | ✅ |
| UAT-006 | Notification Sync | Flow sends Teams + Email alert | Supervisor receives both | ✅ |
| UAT-007 | Dashboard Accuracy | Admin checks escalation logs | Records reflect current state | ✅ |

#### 🖼️ Power Automate Flow Snapshot  
![Escalation Approval Flow](https://github.com/okpunosolomon/Wellness-Check-App/blob/main/visuals/Handling%20Escalation%20AprovalRejection%20Within%20Power%20Automate.png?raw=true)

---

### 📝 UAT Sign-Off

| Role | Name | Signature | Date |
|------|------|-----------|------|
| Project Sponsor |  |  |  |
| Clinical Lead |  |  |  |
| Consultant | Solomon Okpuno | ✅ |  |

---

## 👨‍🏫 3. User Guide & Training Manual

### 📌 App Title:  
**Wellness Check App – SOL Ltd**

---

### 🧭 Getting Started

1. Visit [Power Apps](https://make.powerapps.com)  
2. Select **Wellness Check App** from environment  
3. Sign in with SOL Ltd Microsoft 365 credentials  

---

### 👥 User Roles

| Role | Permissions |
|------|-------------|
| Nurse/Carer | Record wellness checks |
| Supervisor | Review escalations and approve/reject |
| Admin | Review audit logs, manage user roles |

---

### 🔍 Core Features

#### 1. Submit a Patient Assessment  
- Navigate to **Assessments** → Click *New Record*  
- Fill in vital signs and patient info  
- Click *Submit*

#### 2. Supervisor Escalation Flow  
- Triggered automatically if any vitals breach defined limits  
- Supervisor notified via Teams and Email

#### 3. Approve or Reject  
- Supervisors can respond directly from Teams  
- Status is synced to the app

#### 4. View History  
- All escalation activity is logged and visible in **Escalation Logs**

---

### 🖼️ After Approval – App Visual  
![Post-Approval View](https://github.com/okpunosolomon/Wellness-Check-App/blob/main/visuals/After%20Escalation%20was%20Approved.png?raw=true)

---

### 🔔 Notifications  
Notifications sent via:
- Microsoft Teams  
- Outlook Email  
- In-App Notification (Planned)

---

### 🛠️ Troubleshooting Guide

| Issue | Resolution |
|--------|-------------|
| Approval not received | Verify supervisor Teams setup |
| Flow not triggered | Check Power Automate run history |
| Status not updating | Refresh Dataverse connection |

---

### 🤝 Support Contacts

- **Support Team:** support@sol-ltd.com  
- **Consultant Contact:** Solomon Okpuno  
- **GitHub:** [github.com/okpunosolomon](https://github.com/okpunosolomon)

---

### 🧾 Version History

| Version | Date | Summary | Author |
|---------|------|---------|--------|
| 1.0 | Dec 2025 | Initial Deployment | Solomon Okpuno |

---

> 🧩 *This documentation unifies the Wellness Check Application's requirements, testing plan, and user training into one traceable reference for both business and technical stakeholders.*

