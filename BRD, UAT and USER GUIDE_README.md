# 🩺 Wellness Check Application – BRD, UAT & User Guide  
**Client: SOL Ltd** | Consultant: **Solomon Okpuno**  

---

## 📘 1. Business Requirements Document (BRD)

### 🧩 Project Title  
**Wellness Check Application – Empowering Carers with Escalation-Ready Vitals Monitoring**

---

### 🧠 Executive Summary  
SOL Ltd sought a reliable, scalable digital solution to improve how **nurses and carers conduct patient wellness checks**, manage abnormal readings, and escalate concerns to clinical supervisors in real time.  

The **Wellness Check App**, developed on **Microsoft Power Platform**, digitises patient assessments, applies clinical thresholds, and automates the end-to-end **escalation and approval process** through **Power Automate**, **Teams**, and **Dataverse**.

This application strengthens **patient safety**, promotes **workflow efficiency**, and offers **traceable decision-making** for clinical leads.

---

### 🎯 Business Objectives

| Objective | Description | Measurable Outcome |
|-----------|-------------|--------------------|
| Digitise clinical data capture | Replace paper-based assessments with digital records | 100% digital submissions |
| Automate escalation flows | Automatically detect and escalate abnormal vitals | Supervisor alerted within 1 min |
| Improve decision cycle | Enable real-time approval via Teams or Email | Approval cycle < 10 mins |
| Maintain audit logs | Store time-stamped actions in Dataverse | Fully traceable logs |
| Support continuous improvement | Provide visibility into response metrics | Escalation reports & dashboards |

---

### 👥 Stakeholders

| Role | Name / Department | Responsibility |
|------|-------------------|----------------|
| Project Sponsor | Head of Clinical Operations | Strategic leadership & funding |
| Clinical Process Owner | Lead Nurse | Define workflows and escalation logic |
| End Users | Carers, Nurses | Conduct assessments, record data |
| Approvers | Supervisors / Matrons | Act on escalated cases |
| System Admin | IT Administrator | User roles, Power Platform governance |
| Consultant | Solomon Okpuno | Design, implement, document & train |

---

### ❌ Current Challenges

- Reliance on paper forms leading to **data loss or delays**  
- **No standard logic** for escalation thresholds  
- Supervisors frequently **miss escalations** due to email overload  
- Inability to **track decision timeframes or accountability**

---

### ✅ Proposed Solution

The proposed solution digitally transforms the process from assessment to resolution using Microsoft’s low-code ecosystem.

#### 🔧 Core Components:
- **Power Apps (Model-Driven):** Guided forms for wellness check submissions  
- **Dataverse:** Secure and scalable backend for clinical data  
- **Power Automate:** Triggers escalation logic, sends alerts  
- **Microsoft Teams/Email:** Approval or rejection in the supervisor's native channel  
- **Audit View:** Complete trail of actions taken, timestamps, and outcomes

