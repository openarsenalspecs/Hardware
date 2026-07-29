# CircuitPath
Democratizing Chiplet Connectivity.


CircuitPath is an open-source advanced packaging and chiplet connectivity framework designed to redefine how modern AI and high-performance computing systems move data. Instead of relying on traditional monolithic SoC approaches, CircuitPath introduces a modular, simulation-driven, chiplet-based integration model built for bandwidth, determinism, and scalability.

By focusing on the system-level pathways between memory, accelerators, and compute dies, CircuitPath provides the foundation for next-generation architectures built on UCIe-style die-to-die links, 2.5D interposer layouts, and 3D stacking constraints.

## What CircuitPath Does

- Defines standardized models for chiplet interconnects, memory pathways, and packaging-layer behavior  
- Provides reference 2.5D and 3D integration layouts for real-world chiplet systems  
- Includes simulation tooling to evaluate bandwidth, latency, thermal load, and power distribution  
- Establishes a reusable architecture for composing memory, compute, and I/O chiplets  
- Creates an extensible ecosystem for new chiplet types, interposers, packaging variations, and research contributions  
- Supports an open descriptor format for system topology definition  

CircuitPath acts as the programmable “integration fabric” underlying [Conduit Systems’](https://gitlab.com/Roxanne_Ardary/conduitsystems) broader mission to rethink the path between data and decisions.

## How to Build It

CircuitPath is a modular open-source platform built around three primary layers:

### Architecture Layer  
Define system configurations using the CircuitPath descriptor format. Specify chiplets, interposers, bandwidth targets, thermal constraints, and data movement paths.

### Simulation Layer  
Run topology simulations to understand performance characteristics before taping out silicon. Evaluate:
- Chiplet placement  
- Interconnect congestion  
- Thermal envelopes  
- Latency and bandwidth distribution  
- Power delivery and heat dissipation  

### Extension Layer  
Extend the platform with new:
- Chiplet models  
- Interposer frameworks  
- Memory tile designs  
- Packaging workflows  
- Bandwidth optimization modules  

All extensions integrate with the Unified Descriptor Format, ensuring compatibility across the toolchain.

## Features

- UCIe-inspired die-to-die communication models  
- 2.5D silicon interposer reference designs  
- Early-stage 3D stacking optional modules  
- Thermal and power distribution simulation  
- Signal-integrity-aware pattern modeling  
- Extensible ecosystem for community-driven packaging and topology innovations  
- Data-driven validation through simulation and benchmark integration  
- Mature-node-friendly paths for cost-effective prototyping  

---
# CircuitPath Engineering Modules & Agent Tasks

## Module 1: UCIe Die-to-Die Communication Modeling Agent

### Purpose
Develop and optimize open die-to-die communication models for chiplet-based architectures.

### Agent Tasks
- Analyze UCIe-compatible communication requirements
- Model bandwidth, latency, and protocol behavior
- Create configurable chiplet communication templates
- Simulate link performance under different workloads
- Evaluate congestion and communication bottlenecks
- Optimize topology placement for data movement efficiency
- Generate reports comparing interconnect strategies
- Maintain compatibility with evolving chiplet standards

### Outputs
- Die-to-die communication models
- Link performance simulations
- Interconnect topology recommendations
- Communication benchmarks

---

# Module 2: 2.5D Silicon Interposer Design Agent

### Purpose
Create reference architectures for advanced 2.5D chiplet packaging.

### Agent Tasks
- Generate interposer layout models
- Define chiplet placement strategies
- Optimize routing paths between dies
- Analyze interconnect density
- Model microbump placement constraints
- Evaluate package-level bandwidth limitations
- Compare organic vs silicon interposer approaches
- Create reusable packaging templates

### Outputs
- Reference interposer designs
- Chiplet placement models
- Routing optimization data
- Packaging recommendations

---

# Module 3: 3D Stacking Architecture Agent

### Purpose
Research and model future 3D chiplet stacking architectures.

### Agent Tasks
- Analyze vertical stacking approaches
- Model TSV and hybrid bonding constraints
- Evaluate thermal challenges of stacked dies
- Optimize die ordering and placement
- Simulate vertical bandwidth scaling
- Compare stacking configurations
- Identify manufacturability limitations
- Create experimental 3D architecture proposals

### Outputs
- 3D stacking models
- Vertical integration simulations
- Thermal-aware stacking recommendations
- Future architecture proposals

---

# Module 4: Thermal & Power Distribution Simulation Agent

### Purpose
Optimize power delivery and thermal management across multi-die systems.

### Agent Tasks
- Create thermal models for chiplet architectures
- Simulate heat generation patterns
- Analyze hotspots and thermal bottlenecks
- Model power delivery networks
- Optimize voltage and power domains
- Recommend cooling strategies
- Predict thermal failures
- Generate efficiency reports

### Outputs
- Thermal simulations
- Power distribution models
- Cooling recommendations
- Reliability analysis

---

# Module 5: Signal Integrity Modeling Agent

### Purpose
Ensure reliable communication across high-density chiplet packaging.

### Agent Tasks
- Model electrical signal behavior
- Analyze crosstalk and interference
- Simulate transmission losses
- Evaluate routing quality
- Optimize trace patterns
- Identify timing issues
- Validate high-speed signaling constraints
- Generate signal quality reports

### Outputs
- Signal integrity models
- Routing improvements
- Electrical performance reports
- Design validation results

---

# Module 6: Open Packaging Ecosystem Agent

### Purpose
Manage community-driven extensions and architecture growth.

### Agent Tasks
- Maintain plugin architecture
- Validate third-party contributions
- Manage chiplet model libraries
- Track packaging innovations
- Create contribution templates
- Review new topology proposals
- Maintain compatibility standards
- Coordinate ecosystem documentation

### Outputs
- Extension framework
- Community standards
- Chiplet model registry
- Developer documentation

---

# Module 7: Simulation & Benchmark Validation Agent

### Purpose
Provide measurable validation of CircuitPath architectures.

### Agent Tasks
- Develop benchmark workloads
- Compare architecture variations
- Measure bandwidth efficiency
- Analyze latency performance
- Evaluate energy consumption
- Validate simulation accuracy
- Generate performance reports
- Recommend architecture improvements

### Outputs
- CircuitBench results
- Performance comparisons
- Validation reports
- Optimization recommendations

---

# Module 8: Mature Node Prototyping Agent

### Purpose
Create affordable pathways from simulation to physical prototypes.

### Agent Tasks
- Identify suitable semiconductor process nodes
- Evaluate manufacturing constraints
- Design prototype-ready architectures
- Optimize cost vs performance tradeoffs
- Create FPGA validation models
- Prepare shuttle fabrication concepts
- Evaluate packaging partners
- Document prototype workflows

### Outputs
- Prototype roadmaps
- Manufacturing recommendations
- Cost analysis
- Hardware validation plans

---

# Master CircuitPath Orchestration Agent

## Purpose
Coordinate all engineering modules into a unified chiplet development workflow.

### Agent Tasks
- Assign engineering tasks to specialized agents
- Maintain system architecture consistency
- Resolve conflicts between performance, cost, and manufacturability
- Track simulation results
- Recommend design iterations
- Generate architecture documentation
- Manage versioned system configurations

### Final Outputs
- Complete chiplet architecture proposals
- Simulation-validated designs
- Packaging recommendations
- Prototype-ready specifications
- Open-source contribution packages

---

## Specification Branding License (SBL)
### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/circuitpath/](https://roxanneardary.com/circuitpath/)

---


## License & Notice Requirements

CircuitPath is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- CircuitPath specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's notice.md file.
