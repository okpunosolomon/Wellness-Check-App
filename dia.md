```mermaid
flowchart TD
    %% Define styles
    classDef user fill:#dff0d8,stroke:#3c763d,stroke-width:1px;
    classDef system fill:#d9edf7,stroke:#31708f,stroke-width:1px;
    classDef supervisor fill:#fcf8e3,stroke:#8a6d3b,stroke-width:1px;
    classDef decision fill:#f2dede,stroke:#a94442,stroke-width:1px;
    classDef end fill:#ccc,stroke:#333,stroke-width:1px;

    %% Swimlane Labels (pseudo-lanes)
    subgraph A["👩‍⚕️ Carer / Nurse"]
        A1([Start Assessment]):::user
        A2([Select Patient]):::user
        A3([Review Patient History]):::user
        A4([Conduct Wellness Check]):::user
    end

    subgraph B["⚙️ System Logic (Automated)"]
        B1([Save Record to SQL]):::system
        B2{Vitals Breach Threshold?}:::decision
        B3([Trigger Escalation Alert]):::system
        B4([No Action Required]):::system
    end

    subgraph C["🧑‍⚕️ Supervisor"]
        C1([Receive Notification via Teams/Email]):::supervisor
        C2{Approve or Reject}:::decision
        C3([Update Patient Escalation Status]):::supervisor
    end

    A1 --> A2 --> A3 --> A4 --> B1 --> B2
    B2 -- Yes --> B3 --> C1 --> C2
    C2 -- Approve --> C3 --> B4
    C2 -- Reject --> C3
    B2 -- No --> B4
    B4 --> D1([End]):::end
