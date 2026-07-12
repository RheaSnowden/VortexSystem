# Large-Scale VORTEX Integration Example: Plant Bowen

**Status**: Hypothetical / Conceptual — for illustration, sensitivity analysis, and range estimation.  
All values are order-of-magnitude and fully adjustable using the formulas provided below.

## Overview
Plant Bowen (~3.4–3.5 GW electric nameplate coal-fired capacity in Georgia, USA) serves as a realistic high-heat-density anchor point for a VORTEX network. Low-pressure steam exhaust from the plant is directed into connected VORTEX tunnels, providing strong initial drive and thermal mass. Additional heat inputs come from a colocated large AI data center, battery parks, outer-wall solar (which also cools the panels), and H₂ combustion boost. Flue gas and carbon flows can be routed through tunnels for heat recovery and cooling, with cooled CO₂ directed to low “carbon valleys.” Near-boiling water can be returned from the tunnel bottom to Bowen for preheat use.

**Highlighted Operational Advantages**
- Tunnels operate **nonstop** with no required full shutdown for routine maintenance (quick-swap modular sleeves via rail/crane system).
- The system benefits significantly from **continuous running** — heat saturation extends hot zones, reduces the marginal heat needed to maintain flow, and improves overall utilization over time.
- Near-complete internal heat consumption (cooling water/steam and thermal fluid piping feed directly into hydro flow; escaped heat is recaptured on return cold fluid via skeleton + argon layer; pre-staging bay separates cold reservoir mass from final heat dump).

## Key Assumptions (Transparent & Adjustable)
| Parameter                          | Conservative          | Optimistic              | Notes |
|------------------------------------|-----------------------|-------------------------|-------|
| Heat input per 150 ft section      | 6–10 MWth             | 12–15 MWth              | Optimum operating range |
| Hydro sleeve efficiency            | 50–55%                | 65–70%                  | Estimated/untested design target |
| Steam sleeve efficiency            | 35–40%                | 50–55%                  | Estimated/untested design target (wet steam) |
| Generator + drive efficiency       | 88–90%                | 92–94%                  | — |
| Sections per mile                  | ≈35                   | ≈35                     | 150 ft repeating module |
| Low-pressure steam from Bowen      | Significant boost     | Strong sustained driver | Direct injection into tunnels |
| Overall heat utilization           | High                  | Near-complete (>95%)    | Enhanced by continuous running & saturation |
| Tunnel network style               | More distributed      | Denser per tunnel + rings | Flexible configuration |

**Core Formulas (for generating new examples)**
- Steam mass flow (kg/s) ≈ (Heat input in MWth × 1000) / 2260
- Hydro power scales with downward liquid flow × vertical head (~23 m at 30° slope) × efficiency
- Total electric output ≈ (Hydro contribution + Steam sleeve contribution) after generator efficiency
- Annual energy (GWh or TWh) = Average power (MW) × 8760 hours × capacity factor (typically 0.85–0.95 for continuous operation)

Hydro power benefits from continuous/recirculating flow through the canals (maintained by basin level control and overflows), so output is not strictly limited to net steam production alone.

## Per-Section Breakdown (150 ft repeating module)
**Conservative (~8 MWth input)**
- Steam production ≈ 3.5 kg/s
- Hydro contribution ≈ 2.5–4 MW electric
- Steam sleeve contribution ≈ 1–2 MW electric
- **Total per section ≈ 4–6 MW electric**

**Optimistic (~13 MWth input + strong low-pressure steam boost)**
- Steam production ≈ 5.5–7+ kg/s (plus injected Bowen steam)
- Hydro contribution ≈ 5–7 MW electric
- Steam sleeve contribution ≈ 3–5+ MW electric
- **Total per section ≈ 8–12+ MW electric**

## Total System Example — 400 MWth Total Captured Heat
(Realistic mid-scale/partial integration combining Bowen low-pressure steam + waste heat + data center + solar + H₂)

**Note on scaling and heat input**: The 400 MWth example represents a realistic mid-scale or partial integration. A full-scale Bowen deployment could capture 2–6+ GWth (or more) of plant waste heat plus additions from other sources. In such larger networks the section count and output scale accordingly, supporting the higher GW electric figures with excellent integration and dense/ringed configurations.

**Conservative**
- Sections required ≈ 40–65 (more distributed tunnels)
- Average output per section ≈ 5 MW electric
- **Total system ≈ 200–325 MW electric continuous**
  - Per second: 200–325 MW
  - Per hour: 200–325 MWh
  - Annual (85% capacity factor): **≈1.5–2.4 TWh/year**

**Optimistic but plausible**
- Sections required ≈ 30–50 (denser configuration)
- Average output per section ≈ 9–11+ MW electric
- **Total system ≈ 400–800+ MW electric continuous** (scales toward 1.5–4+ GW in very large, well-integrated networks)
  - Per second: 400–800+ MW
  - Per hour: 400–800+ MWh
  - Annual (90%+ capacity factor, continuous-running benefit): **≈3.2–6.5+ TWh/year**

**Solar PV Side Benefit** (separate generation, not counted above)  
Outer-wall solar on longer tunnels adds several to tens of MW of additional electricity. Output scales with total tunnel surface area.

## Sensitivity Table (Compact)
| Total Heat Input | Conservative Output (MW electric) | Optimistic Output (MW electric) | Approx. Sections | Notes |
|------------------|-----------------------------------|---------------------------------|------------------|-------|
| 200 MWth         | 100–160                           | 200–320                         | 20–35            | Smaller/partial integration |
| 400 MWth         | 200–325                           | 400–800+                        | 30–65            | Mid-scale example |
| 1,000 MWth       | 500–800                           | 900–1,600+                      | 70–170           | Large integration |
| 3,000+ MWth      | 1,500–2,500+                      | 2,500–5,000+                    | 200–500+         | Full Bowen-scale network |

## Key Benefits in This Scenario
- Significant overall site energy efficiency improvement.
- Strong carbon management via tunneled flue gas routing and cooled CO₂ to low valleys.
- Heat and power available for surrounding industry and the plant itself.
- Nonstop operation with modular maintenance — no full shutdowns required.
- Synergies from continuous running (heat saturation, evaporation-driven draft assist, potential vortex effects from rising hot / descending cool flows). In space habitats the vacuum assist from evaporation would be significantly stronger.
- Flexible, modular addition (add or extend tunnels as heat sources allow).

## Important Caveats & Uncertainties
- The hydro sleeve is an **untested concept** — real-world performance could be lower or surprisingly higher depending on engineering, materials, and testing.
- Optimistic numbers assume excellent low-pressure steam integration and high utilization. Conservative numbers are safer for initial planning.
- Detailed CFD, thermodynamic modeling, and site-specific integration studies are required.
- Construction around an operating plant would be a major phased project.
- Steam diversion must be balanced against the original plant’s turbine output.

## How to Generate New Examples
All formulas and assumptions are explicit. Changing total heat input, sleeve efficiencies, section count, or capacity factor instantly produces new scenarios. The same per-section math applies to smaller industrial sites or larger multi-plant networks.

**Supporting calculations and variants** can be added in linked files or appendices as the repository develops.

---

**Index**[-Index-](../../Index.md)

**Related Pages**  
← [Back to Power Integration](../vortex-core/power-integration.md)  
[Solar + Battery Integration](solar-battery-integration.md) | [Plant Bowen Example](plant-bowen-example.md) | [Proof-of-Concept Variant](proof-of-concept-variant.md)

