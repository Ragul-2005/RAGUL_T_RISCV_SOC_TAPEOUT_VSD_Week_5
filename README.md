# RAGUL_T_RISCV_SOC_TAPEOUT_VSD_Week_5
<div  style="background-color:#0d1117; color:#e6edf3; padding:40px; border-radius:20px;">

# 🧩 <span style="color:#58a6ff;">OpenROAD Installation & Setup Guide</span>

## 🧠 <span style="color:#a5d6ff;">VSD Hardware Design Program</span>

<p align="center">
  
![Week](https://img.shields.io/badge/Week-5-blue?style=for-the-badge)
![Tasks](https://img.shields.io/badge/Tasks-6_Completed-brightgreen?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-OpenROAD_Setup-orange?style=for-the-badge)

</p>

---

## 📚 <span style="color:#ffa657;">Table of Contents</span>

- [⚙️ Overview](#overview)
- [🧰 Installation Process](#installation-process)
  - [📦 Getting Started: Repository Setup](#getting-started-repository-setup)
  - [🔧 Environment Configuration](#environment-configuration)
  - [🧱 Building the Tool](#building-the-tool)
  - [🧪 Testing Your Installation](#testing-your-installation)
  - [🚀 Executing the Design Flow](#executing-the-design-flow)
  - [🖥️ Viewing Results in GUI](#viewing-results-in-gui)
- [📂 Understanding the Project Structure](#understanding-the-project-structure)

---

## ⚙️ <span style="color:#79c0ff;">Overview</span>

- **OpenROAD** provides a comprehensive open-source solution for transforming RTL designs into physical **GDSII** layouts.  
- This automated toolchain handles every stage of digital IC design — from **synthesis**, **floorplanning**, **placement**, **clock distribution**, **routing**, and **final layout generation**.  
- Its streamlined approach accelerates design cycles, making it particularly valuable for **research** and **rapid prototyping** environments.

---

## 🧰 <span style="color:#ffa657;">Installation Process</span>

### 📦 Getting Started: Repository Setup

- Begin by cloning the repository with all submodules:

```bash
git clone --recursive https://github.com/The-OpenROAD-Project/OpenROAD-flow-scripts
cd OpenROAD-flow-scripts
```

###   🔧 Environment Configuration

- Execute the setup script with administrative privileges:

```bash
sudo ./setup.sh
```
### 🧱 Building the Tool

- Compile OpenROAD locally on your system:
```bash
./build_openroad.sh --local
```

### 🧪 Testing Your Installation

- Confirm successful installation by checking tool availability:
```bash
source ./env.sh
yosys -help  
openroad -help
```
### 🚀 Executing the Design Flow

- Navigate to the flow directory and run the default design:

```bash
cd flow
make
```
### 🖥️ Viewing Results in GUI

- Open the graphical interface to inspect your completed design:
```bash
make gui_final
```
🎉 <span style="color:#3fb950;">Setup Complete!</span>
Your OpenROAD environment is now fully ready for RTL-to-GDSII design exploration.

📂 <span style="color:#ffa657;">Understanding the Project Structure</span>
🏗️ Root Directory Layout

The main repository contains these key directories:

```plaintext
OpenROAD-flow-scripts/
├── docker/          → Container-based deployment files and execution scripts
├── docs/            → Complete documentation and user guides  
├── flow/            → Core RTL-to-GDSII workflow implementation  
├── jenkins/         → Continuous integration and regression testing
├── tools/           → Complete toolchain for physical design flow
├── etc/             → Dependency management and configuration scripts
└── setup_env.sh     → Environment initialization script for workflow execution
```
🧩 Flow Directory Organization

The flow/ subdirectory organizes workflow components:

```plaintext
flow/
├── design/          → Reference designs and example implementations across PDKs
├── makefile         → Build automation and flow execution control
├── platform/        → Technology libraries (liberty, LEF, GDSII) for various nodes
├── tutorials/       → Learning resources and guided examples
├── util/            → Helper scripts and utility functions
└── scripts/         → Flow-specific TCL and automation scripts
```

🧾 <span style="color:#79c0ff;">Summary</span>

This guide ensures that you can seamlessly install, build, and run the complete OpenROAD flow.
After following these steps, you’ll be able to:

✅ Clone and initialize the OpenROAD repositories
✅ Build and verify all necessary tools (Yosys, OpenROAD, etc.)
✅ Execute an end-to-end RTL-to-GDSII design
✅ Visualize layouts using OpenROAD’s GUI
✅ Understand repository organization for future projects

With these foundations in place, you can now:

Explore OpenLane integration

Perform custom floorplanning

Conduct timing analysis and DRC/LVS

Experiment with PDKs like Sky130

### 👨‍💻 <span style="color:#ffa657;">Contributor</span>
<div>
💫 RAGUL T (VLSI Design Engineer & Technology)
📍 Chennai Institute of Technology

<p align="center">
<div align="center" style="margin-top:40px;">

✨ <b>You’re now ready to begin your chip design journey with OpenROAD!</b> 🧠
🚀 <b>Let’s make silicon dreams real!</b>

<p align="center">

</p> </div> </div> ```


