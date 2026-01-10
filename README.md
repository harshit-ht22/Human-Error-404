# CITY GRID MONITOR 
**From Complaint-Driven Governance to Self-Aware Cities**

##  PROBLEM STATEMENT

Urban governance in Indian cities is still largely dependent on citizen complaint platforms
to identify and resolve civic infrastructure issues such as non-functional streetlights,
overflowing garbage bins, and unhygienic public toilets.

Despite the presence of multiple applications and portals, the same problems continue
to reoccur. The core issue is not the lack of complaints, but the lack of system-level
awareness, objective verification, and enforceable accountability.

Existing systems are:
- Reactive, acting only after complaints are raised
- Manual and delayed in execution
- Subjective, relying heavily on photo-based validation
- Weak in resolution verification
- Inconsistent in enforcing accountability

As a result, governance remains complaint-heavy but system-blind.

---

## 🎯 OUR APPROACH

City Grid Monitor introduces a system-centric governance approach that treats complaints
as signals rather than absolute truth.

The platform acts as an intelligence and enforcement layer that enables cities to:
- Detect infrastructure issues automatically
- Validate complaints using data
- Prioritize issues based on risk and urgency
- Enforce time-bound action through SLAs
- Verify resolution objectively before closure

> **Complaint + Data + Rules = Enforced Action**

---

## 🏗️ SYSTEM WORKFLOW

City Grid Monitor is designed as an administrative command dashboard for city authorities.
It provides real-time visibility into infrastructure health, unresolved issues, and
accountability across departments.

The system focuses on critical public services such as:
- Street lighting
- Solid waste management
- Public sanitation infrastructure

Rather than replacing existing government platforms, the system is designed to
upgrade them by adding intelligence, verification, and enforcement.

---

## 🖥️ DASHBOARD OVERVIEW

The dashboard provides a consolidated, real-time view of the city’s operational health.
It enables administrators to quickly identify risk zones, delayed actions, and
responsibility ownership without manually reviewing individual complaints.

The dashboard is structured to support both:
- Strategic oversight
- Day-to-day administrative action

---

## 📊 KEY DASHBOARD COMPONENTS

### System Health Indicators
- **System Status:** Indicates whether monitoring and data pipelines are operational
- **Assets Online:** Shows the number of infrastructure assets connected to the system
- **Active Issues:** Displays unresolved infrastructure issues
- **SLA Breaches:** Highlights issues exceeding resolution timelines

---

### Quick Action Panel
Provides direct access to critical workflows:
- Active issues under resolution
- Escalated cases requiring immediate attention
- Issues pending verification
- SLA breach alerts

This separation ensures faster transition from awareness to action.

---

### Zone Risk Overview
The city is divided into zones based on issue severity and resolution performance:
- **Critical Zones:** Multiple unresolved or high-severity issues
- **At-Risk Zones:** Issues trending toward SLA breach
- **Stable Zones:** Minimal issues and timely resolutions

This allows proactive resource allocation and targeted intervention.

---

### Active Enforcement Cases
This section functions as an enforcement register rather than a simple issue list.

Each case clearly displays:
- Affected public asset
- Jurisdiction and risk level
- Responsible authority
- Time since issue reporting
- Current resolution or verification status

This design ensures that responsibility and delay remain visible.

---

## ⏱️ Escalation & Accountability Logic

City Grid Monitor follows a rule-based escalation mechanism:
- Issues are assigned to the relevant authority upon validation
- SLAs are automatically applied based on issue category
- If an SLA is missed, the system escalates the issue to higher authorities
- Issues are closed only after verification confirms resolution



## 🧭 Dashboard Decision Flow

```mermaid
flowchart LR
    A[Administrator Opens Dashboard] --> B[System Health Overview]
    B --> C{Any Critical Alerts?}

    C -->|Yes| D[View Escalated / High-Risk Issues]
    C -->|No| E[Monitor Zone Performance]

    D --> F[Review Issue Details]
    F --> G{SLA Breached?}

    G -->|Yes| H[Trigger Auto-Escalation]
    G -->|No| I[Continue Monitoring]

    H --> J[Assign to Higher Authority]
    J --> K[Track Resolution Status]

    K --> L[Verification Required]
    L --> M{Verified?}

    M -->|Yes| N[Issue Closed]
    M -->|No| O[Reopen & Escalate]

    E --> K
```

