```mermaid
flowchart TD

%% 👩‍⚕️ Carer / Nurse
    A1([Start Assessment])
    A2([Select Patient])
    A3([Review Patient History])
    A4([Conduct Wellness Check])

%% ⚙️ System Logic (Automated)
    B1([Save Record to SQL])
    B2{Vitals Breach Threshold?}
    B3([Trigger Escalation Alert])
    B4([No Action Required])

%% 🧑‍⚕️ Supervisor
    C1([Receive Notification via Teams/Email])
    C2{Approve or Reject}
    C3([Update Patient Escalation Status])

%% 🛑 End
    D1([End])

%% Flow Connections
    A1 --> A2 --> A3 --> A4 --> B1 --> B2
    B2 -- Yes --> B3 --> C1 --> C2
    C2 -- Approve --> C3 --> B4
    C2 -- Reject --> C3
    B2 -- No --> B4
    B4 --> D1
