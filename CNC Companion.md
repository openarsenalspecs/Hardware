# CNC Companion

**Tagline:** *Step-by-step to shop floor success.*

**CNC Companion** is an open-source AI-powered tutor designed to guide apprentice machinists through CNC and other shop floor machines. It provides **adaptive lessons, real-time feedback, skill tracking, and community-driven learning**, helping novices progress from beginner to skilled machinist safely and efficiently.

---

## 🔧 Features

### Core Tutoring & Learning
- Step-by-step guided lessons for any CNC machine  
- Adaptive lesson pacing based on user performance  
- Challenge mode with timed exercises or precision tasks  
- Hints, tips, and contextual suggestions during lessons  
- Error analysis for setup, toolpaths, and measurements  
- Customizable curriculum for instructors or apprentices  

### Real-Time Monitoring & Feedback
- Multi-angle camera verification of tools and workpiece  
- 3D workpiece modeling and comparison with CAD designs  
- Tool wear detection with replacement alerts  
- Safety monitoring and warnings for unsafe operations  
- Predictive guidance to anticipate mistakes  
- Performance analytics: speed, accuracy, and repeatability  

### Machine & Workflow Integration
- Universal “how-to” modules for any machine type (lathe, mill, router, grinder, 3D printer)  
- Sensor integration (encoders, torque, temperature, vibration)  
- Tool library with recommended feeds, speeds, and RPMs  
- Job logging and operation history for review  
- CAD/CAM integration: import part files and generate lessons  
- Simulation mode for virtual practice before real machining  

### Skill Tracking & Progression
- Apprentice profile with skill level tracking and progress stats  
- Gamified progression with badges, certificates, and levels  
- Personalized recommendations for practice on weak areas  
- Community challenges to share exercises and solutions  

### AI Intelligence & Customization
- Voice assistant for natural-language questions  
- Adaptive AI that learns from multiple users  
- Continuous knowledge upgrades and modular AI model integration  
- Predictive feedback and error prevention  
- AI-based real-time quality control  

## CNC Companion Multi-Agent Task Delegation Module

### Overview

The CNC Companion Multi-Agent Task Delegation Module coordinates specialized AI agents that work together to provide adaptive machining education, machine assistance, quality assurance, and continuous system improvement.

Each agent has a defined responsibility, priority level, decision boundary, and communication role. A central orchestration agent manages task routing, agent collaboration, and conflict resolution.

---

## Agent Hierarchy

## 1. CNC Companion Orchestrator Agent
**Priority Level: Critical**

### Primary Responsibilities
- Coordinates all AI agents
- Assigns tasks based on user needs and machine state
- Determines which agent has decision authority
- Maintains overall learning objectives
- Manages agent communication

### Duties
- Analyze user requests
- Break complex tasks into smaller objectives
- Delegate tasks to specialized agents
- Combine agent outputs into actionable guidance
- Resolve conflicting recommendations

### Authority
Highest-level decision coordinator.

---

## 2. Apprentice Tutor Agent
**Priority Level: Critical**

### Primary Responsibilities
- Teaches machining concepts
- Guides users through lessons
- Adjusts training difficulty
- Provides explanations and demonstrations

### Duties
- Create personalized learning paths
- Explain machining theory
- Answer apprentice questions
- Provide step-by-step instructions
- Evaluate skill development

### Metrics
- Lesson completion
- Knowledge retention
- Skill improvement
- Error reduction

---

## 3. Machine Operation Agent
**Priority Level: Critical**

### Primary Responsibilities
- Provides machine-specific operating guidance
- Understands machine manuals and procedures
- Assists with setup and operation

### Duties
- Identify machine requirements
- Guide machine preparation
- Recommend operating procedures
- Monitor operation steps
- Verify machine settings

### Supported Machines
- CNC mills
- CNC lathes
- Manual mills
- Manual lathes
- Grinders
- Routers
- Fabrication equipment

---

## 4. Safety Guardian Agent
**Priority Level: Emergency/Critical**

### Primary Responsibilities
- Prevent unsafe operations
- Monitor apprentice behavior
- Enforce safety procedures

### Duties
- Detect unsafe movements
- Monitor PPE compliance
- Identify machine hazards
- Issue warnings
- Trigger emergency escalation

### Authority
Can override other agents when safety risks are detected.

---

## 5. Computer Vision Inspection Agent
**Priority Level: Critical**

### Primary Responsibilities
- Analyze camera feeds
- Verify machining accuracy
- Inspect finished parts

### Duties
- Compare parts against specifications
- Detect defects
- Measure dimensions
- Identify surface issues
- Verify tool positioning

### Inputs
- Camera feeds
- CAD models
- Engineering drawings
- Measurement data

---

## 6. CAD/CAM Assistant Agent
**Priority Level: High**

### Primary Responsibilities
- Assist with digital manufacturing workflows

### Duties
- Interpret CAD files
- Generate machining plans
- Explain tool paths
- Identify manufacturing challenges
- Recommend improvements

---

## 7. Tooling Optimization Agent
**Priority Level: High**

### Primary Responsibilities
- Manage tooling decisions

### Duties
- Recommend cutting tools
- Suggest feeds and speeds
- Track tool life
- Detect inefficient tooling choices
- Reduce waste

---

## 8. Quality Assurance Agent
**Priority Level: High**

