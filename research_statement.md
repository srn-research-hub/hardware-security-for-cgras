## Background & Motivation

The paper [1] inserts post-configuration Trojans on FPGAs by exploiting the gap between verified bitstreams and runtime configuration. Malicious circuits are inserted during place-and-route, made inert via disconnected interconnects (TPIPs), and later activated by compromised tools. CGRAs, with similar compiler-driven mapping and runtime configuration, faces risks of the same kind.

## Focus

Study how toolchain trust and interconnect programmability create stealth Trojan surfaces in CGRAs, and develop defensive methods for detection and mitigation.

## Objectives
- Define an attacker model for latent/dormant Trojans in CGRA flows
- Develop detectors for Trojan indicators: unexpected PE reuse, and abnormal routing/resource allocation
- Measure how small routing/mapping changes affect observable signals and performance and how detectable those changes are.
- Exploring Undetectable trojans that will slowly eat away at the device and compromise data flowing through the system for the attacker

# Next steps:
    platform/tool: morpher 

- Research and document various types of trojans and attacks that can happen on reconfigurable fabrics, analyse the impact of said trojans and proceed on which attack/trojan to start with accordingly.
- Prototype lightweight trojans to induce anomalous routing
- Run routing-variation experiments on open CGRA flows to test detection methods
- Build a reproducible-build pipeline to assess toolchain trust.
- Prototype lightweight detectors for anomalous routing.

# Add on(want feedback on this)
- utilizing ai agents built thriugh langgraph to automate and speed up the process of introducing and analysing various trojans swiftly

Reference:
[1] Ahmed, Q.A., Wiersema, T. & Platzner, M. Post-configuration Activation of Hardware Trojans in FPGAs. J Hardw Syst Secur 8, 79–93 (2024). https://doi.org/10.1007/s41635-024-00147-5
