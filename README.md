# AERIS-TWIN

### AI-Enabled Digital Twin & Ground Control System for UAV Engine Health Monitoring

AERIS-TWIN is an AI-enabled Digital Twin platform designed for UAV piston-engine health monitoring, fault detection, and mission-aware decision support. It combines engine simulation, synthetic telemetry, ML-based analytics, and a web-based Ground Control System to visualize engine health and simulated UAV missions.

> **Development status:** Simulation-driven prototype. Real-engine validation and hardware integration are future development stages.

## Overview

AERIS-TWIN creates a virtual representation of a UAV piston engine and compares expected engine behaviour with observed telemetry. The system analyzes deviations, supports fault-related health assessment, and presents engine and mission information through an interactive dashboard.

The project uses a simulation-first approach to enable controlled testing without requiring continuous access to physical engines or test rigs.

## Key Features

- **Engine Simulation:** Generates synthetic telemetry under configurable operating conditions.
- **Digital Twin Monitoring:** Represents expected engine behaviour and compares it with observed telemetry.
- **Engine Health Dashboard:** Displays engine parameters, health trends, and status information.
- **Fault Injection:** Supports controlled abnormal scenarios for testing the monitoring pipeline.
- **ML-Based Analytics:** Provides analytical support for identifying abnormal engine behaviour.
- **Ground Control System:** Includes route visualization, mission status, flight history, and simulated flight controls.
- **Modular Architecture:** Separates simulation, telemetry, analytics, and visualization components.

## System Architecture

```
Simulated Engine Model
        ↓
Synthetic Telemetry Generation
        ↓
Data Processing & Preprocessing
        ↓
Digital Twin Core
        ↓
ML-Based Intelligence & Analytics
        ↓
Health Assessment, Fault Information & Alerts
        ↓
Ground Control System Dashboard
```

## Dashboard Modules

- Mission route visualization and progress
- Simulated flight status and controls
- Engine telemetry and health monitoring
- Expected-versus-observed parameter comparison
- Fault injection and diagnostic information
- Health trends and flight history

## Technology Stack

- **Language:** Python
- **ML:** scikit-learn
- **Simulation:** Custom engine simulation modules
- **Telemetry:** Telemetry processing and messaging components
- **Interface:** Web-based Ground Control System

## Getting Started

### Prerequisites

- Python 3.x
- pip
- Project dependencies listed in the repository's dependency file

### Installation

```bash
git clone <YOUR_REPOSITORY_URL>
cd <YOUR_REPOSITORY_FOLDER>
python -m venv .venv
```

Activate the virtual environment:

**Windows**

```powershell
.venv\Scripts\activate
```

**Linux/macOS**

```bash
source .venv/bin/activate
```

Install dependencies using the dependency file available in the repository:

```bash
pip install -r requirements.txt
```

### Running the Application

The application entry point and startup instructions depend on the current project configuration. Refer to the relevant server, simulation, and dashboard modules for the configured commands.

## Current Status & Limitations

AERIS-TWIN currently uses simulation-generated telemetry. Its outputs are intended for prototype demonstration and controlled testing. Real-world accuracy, fault-detection performance, and remaining useful life estimates have not been established through physical engine validation.

The system is not flight-certified and does not autonomously control a UAV.

## Roadmap

- [x] Simulation-driven engine monitoring prototype
- [x] Web-based Ground Control System
- [x] Synthetic telemetry and controlled fault scenarios
- [ ] Real-engine or test-rig validation
- [ ] Engine-model calibration using real telemetry
- [ ] ECU/CAN integration
- [ ] Edge-based monitoring and deployment
- [ ] Fleet-level engine-health monitoring

## Applications

- UAV piston-engine health monitoring
- Simulation-based fault analysis
- Engine telemetry visualization
- Maintenance decision support
- Digital Twin research and development

## Team

**Team Null Pointers**

Developed for **Smart India Hackathon 2026**.

## License

No license has been specified yet. Add a LICENSE file before permitting reuse or redistribution.
