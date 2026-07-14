# Cascading Heat Transfer System

The cascading heat loops are the circulatory system of VORTEX. They collect, upgrade, distribute, and recover heat at multiple temperature grades while driving the thermosiphon.

## Overall Heat Flow Philosophy
Heat is added at the highest practical grade and progressively stepped down. Most heat is spent productively inside the tunnel (evaporation, steam generation, basin boiling). Only residual low-grade heat reaches final polishing.

## Primary Thermal Fluid Loop
A high-temperature heat transfer fluid (specialized oils, molten salts, etc.) circulates in insulated piping through a network of relay hubs:

1. Return from reservoir (~60–75°C)
2. Low-grade hub — picks up low-temperature waste heat
3. Mid-grade hub — absorbs medium-temperature sources
4. High-grade hub — receives the hottest inputs (nuclear, H₂ combustion, concentrated solar, industrial process heat)
5. Tunnel & basins — delivers the majority of its heat into the stepped basins and canals
6. Reservoir polish — final conditioning before the cycle repeats

Piping runs in dedicated utility corridors beneath or within the tunnel floor, with double insulation, quick-connect fittings, and segment valves for safe isolation.

Basin integration occurs via high-thermal-conductivity plates or direct plug-in ports.

## Hydrogen Loop Integration
Excess electricity powers off-site electrolysis. The resulting hydrogen is routed through the main high-grade hubs (200–280°C) for pre-heating, then injected and burned at strategic points along the tunnels or directly into the stepped basins. This provides high-temperature boost, pure water regeneration, and additional combustion energy.

## Benefits
- Maximizes exergy from each temperature grade
- Self-reinforcing cycle (more heat → more power → more potential H₂ boost)
- Highly adaptable to diverse waste heat sources
- Works with both straight tunnels and looped/ringed configurations (including endless waterfall mode with a central shared reservoir)

For deeper technical details on architecture, hub design, flow behavior, integration with tunnel geometry, and operational modes, see the [detailed technical page](detailed/cascade-heat-detailed.md).

**Related Examples**  
[Plant Bowen Hypothetical](../integration/plant-bowen-example.md) | [Waste-Heat-Only Industrial Hub](../integration/waste-heat-only-industrial-hub.md)

---
**Previous**: [Power integration](power-integration.md)  
**Index**: [Index](../../Index.md)  
**Next**: [Reservoir](reservoir-upper-loop.md)
