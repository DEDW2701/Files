# Technology landscape described in patents.csv

Executive summary
- Core domain: vehicle telematics, in-vehicle diagnostics, and fleet/fleet-like equipment monitoring.
- Typical stack: sensing from ECUs/OBD/CAN, edge acquisition devices, short-range links on the vehicle (e.g., trailer–tractor), backhaul (cellular/IP), and cloud analytics that produce alerts, diagnostics, and business actions.
- Dominant classifications: G07C 5/00 family (vehicle monitoring/registration) is central, with H04L/H04W (data/wireless comms), G06Q (business/fleet ops), G06F (computing/error handling), G05B (industrial control), and B60* (vehicle systems) frequently co-occurring.
- Themes span from early “vehicle monitoring system” logging (1990s–2000s) to proactive, ML-informed diagnosis, standardization across fleets, and connected trailer/tractor architectures (2020s).

Core technical building blocks
- Data acquisition: OBD/CAN/ECU interfaces; reading fault codes (DTCs), sensor streams, vibration/condition metrics.
- On-vehicle networking: short-range links between modules (e.g., trailer sensors to a master control unit), automatic protocol detection, tractor–trailer wireless setup.
- Backhaul and cloud: cellular/IP telematics links, remote servers ingesting logs, rules/ML models for diagnosis and prioritization, dashboards and alerts (including audible/mobile UI).
- Analytics and decisioning: DTC sequencing and prioritization, standardized KPIs across heterogeneous vehicles, anomaly-triggered circular buffers, predictive maintenance and cost estimation.
- Applications: fleet management and maintenance scheduling, insurance telematics/risk scoring, connectivity health troubleshooting, driver/vehicle behavior monitoring.

Thematic clusters with representative examples
1) Vehicle monitoring/logging
   - WO9009645A1 (1990) and WO03073339A1 (2003): early “Vehicle Monitoring System” disclosures.
   - US8892451B2 (Progressive, 2014): logging with risk/safety attributes and networked access.

2) Diagnostics, fault codes, and prioritization
   - US9563492B2 (2017): DTC sequencing to decide repair order.
   - US9811951B2 (UPS, 2017): fleet-oriented management and state-setting for fault codes.

3) Fleet information standardization and maintenance analytics
   - US9672667B2 (2017): standardizing fleet operation metrics from telematics.
   - US8244779B2 (2012): rules-based analysis for maintenance alerts.

4) CAN/ECU interfacing and tooling
   - US8751098B2 (2014): monitoring CANbus info via integrated wireless systems.
   - US8589018B2 (2013): diagnostic tool auto-identifies ECU protocols, with copy protection.
   - US10650621B1 (2020): interface with CAN, compute operating stats, estimate fuel cost.

5) Connected trailer/tractor and on-vehicle wireless
   - US10973061B2 (2021): establishing a wireless network across tractor–trailer.
   - US11496816B2 (2022): bridge integrator unit linking trailer sensors over short-range wireless to a telematics master.

6) Proactive/ML-driven diagnosis and user-facing alerts
   - US11170585B2 (GM, 2021): augmented DFMEA ties diagnostics and signals to failure modes (ML under G06N20/00).
   - US11978291B2 (Zonar, 2024): anomaly-triggered logs sent remotely for diagnosis.
   - US11270529B2 (2022): server analysis produces mobile audible alerts.

7) Network-of-moving-things and broader connectivity
   - US11343327B2 (Veniam, 2022): managing OBD data across a network of moving things.
   - US12081052B2 (Polaris, 2024) and US12143285B2 (Deere, 2024): connectivity health/troubleshooting across CAN and Ethernet in machines/vehicles.

Notable actors and use-cases
- Commercial fleets and logistics: UPS, Zonar, Omnitracs.
- OEMs and tier suppliers: GM, WABCO (ZF), Truck-Lite, Deere, Polaris.
- Telematics/diagnostics and networking: Veniam, Innova Electronics, ioCurrents.
- Insurance telematics: Progressive.

Observed trends (1990 → 2024)
- From data logging and remote parameter checking to connected, cloud-managed fleets with automated prioritization and user alerts.
- Increasing emphasis on standardization across heterogeneous vehicles to make fleet KPIs comparable.
- Growth of on-vehicle wireless architectures (tractor/trailer, sensor bridges) enabling retrofit and modularity.
- Integration of ML/analytics (e.g., augmented DFMEA, anomaly buffers) for predictive and proactive maintenance.
- Expansion into business/operations workflows (G06Q): scheduling service, risk/pricing, and operational decision support.

Frequent CPC/IPC families (plain-language)
- G07C 5/00: registering/monitoring vehicle operation, driver behavior, usage; producing operational records.
- H04L / H04W: data communications and wireless network protocols for telematics backhaul and device networking.
- G06Q: business/operations data processing for fleet management, scheduling, billing/insurance.
- G06F / G05B: digital computing, condition monitoring, and control logic on the edge and in the cloud.
- B60* (B60R, B60W, B60L, B62D): vehicle equipment, drive control, power/charging, and trailer/tractor systems.
- G01M: testing machines/vehicles (e.g., vibration/condition-monitoring).

Scope notes
- Dataset covers 1990–2024 across US and WO filings, with strong concentration in vehicle monitoring (G07C) and pervasive co-classification in communications (H04L/H04W) and fleet/business processing (G06Q).
- The technology set is cohesive: sensing → connectivity → cloud analytics → operational actions. The modern emphasis is proactive diagnosis, modular retrofit connectivity, and standardized fleet metrics powering business decisions.