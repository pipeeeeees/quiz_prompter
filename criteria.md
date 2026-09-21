Here's a comprehensive list organized by area. Each bullet is phrased as something you could quiz on, so you can turn them directly into rubric items (e.g., score 0-3 per bullet).

## 1. Circuit Fundamentals
- 1.1 Ohm's law, Kirchhoff's laws, Thevenin/Norton equivalents
- 1.2 RC, RL, and RLC transient and frequency response; time constants; corner frequencies
- 1.3 Impedance of R, L, C across frequency; parasitic behavior (ESR, ESL, self-resonance)
- 1.4 Op-amp basics: inverting/non-inverting, gain-bandwidth, slew rate, input bias, offset, stability with capacitive loads
- 1.5 Active filters (Sallen-Key, MFB) and passive filter design
- 1.6 Comparators, hysteresis, Schmitt triggers
- 1.7 Bipolar and MOSFET operation: regions, Vgs(th), Rds(on), gate charge, SOA
- 1.8 Diode types (rectifier, Schottky, Zener, TVS) and when to use each
- 1.9 Bode plots, phase margin, gain margin, basic feedback theory

## 2. Power Design
- 2.1 Linear regulators (LDO): dropout, PSRR, quiescent current, thermal dissipation
- 2.2 Buck, boost, buck-boost, flyback, SEPIC: operation and tradeoffs
- 2.3 Inductor selection: saturation vs. RMS current, ripple current, DCR
- 2.4 Output capacitor selection: ESR, ripple, transient response, DC bias derating
- 2.5 Control modes: voltage mode, peak current mode, COT; compensation basics
- 2.6 Efficiency calculation and loss breakdown (conduction, switching, gate drive, core)
- 2.7 Power sequencing, soft-start, inrush limiting, brown-out behavior
- 2.8 Battery chemistry (Li-ion, LiFePO4, NiMH), charging profiles, fuel gauging
- 2.9 Protection: OVP, UVLO, OCP, reverse polarity, load switches, eFuses
- 2.10 Power tree design and budgeting (steady-state and peak loads)
- 2.11 USB-C/PD basics and power negotiation
- 2.12 Decoupling and bulk capacitance strategy

## 3. Digital Design
- 3.1 Logic families and levels (CMOS, LVCMOS, LVDS, open-drain), level translation
- 3.2 Setup/hold time, clock skew, metastability
- 3.3 Pull-ups/pull-downs, open-drain vs. push-pull, bus contention
- 3.4 Reset and power-on behavior, supervisors, watchdogs
- 3.5 Clock sources: crystals, oscillators, PLLs, jitter, load capacitance, ppm accuracy
- 3.6 Boot configuration pins and strapping
- 3.7 Basic FPGA/CPLD concepts: LUTs, constraints, clock domain crossing (if relevant)
- 3.8 Memory types (SRAM, DRAM, Flash, EEPROM) and interface considerations

## 4. Communication Interfaces
- 4.1 I2C: addressing, pull-up sizing, clock stretching, bus capacitance limits
- 4.2 SPI: modes (CPOL/CPHA), chip-select behavior, max speeds
- 4.3 UART/RS-232/RS-485: framing, baud error, termination, biasing
- 4.4 CAN/CAN-FD: differential signaling, termination, arbitration
- 4.5 USB: speeds, differential pair routing, ESD protection, enumeration basics
- 4.6 Ethernet: PHY vs. MAC, magnetics, RGMII/RMII, PoE basics
- 4.7 PCIe, DDR, MIPI, HDMI basics (routing rules, impedance, length matching), scaled to what your products use
- 4.8 Wireless: BLE, Wi-Fi, LoRa, cellular module integration basics
- 4.9 Debug interfaces: JTAG, SWD, UART consoles

