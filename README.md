# MODULAR-MULTILEVEL-CONVERTER-IN-GRID-FOLLOWING-APPLICATION-+

# Modular Multilevel Converter (MMC) for Grid-Following Applications

[![License](https://img.shields.io/badge/License-CC_BY--NC--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This repository contains the design, simulation, and analysis of a **Modular Multilevel Converter (MMC)** for grid-following applications in high-voltage direct current (HVDC) systems. The project focuses on validating control strategies, energy balancing, and dynamic performance under various operational scenarios.

---

## 📖 Table of Contents
- [Project Overview](#-project-overview)
- [Key Features](#-key-features)
- [Simulation Highlights](#-simulation-highlights)
- [Repository Structure](#-repository-structure)
- [Getting Started](#-getting-started)
- [Dependencies](#-dependencies)
- [Contributors](#-contributors)
- [License](#-license)
- [References](#-references)

---

## 🚀 Project Overview
This project implements a simplified **MMC prototype** for grid-following applications, retaining core functionalities of traditional MMCs while integrating advanced control systems. Key objectives include:
- Validating energy balancing between converter arms and phases.
- Testing dynamic responses to active/reactive power injections.
- Demonstrating harmonic filtering and voltage stability.
- Simplifying MMC architecture for cost-effective implementation.

**Target Applications**: HVDC transmission, renewable energy integration, and grid stability enhancement.

---

## ✨ Key Features
1. **Simplified MMC Architecture**:
   - Single submodule per arm for reduced complexity.
   - Average Arm Model (AAM) for capacitor voltage dynamics.
   - MATLAB/Simulink-based simulations.

2. **Control Systems**:
   - **Proportional-Resonant (PR)** and **Proportional-Integral (PI)** controllers.
   - Grid-following synchronization via Phase-Locked Loop (PLL).
   - Energy balancing between upper/lower arms and phases.

3. **Mathematical Framework**:
   - Clarke, Park, and Fortescue transformations for signal decoupling.
   - Dynamic modeling of AC/DC power exchange.

4. **Performance Metrics**:
   - Active/reactive power tracking (<5% deviation).
   - Capacitor voltage ripple management.
   - Transient response analysis for step changes.

---

## 📊 Simulation Highlights
### 1. Active/Reactive Power Tracking
![Active Power Tracking](images/active_power.png)
- **Active Power (P)**: Achieved 500 MW reference with <2% steady-state error.
- **Reactive Power (Q)**: Tracked 400 MVAR reference after transient oscillations.

### 2. Capacitor Voltage Stability
![Capacitor Voltage](images/capacitor_voltage.png)
- Balanced upper/lower arm voltages under active/reactive power injections.
- Oscillations dampened within 0.5 seconds post-disturbance.

### 3. Energy Balancing
![Energy Balancing](images/energy_balance.png)
- Zero energy difference between phases/arms in steady state.
- Robust response to 1 MJ step changes (convergence within 1.5 seconds).

### 4. Grid Synchronization
- PLL-based synchronization with AC grid (50 Hz).
- Minimal harmonic distortion in output waveforms.

---

MMC_GridFollowing/
├── Simulations/ # MATLAB/Simulink models
│ ├── MMC_AverageModel.slx # Main Simulink model
│ └── Control_Modules/ # PR/PI controllers, PLL, etc.
├── Data/ # Simulation results (CSV/figures)
├── Docs/ # Project report (PDF) and references
├── Images/ # Figures for README
└── README.md

Open Simulink Models:

Launch MMC_AverageModel.slx in MATLAB R2021a or later.

Adjust parameters in System_Parameters.m for custom scenarios.

Run Simulations:

Execute Simulate_MMC.m to generate results.

Analyze outputs in Data/ using MATLAB scripts or Jupyter notebooks.

📦 Dependencies
MATLAB R2021a+ (with Simulink and Control System Toolbox)

Python 3.8+ (optional for data analysis: NumPy, Pandas, Matplotlib)

👥 Contributors
Ibrahim Okikiola Lawal - Design, Simulation, and Analysis
LinkedIn

Jaume Girona Badia - Supervision
Universitat Politècnica de Catalunya

📜 License
This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.


---

## 🛠️ Getting Started
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/MMC_GridFollowing.git

## 📂 Repository Structure
