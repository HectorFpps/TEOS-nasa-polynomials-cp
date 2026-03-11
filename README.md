# TEOS Thermodynamic Characterization for RPA 🚀
### Project: ASTERIA | ARIS Rocketry

This repository provides a specialized Python-based tool to characterize **Tetraethyl orthosilicate (TEOS)** ($SiC_8H_{20}O_4$) for high-fidelity rocket engine simulations. It generates **NASA 9-polynomial** coefficients compatible with **RPA (Rocket Propulsion Analysis)**.

## 📌 Overview
In liquid rocket engines, additives like TEOS are used to create a protective $SiO_2$ (silica) layer on combustion chamber walls (e.g., Inconel). To simulate this accurately, the solver needs precise thermodynamic properties for both the liquid fuel and the resulting gaseous combustion products.



## 🛠 Features
- **Experimental Data Integration:** Uses raw $C_p$ data from the **NIST Chemistry WebBook** (Anand et al.).
- **Dual-Phase Regression:** Performs non-linear least squares fitting for:
  - **Liquid Phase (200K - 441.2K):** For regenerative cooling analysis.
  - **Gaseous Phase (441.2K - 5000K):** For combustion and film cooling stability.
- **NASA 9 Format:** Generates the 9 required coefficients ($a_1 \dots a_7, b_1, b_2$) including the **Heat of Vaporization ($\Delta H_{vap}$)** jump at the boiling point.
- **Validation Plots:** Includes automated plotting to verify $C_p$ trends and enthalpy consistency.