This prevents negligence, delays, and false closures.

---

## 🔄 END-TO-END WORKFLOW

```mermaid
flowchart TD
    A[Infrastructure Issue Occurs] --> B{Detection Source}
    B -->|Sensor| C[Sensor Detects Issue]
    B -->|Citizen Complaint| D[Citizen Submits Complaint]

    C --> E[Data Validation & Merging]
    D --> E[Data Validation & Merging]

    E --> F[Risk & Priority Assessment]
    F --> G[Automatic SLA Assignment]
    G --> H[Issue Assigned to Authority]

    H --> I{SLA Met?}
    I -->|Yes| J[Resolution Attempted]
    I -->|No| K[Auto Escalation Triggered]

    J --> L[Verification]
    K --> L[Verification]

    L --> M{Issue Resolved?}
    M -->|Yes| N[Issue Closed]
    M -->|No| O[Case Reopened & Escalated]
    O --> H
```

**This workflow ensures that no issue is resolved without objective confirmation
and that accountability is enforced systematically.**


🌐 **LIVE DEMO**

🔗 Live Dashboard:
https://city-grid-monitor.lovable.app

The current version demonstrates system behavior using simulated data
to reflect real-world workflows and escalation logic.

---

##🔮**ROUND-2 IMPLEMENTATION PLAN**


In Round-2, the project will focus on strengthening system realism
and governance feasibility through deeper software implementation.

*Planned enhancements include:*
- Integration of a lightweight backend to enable real-time issue creation,
  SLA timers, and escalation transitions
- Use of simulated but realistic data streams to represent infrastructure
  signals and citizen inputs
- Live demonstration of automatic escalation when SLA thresholds are crossed
- Enforcement of verification logic to prevent premature issue closure
- End-to-end execution of governance workflows on the live dashboard

-The emphasis in Round-2 is on validating accountability mechanisms
and decision-making logic rather than physical hardware deployment.

-While hardware integration is feasible, the current phase prioritizes
governance logic and system enforcement, which are independent of
specific sensing technologies.


---

##🧪 **Round-1 Scope:**


For Round-1, the project focuses on demonstrating system thinking,
governance workflows, and feasibility through a functional prototype.

*The scope of this round includes:*
- A live administrative dashboard representing city system health
- Simulated data to demonstrate issue creation, SLA tracking, and escalation
- End-to-end workflow visualization from detection to resolution
- Clear articulation of escalation and verification logic
- Architecture and diagrams explaining system behavior

The emphasis in Round-1 is on clarity, originality, and feasibility,
rather than full-scale deployment.


---

## 🚀 Round-2 Implementation (Completed)

### Objective
Strengthen system realism and governance feasibility through deeper software execution.

### Implemented in Round-2

#### ✅ Backend Integration
- Node.js + Express based backend implementation
- REST APIs for:
  - Issue creation
  - Verification
  - Resolution updates

#### ✅ SLA Timers & Escalation Logic
- Time-based SLA breach detection
- Automatic escalation when SLA thresholds are crossed
- Clear authority-level transitions

#### ✅ Verification Enforcement
- Issues cannot be marked as resolved without verification
- Prevents false or premature closure of complaints

#### ✅ End-to-End Live Workflow
- Government dashboard connected to backend APIs
- Real-time state updates on verification and resolution

#### ✅ Citizen Transparency Layer
- Separate citizen-facing dashboard
- Public visibility of only **verified** resolutions

> **Note:**  
> Hardware integration was intentionally deferred in this phase to prioritize governance logic and system enforcement, which are independent of specific sensing technologies.

---

### 🧱 **System Design Documentation**

The repository includes / will include the following system design artifacts:

