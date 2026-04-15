# Inductive Charging System – Modeling, Simulation and Experimental Validation

## 1. Overview

This project investigates wireless power transfer through inductive coupling, with the goal of designing and optimizing an inductive charger.

The work combines:
- theoretical modeling
- numerical simulation (Python)
- experimental validation on a real electronic setup

---

## 2. Problem

Wireless charging systems suffer from low efficiency due to:
- weak magnetic coupling
- misalignment between coils
- energy losses (Joule effect)

The objective is to understand and optimize the efficiency of power transfer.

---

## 3. Approach

### 3.1 Theoretical Modeling

The system is modeled as two coupled coils:
- primary coil powered by an AC source
- secondary coil connected to a load

Using electromagnetic laws (Faraday, Biot-Savart), we derive:
- induced voltage
- transmitted power
- efficiency (Yates model)

---

### 3.2 Simulation

A Python model was developed to:
- compute efficiency as a function of frequency
- study the impact of system parameters (distance, geometry)

Example: simulation of Yates efficiency model.

---

### 3.3 Experimental Setup

A real circuit was built including:
- inductive coils
- resistive loads
- measurement system (Latis Pro + sysAM)

Experiments performed:
- non-resonant coupling
- resonant coupling (LC circuit)
- influence of misalignment (distance, lateral shift, angle)

---

## 4. Results

- The theoretical Yates model does not match experimental results  
- Resonant coupling significantly improves power transfer  
- Efficiency strongly depends on:
  - frequency
  - coil alignment
  - circuit parameters  

A resonance peak was observed experimentally (~5.5 kHz), not predicted by the basic model.

---

## 5. Key Learnings

- Modeling limitations in real physical systems  
- Importance of parasitic effects (capacitance, non-ideal components)  
- Design of experimental protocols  
- Data analysis and validation of models  

---

## 6. Tech Stack

- Python (NumPy, Matplotlib)
- Electronics (RLC circuits, coils, diodes)
- Measurement tools (Latis Pro, sysAM)

---

## 7. Extensions

- Battery charging via rectifier (Graetz bridge)
- Impedance matching
- Efficiency optimization

---

## 8. Repository Structure

- `/simulation` → Python models  
- `/data` → experimental measurements  
- `/figures` → plots and results  
- `/report` → full study (TIPE)

---

## 9. Author

Dimitry Popov