## 5. Analog and Mixed-Signal
- 5.1 ADC types (SAR, sigma-delta, pipeline), resolution vs. ENOB, sampling rate, aliasing
- 5.2 ADC input driving: source impedance, anti-alias filtering, reference quality
- 5.3 DAC basics and output buffering
- 5.4 Sensor interfacing: thermistors, RTDs, thermocouples, strain gauges, photodiodes, Hall sensors
- 5.5 Instrumentation amplifiers and common-mode rejection
- 5.6 Noise sources: thermal, shot, 1/f; noise budget calculations
- 5.7 Grounding strategies for mixed-signal boards (analog vs. digital return paths)
- 5.8 Voltage references: accuracy, drift, noise
- 5.9 Precision resistor and capacitor considerations (tolerance, tempco, dielectric type)

## 6. PCB Layout
- 6.1 Stackup design: layer count, plane placement, dielectric thickness, controlled impedance
- 6.2 Return path concepts and why plane splits are dangerous
- 6.3 Trace width and current capacity (IPC-2221/2152), via current, copper weight
- 6.4 Via types (through, blind, buried, micro), via stubs, via-in-pad
- 6.5 Differential pair routing: coupling, skew, length matching
- 6.6 Impedance calculation: microstrip vs. stripline
- 6.7 Decoupling capacitor placement and loop inductance
- 6.8 Switching regulator layout: hot loops, ground return, feedback routing
- 6.9 Crosstalk mitigation and spacing rules (3W)
- 6.10 High-voltage creepage and clearance (IPC-2221, IEC 60664 / 62368)
- 6.11 Thermal management: copper pours, thermal vias, heatsinking, exposed pads
- 6.12 Connector, test point, and mounting hole placement
- 6.13 Silkscreen, fiducials, panelization, keep-outs

## 7. Signal Integrity and EMC
- 7.1 Transmission line behavior: when a trace becomes a transmission line (rule of thumb by rise time)
- 7.2 Reflections, termination strategies (series, parallel, AC, source)
- 7.3 Eye diagrams, jitter, inter-symbol interference
- 7.4 Common-mode vs. differential-mode noise
- 7.5 Radiated vs. conducted emissions; common sources and mitigation
- 7.6 ESD protection: IEC 61000-4-2, TVS placement, return paths
- 7.7 EMI filtering: ferrite beads, common-mode chokes, pi filters
- 7.8 Shielding, grounding, and cable considerations
- 7.9 Pre-compliance testing techniques (near-field probes, LISN)
- 7.10 Immunity testing: EFT/burst, surge, radiated immunity
- 7.11 Crosstalk and power integrity: PDN impedance, target impedance, ground bounce

## 8. Component Selection and Supply Chain
- 8.1 Reading datasheets critically: absolute max vs. recommended operating conditions, typical vs. guaranteed specs
- 8.2 Capacitor types (MLCC, tantalum, electrolytic, polymer), DC bias derating, microphonics
- 8.3 Resistor types and power ratings, derating curves
- 8.4 Inductor and ferrite bead selection criteria
- 8.5 Connector selection: current rating, mating cycles, environmental sealing
- 8.6 Lifecycle status (active, NRND, EOL), second sourcing, pin-compatible alternates
- 8.7 Lead times, allocation risk, and broker/counterfeit risks
- 8.8 Package types (QFN, BGA, WLCSP, SOT) and their assembly implications
- 8.9 Cost/performance tradeoffs and BOM cost management
- 8.10 Automotive/industrial/commercial temperature grades

## 9. Simulation and Analysis
- 9.1 SPICE simulation: what it can and can't tell you, model accuracy
- 9.2 Worst-case and Monte Carlo analysis, tolerance stack-up
- 9.3 Thermal analysis and estimation (junction temp, theta-JA, theta-JC)
- 9.4 SI/PI simulation tools and when they're worth using
- 9.5 Power budget and reliability calculations
- 9.6 Timing analysis for digital interfaces
- 9.7 Fault analysis (FMEA/FMECA) at the circuit level

