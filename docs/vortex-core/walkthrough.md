# Walkthrough – A Complete Operational Cycle

This page provides a narrative guided tour through a full VORTEX operational cycle. It is intentionally high-level and story-like so you can follow the flow easily. Links to deeper technical pages and worked examples are provided when you want more detail.

## Starting the Cycle – Priming and Heat Input
The system begins with a priming flow of water introduced into the canals and basins. Waste heat from industrial sources (steel mills, data centers, recycling plants, etc.) is collected by the cascading thermal fluid loop.

The thermal fluid is upgraded through relay hubs and delivered to the stepped basins inside the tunnels. As heat enters the basins, water begins to evaporate. This is the spark that starts the thermosiphon.

**Deeper detail**: See [Cascading Heat Transfer](cascading-heat.md) for how heat is collected and delivered.

## Evaporation and Steam Rise
In the stepped basins, heat causes localized boiling. Steam rises buoyantly through the upper sections of the tunnel. This upward vapor flow drives the steam harvesting units (either custom sleeves or conventional low-pressure steam turbines in a proof-of-concept variant).

The rising steam also creates a helpful draft/vacuum assist as it condenses higher up. In looped configurations this effect is particularly strong.

**Deeper detail**: See [How It Works](how-it-works.md) for the dual-phase mechanics and [Power Integration](power-integration.md) for power harvesting details.

## Condensation and Downward Flow
Steam condenses in the upper sections or in the pre-staging zone near the reservoir. The resulting liquid water flows downhill by gravity through the main canals, driving the hydro harvesting units (watermills or custom hydro sleeves).

In “endless waterfall” mode (common in looped designs), most water evaporates before reaching the lowest point, minimizing the need for upward pumping. Any remaining water returns to the central shared thermal reservoir.

**Deeper detail**: See the [Plant Bowen example](plant-bowen-example.md) or [Waste-Heat-Only Industrial Hub](waste-heat-only-industrial-hub.md) for concrete flow numbers.

## Energy Harvesting and Electricity Generation
- Descending water turns the hydro units.
- Rising steam turns the steam units.
- Both contribute to electricity generation via generators (often linked to shared driveshafts in the POC variant).

The system produces continuous power as long as heat is supplied. Excess electricity can charge batteries or power off-site hydrogen electrolysis.

**Deeper detail**: See [Power Integration](power-integration.md) for per-section math and output ranges.

## Heat Recapture and Continuous Running
Any heat that escapes the tunnel insulation is recaptured on the return cold thermal fluid lines. The pre-staging bay at the reservoir separates the cold mass from the final heat dump, keeping most energy productive inside the system.

Once running, heat saturation extends the hot zones and reduces the marginal heat required to maintain flow. This makes continuous operation increasingly efficient.

**Deeper detail**: See [Cascading Heat Transfer – Detailed](cascade-heat-detailed.md) for thermal loop mechanics.

## Closing the Loop – Reservoir and Return
Condensed water and cooled thermal fluid return to the central reservoir or are recycled. In some configurations near-boiling water can be returned to industrial users (e.g., preheating for a plant like Bowen).

The cycle repeats indefinitely, with modular maintenance allowing individual components to be swapped without shutting down the entire tunnel.

## Solar, Battery, and Hydrogen Synergies
Solar panels mounted on the tunnel structure generate additional electricity while being cooled by the thermal loop. Battery storage smooths variability and captures discharge heat. Excess power can produce hydrogen, which is preheated and injected for boost — closing another resource loop.

**Deeper detail**: See [Solar + Battery Integration](solar-battery-integration.md).

## Why This Matters
The walkthrough shows how all the pieces work together in a living system — from waste heat in to clean power and recycled resources out. Different configurations (straight tunnels, looped rings, underground sections) adapt the same core cycle to different sites and needs.

For concrete numbers and scenarios, explore the worked examples in the [Power Integration section](power-integration.md).

---

**Previous**: [Power-integration](power-integration.md)
**Index**[-Index-](../../Index.md)
**Next**: [Cascade-heat](cascading-heat.md)

