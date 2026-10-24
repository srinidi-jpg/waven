# 🌊 HydroX — Flood Intelligence Platform

### 🚨 From Reservoir Signals to Downstream Safety

**Built by Team HydroX | HackBuild'26**

An AI-assisted flood intelligence and early-warning decision-support platform designed to help identify potential downstream risks, visualise affected areas, and prepare clearer, location-relevant safety guidance.

HydroX brings rainfall and reservoir information into one workflow, helping authorised officials review risk indicators and prepare warning messages before conditions become critical.

> **Safety first:** HydroX is a decision-support prototype. It does not control dam gates, replace official emergency authorities, or send real emergency alerts without authorised integrations.

**Python · FastAPI · React · TypeScript · Tailwind CSS · Recharts · React Leaflet · OpenStreetMap**

---

## 📖 Table of Contents

- 💡 [The Big Idea](#-the-big-idea)
- 😟 [The Problem](#-the-problem)
- ✨ [Our Solution](#-our-solution)
- 🎬 [See It in Action](#-see-it-in-action)
- 🏗️ [How It Works](#️-how-it-works)
- 🧭 [Workflow Architecture](#-workflow-architecture)
- 🛠️ [Tools and Technologies](#️-tools-and-technologies)
- 📚 [Concepts Explained Simply](#-concepts-explained-simply)
- 🆚 [Why HydroX Is Different](#-why-hydrox-is-different)
- 🚀 [Getting Started](#-getting-started)
- 🗺️ [Roadmap](#️-roadmap)
- 👥 [Team](#-team)

---

## 💡 The Big Idea

Imagine heavy rainfall is approaching a reservoir. Water levels may be rising, and downstream communities could need to prepare.

Different pieces of information may be available through different sources, leaving an important question:

**Which downstream locations need attention first, and what information should residents receive?**

HydroX aims to bring these signals together in one dashboard.

Instead of making users interpret scattered readings manually, HydroX provides a connected workflow:

- 🌧️ Review rainfall and reservoir information.
- ✅ Validate available data and identify missing or stale information.
- ⚠️ Display an explainable risk band.
- 🗺️ Visualise downstream locations and potential exposure.
- 📝 Prepare safety-message drafts for authorised officer review.
- 📋 Maintain a traceable record of alert-review activity.

The goal is to make flood preparedness information easier to understand and decisions easier to review.

---

## 😟 The Problem

Flood-related risks can change quickly during heavy rainfall and reservoir operations. Residents, farmers, commuters, responders, and local officials need understandable and timely information to prepare.

### 🌧️ Who faces this problem?

| Users                    | Challenge                                                         |
| ------------------------ | ----------------------------------------------------------------- |
| 🏠 Downstream households | May not know whether local conditions require preparedness action |
| 🌾 Farmers               | Need understandable updates relevant to their locations           |
| 🚗 Commuters             | Need information about potential flood-related disruption         |
| 🚑 Emergency responders  | Need a clearer view of locations requiring attention              |
| 🏛️ Local authorities    | Need to review multiple indicators and communicate guidance       |

### 😬 Why existing information can be difficult to use

- Weather forecasts provide rainfall information, but rainfall alone does not establish the impact of a reservoir release.
- Reservoir observations, official release information, and local preparedness guidance may be available through separate channels.
- General warnings may not explain which downstream locations require closer attention.
- Missing, delayed, or uncertain data can make risk interpretation more difficult.

Official warnings remain essential. HydroX is intended to support their review and communication, not replace them.

### 🎯 Example use case

Heavy rainfall is forecast and reservoir levels are rising.

An authorised official needs to assess the available information, identify downstream locations that should be checked first, and prepare understandable guidance for affected communities.

**HydroX aims to support that workflow through a shared, explainable dashboard.**

---

## ✨ Our Solution

HydroX is a flood intelligence and early-warning decision-support platform that connects available data, risk assessment, downstream visualisation, and alert review in one workflow.

### 1️⃣ Explainable Risk Bands

HydroX uses a rule-based approach to classify illustrative scenarios into three risk bands:

- 🟢 **Watch** — conditions require monitoring.
- 🟠 **Warning** — increased attention and preparedness may be needed.
- 🔴 **Alert** — the configured scenario indicates a higher level of concern.

These labels are illustrative prototype categories, not official emergency declarations. Real-world thresholds must be validated and approved by relevant authorities.

### 2️⃣ Downstream Map View

🗺️ A map-based interface helps users visualise relevant downstream locations and understand where additional assessment may be needed.

The reliability of any exposure view depends on accurate geographic information, verified downstream connections, and suitable data sources.

### 3️⃣ Staged Alert Preparation

📝 HydroX prepares simple, location-relevant warning drafts that an authorised officer can review, edit, and approve.

The prototype demonstrates the alert-review workflow rather than independently issuing real-world emergency notifications.

### 4️⃣ Data Visualisation

📊 Rainfall and reservoir charts help users inspect available information in a shared dashboard instead of relying entirely on separate readings.

### 5️⃣ Safety and Transparency

🔐 HydroX is designed around explainable rules, data-quality checks, clear sample-data labelling, and human oversight.

The system is intended to assist decision-making, not autonomously control reservoir operations.

---

## 🎬 See It in Action

### 🧪 Illustrative demonstration scenario

Consider a demonstration in which rainfall increases and reservoir observations indicate changing conditions.

| Step | What happens                                                   |
| ---- | -------------------------------------------------------------- |
| 1️⃣  | The user loads the available demonstration data                |
| 2️⃣  | The dashboard displays rainfall and reservoir information      |
| 3️⃣  | The risk engine evaluates the configured scenario              |
| 4️⃣  | HydroX displays the corresponding illustrative risk band       |
| 5️⃣  | The user reviews the downstream map                            |
| 6️⃣  | The system prepares a warning draft                            |
| 7️⃣  | An authorised user reviews and approves the draft in demo mode |

### 🏁 Demonstration outcome

The demonstration shows how data visualisation, explainable risk rules, map-based context, and officer review can be connected into a single workflow.

**Important:** Sample scenarios demonstrate the concept. They must not be interpreted as live flood predictions or official warnings.

### 🔗 Project Repository

[View the HydroX project repository on GitHub](https://github.com/srinidi-jpg/waven.git)

---

## 🏗️ How It Works

HydroX follows a structured workflow from data input to alert review.

```text
         🌧️ Rainfall Data
                +
         🌊 Reservoir Data
                │
                ▼
       ✅ Data Validation
                │
                ▼
       ⚠️ Rule-Based Risk Engine
                │
                ▼
        🗺️ Downstream Map
                │
                ▼
        📝 Alert Drafting
                │
                ▼
       👤 Officer Review
                │
                ▼
        📋 Alert Review Log
```

### 🧩 What each stage does

| Stage             | Responsibility                                                 |
| ----------------- | -------------------------------------------------------------- |
| 🌧️ Data Inputs   | Collects or loads available rainfall and reservoir information |
| ✅ Validation      | Checks data quality, timestamps, and availability              |
| ⚠️ Risk Engine    | Applies configured rules to assign an illustrative risk band   |
| 🗺️ Map View      | Presents relevant downstream geographic information            |
| 📝 Alert Drafting | Prepares understandable warning-message drafts                 |
| 👤 Officer Review | Allows authorised personnel to review and approve drafts       |
| 📋 Alert Log      | Supports traceability of alert-review activity                 |

Actual functionality depends on the connected data sources and implemented prototype features.

### 🔐 Safety principles

- **Human oversight:** warning drafts are intended for authorised review.
- **Data transparency:** sample data must be clearly distinguished from verified live data.
- **Explainable decisions:** risk classifications should be linked to the rules and inputs that triggered them.
- **Responsible integration:** live data feeds and operational thresholds require appropriate verification and approval.
- **No gate control:** HydroX does not operate reservoir gates.

---

## 🧭 Workflow Architecture

HydroX can be understood through three main phases.

### 📥 Phase 1 — Data Input and Validation

Available rainfall and reservoir data are loaded and checked before risk assessment.

The prototype can use sample CSV/JSON data for demonstration. Live integration requires compatible and verified data sources.

### 🧮 Phase 2 — Risk Assessment and Visualisation

A rule-based risk engine evaluates the configured inputs and produces an illustrative risk band. Charts and the downstream map help users interpret the scenario.

The system should communicate uncertainty and avoid treating incomplete data as definitive evidence of safety.

### 🚨 Phase 3 — Alert Review and Logging

HydroX prepares a warning draft for review. An authorised officer can inspect and approve the draft within the demonstrated workflow.

Live notification delivery, official approval workflows, and operational audit requirements depend on future integrations.

---

## 🛠️ Tools and Technologies

| Technology        | Purpose                                          |
| ----------------- | ------------------------------------------------ |
| 🐍 Python         | Backend development and risk-rule implementation |
| ⚡ FastAPI         | Backend API framework                            |
| ⚛️ React          | Interactive frontend interface                   |
| 📘 TypeScript     | Typed frontend development                       |
| 🎨 Tailwind CSS   | Interface styling                                |
| 📊 Recharts       | Rainfall, reservoir, and dashboard charts        |
| 🗺️ React Leaflet | Interactive map interface                        |
| 🌍 OpenStreetMap  | Map data and geographic visualisation            |
| 📄 CSV / JSON     | Demonstration data formats                       |

### 🧠 Why this stack?

- **Python and FastAPI** provide a practical foundation for implementing risk rules and exposing backend endpoints.
- **React and TypeScript** support an interactive dashboard with reusable components.
- **Recharts** helps present time-series and other numerical information visually.
- **React Leaflet and OpenStreetMap** support geographic visualisation.
- **CSV and JSON** make it possible to demonstrate the workflow without requiring paid live-data APIs.

These technologies describe the project's intended stack; the exact implementation and configuration should be confirmed against the repository.

---

## 📚 Concepts Explained Simply

### 🌧️ Rainfall Monitoring

Rainfall measurements help users understand precipitation over a selected period. Rainfall alone cannot determine whether a particular location will flood.

### 🌊 Reservoir Observations

Reservoir information can provide context about changing water conditions. Accurate assessment also depends on other factors, including authorised release information, inflow, downstream conditions, and verified operational data.

### ⚠️ Rule-Based Risk Assessment

A rule-based engine applies predefined conditions to input data. Unlike an unexplained prediction, a well-designed rule system can show which configured conditions triggered a risk classification.

### 🗺️ Downstream Exposure Mapping

A map helps users understand geographic context. Reliable exposure assessment requires verified downstream pathways, terrain and geographic information, and suitable hazard data.

### 👤 Human-in-the-Loop Decision Support

The system prepares information, while authorised people retain responsibility for reviewing and approving operational communications.

### 📋 Auditability

A traceable record can help reviewers understand what information was available, which rules were applied, and what action was taken. The scope of logging depends on the implementation.

---

## 🆚 Why HydroX Is Different

HydroX focuses on connecting several steps that may otherwise be handled separately.

| Dimension           | Disconnected information workflow          | HydroX approach                                             |
| ------------------- | ------------------------------------------ | ----------------------------------------------------------- |
| Data interpretation | Users may need to inspect separate sources | Shared dashboard for available inputs                       |
| Risk assessment     | May require manual interpretation          | Explainable, configured rule-based risk bands               |
| Geographic context  | May be separated from readings             | Downstream map view                                         |
| Warning preparation | May require separate drafting steps        | Staged warning-draft workflow                               |
| Human oversight     | Depends on the existing process            | Officer review is part of the intended workflow             |
| Transparency        | Can vary between tools                     | Designed to connect inputs, risk rules, and review activity |

### 🌟 Our core differentiator

**HydroX connects data validation → explainable risk assessment → downstream visualisation → officer-reviewed alert preparation.**

The project is not simply a weather dashboard. Its focus is on turning available information into a structured workflow for flood preparedness and human decision support.

This is the intended differentiation; comparative performance and real-world effectiveness would need to be evaluated through testing and an approved pilot.

---

## 🚀 Getting Started

### 📋 Prerequisites

Depending on the repository's current configuration, you may need:

- Node.js and npm for the React frontend.
- Python for the FastAPI backend.
- Git to clone the repository.
- A supported browser to view the dashboard.

### 1️⃣ Clone the repository

```bash
git clone https://github.com/srinidi-jpg/waven.git
cd waven
```

### 2️⃣ Install frontend dependencies

Run these commands from the directory containing the frontend's `package.json` file:

```bash
npm install
```

### 3️⃣ Start the frontend

```bash
npm run dev
```

Use the local URL printed by the development server to open the dashboard.

### 4️⃣ Set up the backend

If the backend includes a `requirements.txt` file, create and activate a Python virtual environment, then install its dependencies.

```bash
python -m venv .venv
```

Windows:

```bash
.venv\Scripts\activate
```

macOS/Linux:

```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Start the FastAPI application using the actual Python module and application variable configured in your repository. For example, if the entry point is `main.py` and the application variable is `app`:

```bash
uvicorn main:app --reload
```

**Setup note:** The repository's exact folder structure, scripts, backend entry point, environment variables, and dependency files have not been verified here. Adjust these commands to match the actual project. The frontend and backend may require separate terminals.

### 5️⃣ Run the demonstration

Once the required components are running:

1. Open the HydroX dashboard.
2. Load the supported sample dataset.
3. Review rainfall and reservoir charts.
4. Inspect the illustrative risk band.
5. Explore the downstream map.
6. Review the generated warning draft.
7. Test the officer-review workflow in demo mode.

Use only the sample or verified data sources configured for the prototype. Do not rely on the demonstration for real-world emergency decisions.

---

## 🗺️ Roadmap

### ✅ Prototype Focus

- Dashboard for available rainfall and reservoir information.
- Illustrative rule-based risk bands.
- Downstream map visualisation.
- Warning-draft review workflow.
- Demonstration using sample data.

### 🔜 Planned Improvements

**Phase 1 — Validation**

- Verify risk thresholds with relevant domain experts.
- Test the rules against suitable historical events.
- Improve handling of missing, stale, and uncertain data.

**Phase 2 — Approved Data Integration**

- Connect to verified rainfall, reservoir, and authorised release data sources.
- Validate timestamps, data quality, and update frequency.
- Evaluate the system with relevant stakeholders.

**Phase 3 — Community Communication**

- Explore authorised SMS or other notification integrations.
- Improve English and Tamil usability.
- Test whether messages are understandable and relevant to different communities.

**Phase 4 — Scalability**

- Explore support for multiple reservoirs and downstream regions.
- Strengthen access control, auditability, and operational monitoring.
- Evaluate the system through a controlled pilot with appropriate public-sector or NGO partners.

These are proposed improvements, not claims that the features are already operational.

---

## 👥 Team HydroX

Built for **HackBuild'26 — Climate Resilience Track**.

- **S. Krishitha — CSE A**
- **J. S. Srinidi** — CSE E
- **M. Suriya** — CSE E

### 🌊 Our Vision

**Clearer signals. Faster review. Safer preparation.**

HydroX aims to make flood-related information easier to interpret and help communities and authorities prepare through better-informed, human-reviewed decisions.

---

## ⚠️ Disclaimer

HydroX is a prototype intended for demonstration and decision-support research. Risk bands and sample scenarios are illustrative and must not be treated as official forecasts, evacuation orders, or emergency warnings.

The platform does not control dams or reservoir gates. Any real-world deployment would require verified data sources, expert-validated thresholds, appropriate security and reliability testing, and authorisation from the responsible agencies.

In an actual emergency, follow instructions from official authorities.

---

*Made with 🌊 by Team HydroX for a more prepared and resilient future.*

