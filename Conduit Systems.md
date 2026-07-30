# Conduit Systems
Rethink the Path Between Data and Decisions.


Conduit Systems is an open system architecture platform designed to rethink how data moves between memory, compute, and accelerators in modern AI and high-performance computing environments. Instead of treating compute as the primary constraint, Conduit Systems focuses on the **data movement layer**, enabling deterministic, high-bandwidth, and simulation-driven system design.

At its core, Conduit Systems integrates advanced chiplet packaging concepts, system-level memory orchestration, and modular compute topologies into a unified, extensible framework.

---

## What Conduit Systems Does

- Defines system-level data movement between memory, compute, and accelerator chiplets  
- Provides a modular architecture for composing heterogeneous compute systems  
- Simulates bandwidth, latency, thermal behavior, and power distribution across multi-die systems  
- Enables programmable control of memory pathways and compute locality  
- Supports extensible chiplet-based system design through open descriptors and plugins  
- Serves as the parent architecture for CircuitPath (advanced packaging layer)  

---

## Features + Updated Technology

### Core Features
- **Modular Data Routing** – Define and orchestrate data flows between system components and chiplets  
- **Event-Driven Architecture** – React to system states, workload changes, and hardware conditions in real time  
- **Smart Transformation Layer** – Modify and optimize data as it moves through system pathways  
- **Source-Agnostic Input System** – Supports APIs, databases, streaming data, and hardware-level feeds  
- **Destination-Agnostic Output System** – Route outputs to storage, compute, or external services  
- **Unified Mapping Engine** – Declarative or visual mapping of system-level data movement  
- **Flow Validation Layer** – Ensures correctness of system topology and data routing  
- **Error Isolation Zones** – Prevent localized failures from cascading across the system  
- **Real-Time Monitoring Dashboard** – Tracks performance, bandwidth, and system health  
- **Plugin Extension Framework** – Supports custom compute, memory, and routing modules  

---

### Updated Technology Stack

#### System Architecture
- Memory-centric compute orchestration model  
- Disaggregated chiplet-based system topology  
- Deterministic bandwidth allocation framework  
- Hardware-aware execution planning layer  

#### CircuitPath Integration Layer
- UCIe-style die-to-die interconnect modeling  
- 2.5D interposer and 3D stacking layout support  
- Parametric packaging generation system  
- Thermal-aware floorplanning and routing models  

#### ConduitOS Runtime
- Topology-aware workload scheduler  
- Distributed memory fabric manager  
- Bandwidth reservation and allocation protocol  
- Latency-aware execution planning  

#### Simulation & Modeling
- Full system digital twin (compute + memory + interconnect)  
- Signal integrity and congestion simulation  
- Thermal and power distribution modeling  
- AI-assisted interposer routing optimization  

#### Chiplet & Packaging Technologies
- UCIe-class interconnect abstraction  
- Hybrid bonding and high-density stacking support  
- Active silicon bridge fabric modeling  
- Backside power delivery awareness  

#### Benchmarking & Validation
- CircuitBench system performance suite  
- Bandwidth utilization metrics  
- Thermal efficiency analysis  
- Cross-chiplet latency measurement  
- Tensor throughput per watt evaluation  

#### Ecosystem Layer
- Open chiplet plugin system  
- Community-driven interposer and memory models  
- Extensible packaging architecture library  
- Open simulation contribution framework  

---

## How to Build It

Conduit Systems is designed as a modular stack composed of:

### 1. Architecture Layer
Define system configurations using declarative descriptors that specify:
- Chiplet types  
- Memory layout  
- Interconnect topology  
- Bandwidth constraints  
- Thermal and power budgets  

### 2. Simulation Layer
Run full-system simulations before hardware design:
- Latency modeling  
- Bandwidth congestion analysis  
- Thermal distribution simulation  
- Power efficiency estimation  

### 3. Runtime Layer (ConduitOS)
Execute workloads using topology-aware scheduling:
- Memory-aware task placement  
- Dynamic bandwidth allocation  
- Compute locality optimization  
- Real-time system adaptation  

### 4. Extension Layer
Extend the ecosystem with:
- New chiplet models  
- Packaging layouts  
- Simulation modules  
- Hardware abstraction layers  

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
  - [https://roxanneardary.com/conduitsystems/](https://roxanneardary.com/conduitsystems/)

---

## License & Notice Requirements

Conduit Systems is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Conduit Systems specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.  

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## Summary

Conduit Systems provides a unified architecture for system-level data movement, enabling modular chiplet-based design, simulation-driven validation, and runtime-aware execution for next-generation AI and high-performance computing systems.