#### 🖼️ Strategic Visualisation – Process Flow  
![Wellness Check Process Map](https://github.com/okpunosolomon/Wellness-Check-App/blob/main/visuals/Process%20Map.png?raw=true)

---

### 📦 Scope of Work

**Included (In Scope)**
- Patient profile setup and vitals recording  
- Supervisor escalation flow based on predefined thresholds  
- Email/Teams notification for escalations  
- Approval/rejection workflows  
- Action history dashboard

**Excluded (Out of Scope – Phase 2)**
- Patient diagnosis  
- External health record (EHR) integration  
- AI-based prediction or triage logic

---

### 📈 Success Criteria

- 80% decrease in missed escalations  
- 90% reduction in time-to-approval for urgent cases  
- All actions time-stamped and stored for audit purposes  
- User satisfaction score ≥ 90% post-deployment  

---

### 🛡️ Risk Assessment

| Risk | Impact | Mitigation Strategy |
|------|--------|----------------------|
| Carers forgetting to escalate | High | Embed automatic trigger logic for thresholds |
| Supervisor delay in approval | Medium | Dual-channel alert: Teams + Email |
| Permission misconfiguration | High | Role-based testing across DEV/UAT |
| Missed flow runs or outages | Medium | Alert on flow failures; retry logic enabled |

---

### ✍️ Approval Table

| Role | Name | Signature |
|------|------|-----------|
| Project Sponsor |  |  |
| Lead Nurse |  |  |
| Consultant | Solomon Okpuno | ✅ |

---

## ✅ 2. User Acceptance Testing (UAT)

### 🎯 UAT Goal  
To confirm that the application satisfies business needs, functions as intended, and performs reliably under realistic use cases.

---

### 🧪 UAT Test Matrix

| ID | Test Scenario | Steps | Expected Outcome | Status |
|----|---------------|-------|------------------|--------|
| UAT-001 | Submit patient assessment | Carer logs vitals and submits form | Form saved, system evaluates values | ✅ |
| UAT-002 | No escalation triggered | Vitals are within normal limits | System logs without notifying supervisor | ✅ |
| UAT-003 | Escalation triggered | Record abnormal BP and submit | Supervisor receives Teams + Email alert | ✅ |
| UAT-004 | Supervisor approves case | Click "Approve" from Teams | Status changes to *Approved*, logs updated | ✅ |
| UAT-005 | Supervisor rejects case | Reject via email link | Status = *Rejected*, patient monitored | ✅ |
| UAT-006 | Flow reliability | Submit during off-hours | Escalation still triggers automatically | ✅ |
| UAT-007 | Audit log accuracy | View Dataverse logs | Accurate timestamps of all actions | ✅ |
| UAT-008 | Access control | Nurse tries to access supervisor data | Access denied | ✅ |

#### 🖼️ UAT Visual Evidence – Escalation Workflow  
![Escalation Approval Flow](https://github.com/okpunosolomon/Wellness-Check-App/blob/main/visuals/Handling%20Escalation%20AprovalRejection%20Within%20Power%20Automate.png?raw=true)

---

### 📝 Final UAT Sign-Off

| Role | Name | Signature | Date |
|------|------|-----------|------|
| Sponsor |  |  |  |
| Lead Nurse |  |  |  |
| Consultant | Solomon Okpuno | ✅ |  |

---

## 👨‍🏫 3. User Guide & Training Manual

### 📌 App Title:  
**Wellness Check App – SOL Ltd**

---

### 🧭 Accessing the App

1. Go to [Power Apps](https://make.powerapps.com)  
2. Choose your SOL Ltd environment  
3. Launch **Wellness Check App** from app list  
4. Log in using your company credentials  

---

### 👥 User Roles & Permissions

| Role | Key Permissions |
|------|-----------------|
| Carer / Nurse | Create and submit patient records |
| Supervisor | Approve/reject escalations, view records |
| Admin | Configure tables, manage users, monitor logs |

---

### 🔍 Application Features

#### 1. Record a Patient Assessment  
- Navigate to **Patient Vitals → New Entry**  
- Input vitals: BP, heart rate, temperature  
- Click **Submit Assessment**

#### 2. Escalation Flow Trigger  
- If values exceed safe ranges → system sends alert  
- **Supervisor receives Teams + Email notification**

#### 3. Supervisor Actions  
- Review record and click *Approve* or *Reject*  
- Submit decision directly via Teams or within app

#### 4. Post-Decision Dashboard  
- View outcomes in **Escalation Logs**  
- Filter by date, user, outcome

---

### 🖼️ Post-Escalation View  
![Post-Approval View](https://github.com/okpunosolomon/Wellness-Check-App/blob/main/visuals/After%20Escalation%20was%20Approved.png?raw=true)

---

### 🔔 Notification Overview

| Type | Trigger |
|------|---------|
| Teams | Abnormal assessment submitted |
| Email | Escalation decision pending |
| System Log | All actions recorded in Dataverse |

---

### 🔧 Troubleshooting & Self-Service

| Issue | Suggested Fix |
|-------|---------------|
| App not launching | Verify Power Apps access and role |
| No notification received | Check flow run history and Teams permissions |
| Wrong user triggered | Validate escalation logic and OData filters |

---

### 📞 Support Contacts

- **Support Email:** [support@sol-ltd.com](mailto:support@sol-ltd.com)  
- **Emergency Escalation:** +44 20 5555 0123  
- **Consultant:** Solomon Okpuno – [GitHub](https://github.com/okpunosolomon)

---

### 🧾 Version History

| Version | Date | Summary | Author |
|---------|------|---------|--------|
| 1.0 | Dec 2025 | First Release (Full Deployment) | Solomon Okpuno |

---

> 📌 *This document consolidates all key delivery components – from business requirements and testing to user education – providing a single source of truth for the Wellness Check App implementation.*