## 10. Lab Skills and Debugging
- 10.1 Oscilloscope usage: probing technique, ground lead effects, bandwidth, triggering, measuring ripple properly
- 10.2 Multimeter, power supply, electronic load, and function generator use
- 10.3 Logic analyzer and protocol decoding
- 10.4 Spectrum analyzer and VNA basics
- 10.5 Thermal camera and thermocouple use
- 10.6 Board bring-up procedure (power rails first, current limiting, sequencing)
- 10.7 Systematic fault isolation: hypothesis, measurement, narrowing
- 10.8 Soldering, rework (hot air, BGA), and jumper wire fixes
- 10.9 Common failure signatures (shorts, cold joints, ESD damage, latch-up)
- 10.10 Measurement uncertainty and knowing when a measurement is lying to you

## 11. Design for Manufacturing, Test, and Reliability
- 11.1 DFM: minimum trace/space, annular ring, drill sizes, solder mask rules, fab capabilities
- 11.2 DFA: component orientation, spacing, tombstoning risk, reflow profile awareness
- 11.3 Solder types (leaded/lead-free), RoHS, and reflow considerations
- 11.4 Test strategy: ICT, flying probe, functional test, boundary scan, test point access
- 11.5 Programming and calibration in production
- 11.6 Reliability concepts: MTBF, derating, burn-in, HALT/HASS, bathtub curve
- 11.7 Environmental considerations: humidity, conformal coating, vibration, thermal cycling
- 11.8 Failure analysis basics: common failure modes of capacitors, connectors, solder joints
- 11.9 Tolerance and yield: how component variation affects production yield

## 12. Compliance and Standards
- 12.1 FCC Part 15, CE marking, and basic RED/EMC directive awareness
- 12.2 Safety standards (IEC 62368-1, UL 60950 legacy, UL 94 flammability)
- 12.3 Medical (IEC 60601), automotive (ISO 26262, AEC-Q100/200), industrial standards, as relevant
- 12.4 RoHS, REACH, WEEE
- 12.5 Battery transport and safety (UN 38.3, IEC 62133)
- 12.6 Ingress protection ratings (IP codes)
- 12.7 Wireless certification (module vs. intentional radiator, SAR)
- 12.8 Labeling and documentation requirements

## 13. Firmware and Software Awareness
- 13.1 Reading and reasoning about register maps and datasheets from the firmware perspective
- 13.2 Bootloader and boot sequence basics
- 13.3 GPIO, interrupts, DMA, timers, PWM concepts
- 13.4 Low-power modes and their hardware implications
- 13.5 Writing simple test firmware or scripts for bring-up
- 13.6 Python/scripting for test automation and data analysis
- 13.7 Version control (Git) for hardware projects

## 14. Mechanical and System Integration
- 14.1 Thermal design at the enclosure level (convection, conduction, airflow)
- 14.2 Connector and cable interfaces to mechanical design
- 14.3 Board mounting, stress relief, and flex concerns (MLCC cracking)
- 14.4 Tolerance stack-ups between PCB, enclosure, and connectors
- 14.5 Enclosure materials and their effect on RF and EMC
- 14.6 Antenna placement and ground plane considerations
- 14.7 Basic understanding of DFM constraints from injection molding or sheet metal

## 15. Process, Documentation, and Communication
- 15.1 Product lifecycle stages: proof of concept, EVT, DVT, PVT, MP
- 15.2 Design review practice: what to review at schematic, layout, and pre-release stages
- 15.3 Schematic quality: hierarchy, naming, notes, readability
- 15.4 Design checklists and lessons-learned practices
- 15.5 BOM management and revision control
- 15.6 ECO/ECN process and change management
- 15.7 Root cause analysis methods (5 Whys, fishbone, 8D)
- 15.8 Requirements definition and traceability
- 15.9 Writing clear test plans and reports
- 15.10 Estimating effort and communicating risk to stakeholders

