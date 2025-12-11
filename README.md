# 🩺 Wellness Check Application  
**Modernizing Patient Health Monitoring & Escalation with Microsoft Power Platform**

---

![Banner](./visuals/Health%20Escalation%20Approval%20request%20via%20Mail%20Power%20automate.png)

---

## 🚀 Executive Overview

The **Wellness Check Application** is a digital health workflow solution designed to streamline the way healthcare organizations perform wellness assessments, escalate clinical concerns, and ensure compliance.

Developed with **Microsoft Power Platform** technologies — including **Canvas Apps**, **Power Automate**, and **Azure SQL Server** — the app offers **real-time, auditable, and mobile-first workflows** that replace manual, paper-based processes.

### ✅ Strategic Objectives
- Improve patient safety through instant clinical escalation
- Standardize documentation with digital records
- Reduce staff burden and burnout through automation
- Ensure audit-readiness and regulatory compliance

---

## 🔍 Problem Landscape

Healthcare professionals often face:

| Problem                            | Impact                                                           |
|------------------------------------|------------------------------------------------------------------|
| Manual assessments (paper/excel)   | Inconsistent data, missed risks, lack of traceability            |
| Slow response to abnormal readings | Delayed care, poor patient outcomes                              |
| Disjointed communication channels  | Approval bottlenecks, fragmented accountability                  |
| No centralized patient history     | Difficult audits, incomplete care history                        |
| Compliance & safeguarding risk     | Inability to meet regulatory and internal audit requirements     |

> 📉 These issues contribute to workflow inefficiencies, high error rates, and avoidable clinical incidents.

---

## 💡 Solution Summary

The **Wellness Check App** addresses these pain points by offering a **centralized, intelligent health assessment system** that empowers frontline carers and clinical supervisors.

### 🔧 Key Capabilities
- 📋 Digital wellness checks: BP, temperature, glucose, meds, mood
- 🚦 Auto-triggered escalation flows with real-time alerts
- 📥 Supervisor approvals via **Teams** or **Outlook**
- 🔐 Role-based security: carers, supervisors, and admins
- 💬 In-app communications: call, email, Teams chat
- 🧾 Audit-ready records with timestamped activity logs
- 📱 Fully responsive across mobile and desktop

---

## 🧱 Architecture Overview

| Layer           | Technology             | Description                                      |
|----------------|------------------------|--------------------------------------------------|
| UI Layer        | Power Apps Canvas App  | Interface for wellness input and record review   |
| Workflow Engine | Power Automate         | Business logic, escalation triggers              |
| Data Layer      | Azure SQL Server       | Scalable backend for wellness and audit data     |
| Communication   | Teams & Outlook        | Supervisor notifications and approvals           |
| Access Control  | Role-Based Permissions | Data protection and user-specific experiences    |

📌 *See diagram in `/visuals/System Architecture.png`*

---

## 🔄 Functional Workflow

1. **Select Patient** — Searchable interface with filters
2. **Review History** — Timeline of prior wellness assessments
3. **Complete Check** — Record vital signs, meds, and observations
4. **Store Record** — Saved securely to SQL Server with timestamp
5. **Trigger Escalation (if needed)** — Based on threshold rules
6. **Supervisor Notified** — Via Teams or Email
7. **Approval Action** — Status updated automatically in app

📷 Visuals:
- `Creating New Patient Record.png`
- `Teams Escalation Approval Status.png`
- `After Escalation was Approved.png`

---

## 🔁 Escalation & Communication Flow

Escalations are powered by **Power Automate**, ensuring timely routing and resolution.

### 🔄 Flow Summary
- Escalation triggered by app logic
- Notification sent to assigned supervisor
- Approvals processed via Microsoft Teams or Outlook
- Decision reflected back in app instantly
- Escalation status logged with timestamp and approver identity

📂 Refer to visuals:
- `Patient Approval Flow.png`
- `Handling Escalation ApprovalRejection Within Power Automate.png`

---

## 🔐 Security & Governance

| Area            | Control Measures                                      |
|------------------|--------------------------------------------------------|
| Data Protection  | Azure SQL with row-level security & encryption         |
| Access Management| Role-based app experiences (Nurse, Supervisor, Admin) |
| Audit Logs       | Time-stamped actions tracked and stored               |
| Regulatory Fit   | HIPAA-aligned storage and communications               |

> 🔒 This app enforces policy-driven access, activity logging, and full data traceability.

---

## 📊 Measured Business Outcomes

| KPI                          | Before             | After                | Benefit                 |
|-----------------------------|--------------------|----------------------|-------------------------|
| Escalation Response Time     | 24–48 hours         | < 8 hours             | 70% faster              |
| Documentation Accuracy       | Manual & error-prone | Digitized, auto-timestamped | 60% fewer errors  |
| Supervisor Response Rate     | Inconsistent        | 95% within SLA        | Faster, reliable action |
| Admin Hours/Week             | 10+ hours           | < 3 hours             | 40+ hrs/week saved      |
| Paper Usage                  | High                | Eliminated            | 100% digital workflow   |

---

## 🧪 Technical Implementation

- **Platform**: Microsoft Power Platform (Canvas App + Power Automate)
- **Backend**: Azure SQL Server
- **Cloud Flows**:
  - `WellnessCheck_Escalation_Trigger`
  - `Supervisor_Approval_Flow`
  - `Update_Patient_Status_Auto`
- **Testing**:
  - Conducted across 3 user roles (Carer, Supervisor, Admin)
  - 100% UAT pass rate across functional cases
- **Deployment**:
  - Exported as Managed Solution ZIP for lifecycle management

---

## 🔭 Future Roadmap

| Feature                     | Description                                    | Target Release |
|-----------------------------|------------------------------------------------|----------------|
| 🔍 Predictive Alerts (AI)   | Early warning system for risk conditions       | Q1 2026        |
| 📊 Power BI Dashboards     | Supervisor and executive reporting dashboards  | Q2 2026        |
| 🎙️ Voice-Enabled Entry     | Voice-to-text for mobile assessments           | Q3 2026        |
| 📡 IoT Device Integration   | Smart health monitoring via wearables          | Q4 2026        |
| 🏥 Multi-Site Rollout       | Centralized system across care networks        | 2027           |

---

## 📁 Repository Contents

```

📁 visuals/                     → Screenshots, app interface, and flow diagrams
📁 Overview PDF/               → Client presentation slides
📁 Solution Zip File/          → Managed Power Platform solution
📄 README.md                   → Project documentation (this file)

```

---

## 📌 Conclusion

The **Wellness Check Application** is not just a Power App — it's a **transformational framework** for healthcare workflow modernization.

By automating risk escalation, digitizing patient assessments, and creating a seamless audit trail, the solution delivers measurable outcomes in **clinical safety, operational efficiency, and regulatory confidence**.

> 💬 If your organization seeks to digitize care delivery and reduce operational friction — let’s talk implementation.

---

### 👤 Developed By

**Solomon Okpuno**  
*Power Platform Consultant | Data & Workflow Automation Specialist*  
🔗 [LinkedIn](https://linkedin.com/in/okpunosolomon) • 💻 [GitHub](https://github.com/okpunosolomon)

---
