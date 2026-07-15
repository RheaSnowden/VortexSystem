
# VORTEX Calculations & Quantitative Analysis

**Purpose**: This document is the central, transparent reference for all quantitative estimates in the VORTEX repository. Any number appearing in other documents should be traceable back to the formulas, assumptions, and reasoning presented here.

This page is written for engineers and technical reviewers who want to understand, validate, or adjust the estimates. All values are order-of-magnitude and conceptual unless otherwise noted. The calculations are modular so you can modify variables and recalculate easily.

## Key Variables & Assumptions

| Variable                          | Conservative Value          | Optimistic Value            | Notes / Reasoning |
|-----------------------------------|-----------------------------|-----------------------------|-------------------|
| Hydro sleeve efficiency           | 50–55%                      | 65–70%                      | Untested custom design; includes flow narrowing effect |
| Steam sleeve efficiency           | 35–40%                      | 50–55%                      | Accounts for wet steam conditions |
| Generator + drive efficiency      | 88–90%                      | 92–94%                      | — |
| Latent heat of vaporization       | 2.26 MJ/kg                  | 2.26 MJ/kg                  | At ~100°C (adjust for operating pressure/temperature) |
| Vertical head per 150 ft section  | 22.86 m                     | 22.86 m                     | 30° slope |
| Canal narrowing effect            | Moderate torque gain        | Higher torque gain          | 2 m half-pipe → 1.75 m full pipe (velocity increase) |

**General Notes**:
- All calculations assume water/steam as the working fluid in a closed loop.
- Heat input per 150 ft section is treated as a primary variable.
- Continuous operation and heat saturation effects are assumed after initial priming.

## Core Per-Section Formulas

### 1. Steam Mass Flow from Heat Input
$$
m_{\text{steam}} (\text{kg/s}) = \frac{Q_{\text{heat}} \times 1000}{h_{fg}}
$$

Where:
- $Q_{\text{heat}}$ = Heat input to the section (MWth)
- $h_{fg}$ = Latent heat of vaporization (kJ/kg)

### 2. Hydro Power (Gravity + Flow)
$$
P_{\text{hydro}} (\text{MW}) = \frac{\rho \times g \times Q \times h \times \eta_{\text{hydro}} \times \eta_{\text{gen}}}{1,000,000}
$$

Where:
- $\rho$ = 1000 kg/m³
- $g$ = 9.81 m/s²
- $Q$ = Volumetric flow rate (m³/s) — derived from condensed steam + recirculation
- $h$ = Vertical head (22.86 m)
- $\eta_{\text{hydro}}$ = Hydro sleeve efficiency
- $\eta_{\text{gen}}$ = Generator + drive efficiency

The canal narrowing (2 m → 1.75 m) is expected to increase velocity and torque on the sleeve.

### 3. Friction Head Loss (Simplified Darcy-Weisbach)
$$
\Delta h_{\text{friction}} \approx f \times \frac{L}{D} \times \frac{v^2}{2g}
$$

Where:
- $f$ = Darcy friction factor
- $L$ = Length of section
- $D$ = Hydraulic diameter
- $v$ = Flow velocity

This helps engineers compare frictional losses against the available driving head.

### 4. Steam Power
$$
P_{\text{steam}} (\text{MW}) \approx m_{\text{steam}} \times \Delta h \times \eta_{\text{steam}} \times \eta_{\text{gen}} / 1000
$$

Where $\Delta h$ is the effective enthalpy drop or kinetic energy available in the rising vapor.

### 5. Total Electric Output per Section
$$
P_{\text{total}} (\text{MW}) \approx P_{\text{hydro}} + P_{\text{steam}}
$$

## System-Level Example: 400 MWth Total Captured Heat

This scenario combines low-pressure steam from Plant Bowen + waste heat from a data center, solar, battery parks, and H₂ boost.

**Conservative Case**
- Sections required: ~50–65
- Average output per section: ~4–5 MW electric
- **Total system output**: **200–325 MW electric** continuous
- Annual (85% capacity factor): **≈1.5–2.4 TWh/year**

**Optimistic Case**
- Sections required: ~35–50
- Average output per section: ~9–11+ MW electric
- **Total system output**: **400–800+ MW electric** continuous
- Annual (90%+ capacity factor): **≈3.2–6.5+ TWh/year**

**Notes on Ranges**:
- Conservative values use lower sleeve efficiencies and account for higher losses.
- Optimistic values assume strong low-pressure steam integration, good heat saturation, and higher sleeve performance.
- The wide range reflects the current uncertainty in untested sleeve technology.

## Sensitivity Analysis

| Total Heat Input | Conservative Output | Optimistic Output     | Notes |
|------------------|---------------------|-----------------------|-------|
| 200 MWth         | 80–160 MW           | 160–320 MW            | Smaller integration |
| 400 MWth         | 200–325 MW          | 400–800+ MW           | Mid-scale example |
| 1,000 MWth       | 500–800+ MW         | 900–1,600+ MW         | Large cluster |
| 3,000+ MWth      | Multi-GW            | Multi-GW+             | Major regional hub |

Key sensitivities:
- Sleeve efficiencies have the largest impact.
- Heat input consistency (steady vs. variable sources) strongly affects capacity factor.
- Canal narrowing and pre-rotation effectiveness can meaningfully improve hydro output.

## Operational Thresholds

### Minimum Heat for Passive Operation
Rough estimate: **~2–5 MWth per 150 ft section** is generally required to sustain natural thermosiphon without auxiliary pumping after priming. Below this, the system may stall or require external assistance.

### Practical Maximum Capacity
Limited by:
- Steam velocity in upper sections (typically kept under 15–25 m/s to limit erosion and carryover)
- Basin heat transfer capacity
- Two-phase flow stability
- Structural and maintenance considerations for very long tunnels

At very high heat fluxes, additional tunnels become preferable to overloading a single loop.

## Uncertainties & Future Refinement

These are priority areas for deeper analysis as the project matures. The calculations above are conceptual and order-of-magnitude. Real values will be affected by:

- Actual sleeve efficiencies (requires testing or high-fidelity CFD)
- Two-phase flow behavior in inclined tunnels
- Heat transfer coefficients in stepped basins
- Pressure losses and condensation dynamics
- Material performance under continuous operation

**Recommended next steps for validation**:
- Thermodynamic cycle modeling
- CFD of sleeve performance and transition zones
- Small-scale physical prototype

## How to Use & Modify These Calculations
All formulas and assumptions are explicit. Engineers are encouraged to adjust any variable (efficiency, heat input, head, etc.) and recalculate. The structure is designed to make such modifications straightforward.

**Cross-reference** with the worked examples in the Power Integration section for context.

## References & Further Reading
- Thermosiphon and two-phase flow in inclined channels
- Waste heat recovery systems (ORC benchmarks and performance data)
- Low-head hydro turbine performance and efficiency curves
- Heat pipe and passive cooling literature
- Two-phase flow stability and pressure drop studies

*Last major update: Based on detailed scenario modeling (Plant Bowen 400 MWth case and per-section analysis).*

---
**Index**: [Index](../../Index.md)