## Suggested Rubric Approach
- **Weight sections by your domain.** A power-electronics engineer should weight sections 2, 6, and 7 heavily, while an IoT engineer might weight 4, 12, and 14.
- **Pair each bullet with a "war story" prompt:** "Describe a time this went wrong in a design." Practical experience is a stronger signal than textbook recall.

# Scoring Approach

Score each quiz item on **answer quality**, separate from experience. Judge the answer against a pre-written answer key with 3-5 key points per item.

## Per-Item Score (0-4)

| Score | Label | Criteria |
|---|---|---|
| **0** | Wrong / blank | Incorrect, or can't answer. Also use 0 for a *confidently wrong* answer, and flag it (see below). |
| **1** | Minimal | Recognizes the term or gets one key point, but the explanation is mostly wrong or too vague to apply. |
| **2** | Partial | Gets the core idea, but misses key points or has a meaningful error. Wouldn't be safe to apply without checking. |
| **3** | Mostly right | Hits nearly all key points. Only minor omissions or imprecision (e.g., forgets a derating factor, fuzzy on a number but right on the concept). Would produce a working design. |
| **4** | Perfect | Complete and accurate, states the assumptions and edge cases, and gives correct numbers or rules of thumb where relevant. |

**Quick rule of thumb for graders:**
- Would a design based on this answer **fail or be unsafe**? → 0 or 1
- Would it **work but be suboptimal or miss an edge case**? → 2 or 3
- Would it **work and hold up in review**? → 4

## Flags (tracked separately, not part of the score)

- **Confidently wrong (CW):** The person stated an incorrect answer with high certainty. This is riskier than "I don't know," so track the count per section.
- **Experience (E):** They gave a real war story where they hit this issue. It doesn't change the score, but it shows depth.
- **Needs refresh (R):** They knew it once but it's rusty. Useful for prioritizing study.

## Optional Confidence Calibration

Have the person rate their confidence (Low / Med / High) before seeing the result. Compare it to the score:

| | Score 0-1 | Score 2 | Score 3-4 |
|---|---|---|---|
| **High confidence** | Danger zone (CW) | Overconfident | Solid |
| **Low confidence** | Known gap | Calibrated | Underconfident, build trust |

## Section-Level Results

Average the item scores per section and convert to a percentage (average ÷ 4):

| Section Score | Interpretation |
|---|---|
| **85-100%** | Strong. Maintain with periodic review. |
| **70-84%** | Solid for mid-level. Fill specific gaps. |
| **50-69%** | Developing. Prioritize study on missed items. |
| **Below 50%** | Gap area. Needs focused learning or mentorship. |

**Mid-level target:** about 70%+ in your core sections, 50%+ in adjacent ones, with **zero or near-zero CW flags** in safety-critical areas (power, protection, high-voltage clearance, compliance).

## Spreadsheet Layout

| Section | Question | Score (0-4) | Confidence (L/M/H) | Flags (CW/E/R) | Notes / Missed Points |
|---|---|---|---|---|---|

Add a summary tab with per-section averages, CW counts, and a list of every item scored 0-2 as your study queue.

## Sample Scored Answer

**Question:** *Why does an MLCC's capacitance drop on a 5V rail?*
- **0:** "Because it heats up." (Wrong)
- **1:** "Ceramic caps change with voltage somehow." (Recognizes it, no mechanism)
- **2:** "DC bias reduces capacitance, especially in small packages." (Core idea, no numbers or dielectric context)
- **3:** "DC bias derating on X5R/X7R, can lose 50%+ at rated voltage, bigger case or higher voltage rating helps." (Nearly complete)
- **4:** All of the above, plus: Class II dielectric polarization mechanism, check the manufacturer's DC bias curve rather than the nominal value, C0G/NP0 has no such effect, and it matters for regulator stability and ripple calculations.
