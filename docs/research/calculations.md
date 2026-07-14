# Research, Calculations & Estimates

This page collects the quantitative foundation for the VORTEX system — formulas, key assumptions, performance estimates, and worked examples. It serves as the central reference for calculations that appear throughout the documentation.

> **Note**: All values are conceptual / order-of-magnitude unless otherwise stated. Real-world performance will require detailed thermodynamic modeling, CFD analysis, and site-specific engineering.

## Key Assumptions & Parameters
- Tunnel slope: 30–45° (30° preferred for length vs. drive)
- Effective tunnel length examples: 1 mile, 3+ miles, or stacked/ring configurations
- Heat sources: Nuclear (ideal), industrial waste heat, geothermal, etc.
- Working fluid: Water/steam (closed loop)
- Minimum heat/steam threshold required to sustain natural thermosiphon circulation

## Thermosiphon & Flow Fundamentals
- Driving force: Density difference between rising steam and descending liquid + gravitational component on the incline.
- Key physics: Buoyancy-driven two-phase flow, latent heat of vaporization, and gravity-assisted liquid return.
- Placeholder for detailed head calculation:

- Where:
- Δρ = density difference (steam vs liquid)
- L = effective length along incline
- θ = slope angle

## Power Generation Estimates
**Preliminary order-of-magnitude estimates** (strong heat input assumed):

| Configuration              | Estimated Electric Output     | Notes |
|----------------------------|-------------------------------|-------|
| 1 mile effective length    | 100 – 800+ MW                 | Depends on heat flux and efficiency |
| 3+ miles or stacked/ringed | Multi-GW scale possible       | Highly scalable with network size |
| Per 150 ft section (V-formation) | Scales proportionally    | Modular building block |

**Efficiency considerations**:
- Overall system efficiency limited by Carnot efficiency for the available temperature difference.
- Dual-phase extraction (hydro + steam sleeves) aims to improve net energy capture.
- Distributed sleeves reduce single-point losses and improve availability.

## Sleeve Turbine Performance
- Hydro sleeves: Extract kinetic energy from downward liquid flow in sloped canals.
- Steam sleeves: Extract energy from upward vapor flow (kinetic + pressure work).
- Modular design: 2–3 sleeves per generator (incremental linking).
- Placeholder for efficiency curves and power-per-sleeve estimates.

## Worked Example Placeholder
Detailed calculations for a specific plant (e.g. Bowen or similar industrial/nuclear site) are documented in:
- `plant-bowen-example.md` (or link here once created)

Cross-reference any specific numbers or assumptions from that example here for easy comparison.

## Scaling & Integration
- Networked tunnels can form “arcology spines” or industrial park rings.
- Synergy with carbon capture, district heating, or agricultural thermal loops.
- Closed-loop water balance minimizes external makeup requirements.

## Future Work & Open Questions
- Detailed thermodynamic cycle modeling (1D or CFD)
- Two-phase flow stability in inclined counter-current sections
- Sleeve turbine efficiency curves at relevant Reynolds numbers and steam qualities
- Material compatibility and long-term degradation
- Economic modeling (LCOE comparisons)

## References & Further Reading
- Thermosiphon and two-phase flow literature
- Waste heat recovery technologies (ORC, Kalina cycle, etc.)
- Rim-driven and ducted turbine designs
- Arcology and large-scale closed-loop habitat concepts

---

**How to use this page**:
- Add new calculations as they are developed.
- Link specific results back to the main docs (Summary, How It Works, Power Integration, etc.).
- Keep assumptions clearly stated so readers can evaluate or improve them.

Contributions to this section (new formulas, references, or example refinements) are especially welcome — see [CONTRIBUTING.md](../../CONTRIBUTING.md).

---  
**Index**: [Index](../../Index.md) 
