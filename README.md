# CIV Bridge

## 🏗️ Project Overview

The CIV102 bridge contest is a cherished EngSci tradition that challenges first-year students to apply fundamental civil engineering principles to design and build a **box girder bridge** using matboard and contact cement. Our goal was to maximize strength-to-weight ratio and withstand the highest possible load under realistic failure constraints.

> 🏆 **Our bridge supported over 1000N (1kN) — the highest among 300+ competing students.**

## 🧱 Tools
- **Software**: MATLAB 
- **Construction tools**: Matboard, contact cement, Opticutter, Exacto knife
- **Testing**: Manual weight loading on a hydraulic rig (performed by course staff)

## ⚙️ Design and Analysis

We began our process by writing a MATLAB script to generate Shear Force Diagrams (SFD) and Bending Moment Diagrams (BMD) under a simulated train loading scenario. Our workflow included:
- Verifying code output with hand calculations
- Iterating on design parameters (geometry, material layout) based on failure modes
- Using Opticutter (online tool) to determine precise cuts for matboard assembly
- Constructing the bridge using contact cement and curing for 3 days before testing

We computed **Factors of Safety (FOS)** against:
- Tension and compression
- Shear and glue shear
- Buckling in the top flange and web (both flexural and shear)
> 📄 Read the full [design report](https://docs.google.com/document/d/1NyjHP5j28R9uciNkeaLgJFvNh0XSbSl3FdUJxr8d7a8/edit?usp=sharing)

## 🧪 MATLAB Code
This repo includes:
- Parametric simulation of bridge under various load positions
- Evaluation of maximum internal forces (shear, bending)
- Sectional stress analysis and buckling prediction
- FOS plots and visualization for critical failure points

### Main script highlights:
- Discretized the bridge into 1 mm segments
- Evaluated worst-case stress scenarios from all train positions
- Calculated FOS for all key material and geometric constraints
- Plotted envelopes for SFD/BMD and failure loads (Vfail/Mfail)