- High-Level System Architecture Diagram
- Data Flow Diagrams (DFDs)
- Logical Database Schema
- SLA & escalation rule mapping
  
  ## *High-Level System Architecture*
```mermaid
flowchart LR
    Citizen[Citizen Interface] -->|Issue View / Status Check| Frontend
    Authority[Government Authority] -->|Monitoring & Actions| Frontend

    Frontend -->|REST API Requests| Backend

    Backend -->|Issue Data| Database[(Issue Store)]
    Backend -->|SLA Rules| SLAEngine[SLA & Escalation Engine]

    SLAEngine -->|Escalation Trigger| Backend
    Backend -->|Verified Issues| Frontend
```
#### *“This shows how UI, backend, SLA engine, and data layer interact.”*

---

## *End-to-End Governance Workflow (DFD)*
```mermaid
flowchart TD
    A[Issue Occurs / Complaint Raised]
    B[Validation & De-duplication]
    C[Risk & Priority Assessment]
    D[SLA Assignment]
    E[Authority Action]
    F[Verification Step]
    G[Issue Resolved]
    H[Auto Escalation]

    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
    F -->|Verified| G
    F -->|Not Verified / SLA Breach| H
    H --> E
```
# *“No issue can reach resolution without verification.”*

---

## *SLA & Escalation Logic*
```mermaid
flowchart LR
    Low[Low Risk Issue] -->|48 hrs SLA| L1[Local Authority]
    Medium[Medium Risk Issue] -->|24 hrs SLA| L1
    High[High Risk Issue] -->|12 hrs SLA| L2[Zonal Authority]
    Critical[Critical Issue] -->|4 hrs SLA| L3[City Authority]

    L1 -->|SLA Breach| L2
    L2 -->|SLA Breach| L3
```
# *“Escalation is automatic, not dependent on manual follow-ups.”*

---

## *Database Schema*
```mermaid
erDiagram
    ISSUE {
        string issueId
        string publicAsset
        string zone
        string jurisdiction
        string riskLevel
        int slaMinutes
        int timeSinceMinutes
        string resolutionStatus
        boolean verified
        string responsibleAuthority
    }

    AUTHORITY {
        string authorityId
        string department
        string level
    }

    ISSUE }o--|| AUTHORITY : assigned_to
```
# *“The schema tracks issue lifecycle and authority ownership.”*
---

## *Citizen Transparency Flow*
```mermaid
flowchart LR
    VerifiedIssue[Verified Issue]
    Publish[Publish to Citizen Dashboard]
    CitizenView[Citizen Views Status]

    VerifiedIssue --> Publish
    Publish --> CitizenView
```
# *“Only verified resolutions are visible to citizens.”*

---

> Diagrams are added separately as images for clarity.

---

## 📈 Scalability & Future Growth

The system is designed to scale through:

- Modular backend services
- Zone-based data partitioning
- Rule-driven enforcement engine
- Seamless integration with existing government platforms

### Planned Extensions
- Real sensor integration
- Predictive failure analytics
- Department-specific dashboards
- Government SSO authentication

---

## 🤖 AI Usage Declaration

AI tools (such as Lovable and LLMs) were used **only for repetitive or basic UI scaffolding tasks**.

All **decision-making logic, SLA rules, escalation mechanisms, verification workflows, and system architecture** were **manually designed and implemented**.

No autonomous or decision-making agents were used.

---

## 🏆 Conclusion

**City Grid Monitor transforms civic governance** from reactive complaint handling to a **proactive, system-aware, and accountable model**.

By making **risk, delay, and responsibility visible**, the platform enables:

- Faster intervention
- Better resource utilization
- Stronger administrative accountability
- Increased citizen trust

---


## 👥 **Team Information**

*Team Name:* Human Error 404

*College:* GLA University, Greater Noida

*Hackathon:* Hack The Winter – The Second Wave

*Theme:* Governance

**Team Members**

Yashashvi Jadoan

Harshit Thakur (Team Leader)

Priyanshu Singh

Anvesha Sharma
