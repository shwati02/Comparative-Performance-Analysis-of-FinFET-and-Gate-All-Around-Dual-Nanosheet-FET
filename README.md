# Synopsis Sentaurus TCAD Simulations – FinFET vs GAAFET
Coursework part of the ELEC70003 Advanced Electronic Devices Spring 2026 

This repository contains all **Sentaurus Device (sdevice)** and **Sentaurus Structure Editor (sde)** files used for simulating and analysing advanced transistor architectures.

## Overview

The project focuses on a comparative study between:
- FinFET (rectangular and rounded fin)
- Dual nanosheet Gate-All-Around FET (GAAFET)

Simulations were carried out using **Synopsys Sentaurus TCAD** to evaluate DC performance and electrostatic control at nanoscale dimensions.

## Contents

- `*.sde` – Device structure definitions (geometry, doping, meshing)
- `*.sdevice` – Simulation setup and physics models
- `*.csv` – Output result files
- MATLAB code for parameter extraction



## Results Summary
Transitioning from FinFET to GAAFET enables dramatically improved short-channel control, reduced leakage, and near-ideal switching behaviour, making GAAFETs more suitable for advanced, low-power nanoscale technologies.
The comparative analysis highlights clear performance differences between FinFET structures and the dual nanosheet GAAFET.

- **Fin corner rounding degrades electrostatic performance**:
  - Transconductance reduced (~4.82 → 3.01 µS in linear region)
  - DIBL worsens significantly (106.6 → 187.6 mV/V)
  - Ion/Ioff drops by ~1 order of magnitude (10⁵ → 10⁴)

- **Rectangular FinFET outperforms rounded FinFET**:
  - Higher drive current (Ion ≈ 21.04 µA vs 16.83 µA)
  - Lower leakage (Ioff ≈ 1.99×10⁻¹⁰ A vs 1.70×10⁻⁹ A)
  - Better overall switching behaviour

- **GAAFET demonstrates superior electrostatic control**:
  - Near-ideal subthreshold swing (~60.13 mV/dec)
  - Very low DIBL (~28.4 mV/V vs >100 mV/V for FinFETs)
  - Extremely low leakage (Ioff ≈ 2.24×10⁻¹⁵ A)
  - Ion/Ioff ≈ 1.08×10¹⁰ (vs 10³–10⁵ for FinFETs)
  - Higher transconductance (gm,lin ≈ 10.50 µS)