### Primary Responsibilities
- Maintain manufacturing accuracy

### Duties
- Compare output against specifications
- Track quality trends
- Identify recurring errors
- Recommend corrective actions
- Generate inspection reports

---

## 9. Maintenance Assistant Agent
**Priority Level: Medium**

### Primary Responsibilities
- Maintain machine reliability

### Duties
- Track machine usage
- Schedule maintenance
- Detect abnormal conditions
- Monitor vibration and temperature
- Recommend service actions

---

## 10. Knowledge Library Agent
**Priority Level: Medium**

### Primary Responsibilities
- Manage CNC Companion knowledge

### Duties
- Organize machine modules
- Maintain documentation
- Validate contributed lessons
- Update procedures
- Manage version history

---

## 11. Community Contribution Agent
**Priority Level: Medium**

### Primary Responsibilities
- Manage open-source collaboration

### Duties
- Review community lessons
- Categorize contributions
- Identify duplicate content
- Recommend improvements
- Maintain contribution standards

---

## 12. Simulation Training Agent
**Priority Level: Medium**

### Primary Responsibilities
- Provide virtual machining practice

### Duties
- Generate practice scenarios
- Simulate mistakes
- Create training challenges
- Evaluate simulated performance

---

## 13. Performance Analytics Agent
**Priority Level: Medium**

### Primary Responsibilities
- Track apprentice development

### Duties
- Analyze progress
- Identify skill gaps
- Generate reports
- Recommend training paths

---

## 14. Research & Upgrade Agent
**Priority Level: Low**

### Primary Responsibilities
- Improve CNC Companion over time

### Duties
- Monitor new machining technologies
- Recommend AI improvements
- Identify new training methods
- Suggest new modules

---

## Agent Priority Rules

## Emergency Priority
1. Safety Guardian Agent
2. Machine Operation Agent
3. Quality Assurance Agent
4. Apprentice Tutor Agent
5. Supporting Agents

---

## Normal Operation Priority

1. Orchestrator Agent
2. Apprentice Tutor Agent
3. Machine Operation Agent
4. Computer Vision Agent
5. Quality Assurance Agent
6. CAD/CAM Agent
7. Tooling Agent
8. Analytics Agent
9. Knowledge Agents

---

## Agent Communication Protocol

Each agent reports:

- Task assigned
- Current status
- Findings
- Confidence score
- Recommended action
- Required escalation

Example:
```
Agent:
Computer Vision Inspection Agent

Task:
Verify finished component dimensions

Result:
Detected 0.04mm deviation

Confidence:
97%

Recommendation:
Adjust tool offset by +0.04mm

Escalation:
None
```
---

## Future Expansion Agents

Possible future modules:

- Robotics Integration Agent
- Additive Manufacturing Agent
- Welding Tutor Agent
- Metrology Agent
- Materials Science Agent
- Production Scheduling Agent
- Supply Chain Agent
- Factory Digital Twin Agent


### Documentation & Knowledge Base
- Interactive manuals with diagrams, videos, and tutorials  
- Versioned knowledge base for machine procedures and updates  
- Open-source community contributions for new machines and lessons  
- Exportable reports and logs for apprentices and instructors  

### Interactive & Immersive Learning
- AR overlay guidance for workpiece or machine interface  
- Haptic feedback support for virtual or simulation mode  
- Gamification leaderboard for apprentice progress comparison  
- Scenario-based learning with real-world machining challenges  

### Knowledge Sharing & Community
- Open-source lesson marketplace for sharing and downloading lessons  
- Expert review system for lesson validation and improvement  
- Collaborative projects with multi-apprentice challenges tracked by AI  

### Optional / Advanced Features
- Remote mentoring and live session review  
- Maintenance assistant with scheduled calibration reminders  
- Performance dashboards with detailed metrics  
- IoT integration for advanced shop floor monitoring  

---

## ⚙ Installation

1. Clone this repository:  
```bash
git clone https://gitlab.com/Roxanne_Ardary/cnccompanion.git
```
2. Install required Python dependencies:
```bash
pip install -r requirements.txt
```
3. Connect compatible CNC machines or simulation modules.
4. Launch CNC Companion:
```bash
python run_cnccompanion.py
```
---

## 🤝 Contributing

We welcome community contributions! You can contribute by:  
- Adding new machine “how-to” modules or lessons  
- Improving AI guidance or computer vision models  
- Adding new tutorials, simulations, or AR features  
- Reporting bugs or suggesting improvements  

Please follow the open-source guidelines and ensure **all contributions maintain safety standards**.

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
  - [https://roxanneardary.com/cnc-companion/](https://roxanneardary.com/cnc-companion/)

---

## License & Notice Requirements

CNC Companion is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- CNC Companion specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## ⚠️ Important Notice

- CNC Companion is for **educational and training purposes only**.  
- Always follow machine safety protocols; the developers and contributors are not responsible for accidents, injuries, or damage caused by improper use.  
- Supervision by a qualified machinist is recommended until fully competent.  
- Always verify measurements, tool settings, and part specifications before production.  

---

## 📌 Summary

CNC Companion is your **AI shop floor mentor**:  
- Teaching fundamentals and advanced operations  
- Providing real-time feedback and monitoring  
- Tracking skill progression and performance  
- Supporting immersive AR learning and community collaboration  
- Helping apprentices achieve **step-by-step shop floor success**  
