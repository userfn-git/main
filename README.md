<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:04070D,50:0B192C,100:1E3E62&height=240&section=header&text=MOHAMMED%20ALKHALDI&fontSize=44&fontColor=00F5D4&fontAlignY=36&desc=Systems%20Architect%20%7C%20Low-Latency%20Physics%20%26%20Input%20Engine%20Developer&descAlignY=56&descSize=16&descColor=E2E8F0" width="100%" alt="FN-WORKSTATION Header" />
  <a href="https://github.com/userfn-git/main">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=18&duration=3000&pause=900&color=00F5D4&center=true&vCenter=true&multiline=false&width=880&height=38&lines=Deterministic+Zero-Overhead+Native+Engines+(C%2B%2B20+%2F+Lua+5.5+%2F+Python);Shared+Memory+IPC+(Local%5CFN_PHYSICS_SHM)+%26+Vector+Clamping;240Hz+Competitive+KBM+Mechanics+(fnpro.space+%2F+FN3_2);Unified+Multi-Node+Baseline%3A+FN-WORKSTATION+%2B+HONOR+X6c+(NIC-LX2)" alt="Telemetry Stream" />
  </a>
  <br/>
  <p>
    <a href="https://github.com/userfn-git/main"><img src="https://img.shields.io/badge/PRIMARY%20HUB-userfn--git%2Fmain-0B192C?style=for-the-badge&logo=github&logoColor=00F5D4" alt="Main Hub"/></a>
    <a href="https://github.com/userfn-git/wiki-live-core"><img src="https://img.shields.io/badge/KNOWLEDGE%20CORE-wiki--live--core-0B192C?style=for-the-badge&logo=git&logoColor=00F5D4" alt="WikiLife Core"/></a>
    <a href="https://fnpro.space"><img src="https://img.shields.io/badge/DOMAIN-fnpro.space-0B192C?style=for-the-badge&logo=cloudflare&logoColor=00F5D4" alt="Domain"/></a>
    <a href="mailto:fnprospace@gmail.com"><img src="https://img.shields.io/badge/CONTACT-fnprospace%40gmail.com-0B192C?style=for-the-badge&logo=gmail&logoColor=00F5D4" alt="Email"/></a>
  </p>
  <p>
    <img src="https://img.shields.io/badge/C%2B%2B20-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++20"/>
    <img src="https://img.shields.io/badge/Python%203.12%20%7C%203.15-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
    <img src="https://img.shields.io/badge/Lua%205.4%20%7C%205.5-2C2D72?style=flat-square&logo=lua&logoColor=white" alt="Lua"/>
    <img src="https://img.shields.io/badge/PowerShell%205.1%20%7C%207-5391FE?style=flat-square&logo=powershell&logoColor=white" alt="PowerShell"/>
    <img src="https://img.shields.io/badge/CMake%20%2B%20Ninja-064F8C?style=flat-square&logo=cmake&logoColor=white" alt="CMake"/>
    <img src="https://img.shields.io/badge/PyTorch%20%2B%20CUDA-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch"/>
  </p>
</div>

---

## 01 // Systems & Physics Engineering Architecture

> **Lead Architect:** Mohammed Alkhaldi (`userfn-git`) · **Location:** Al Jubail, Saudi Arabia  
> **Design Doctrine:** Bare-Metal Determinism · Zero Cloud Bloat · Kernel-Level Anti-Cheat (`EOS`) Compliance

I engineer self-contained, offline-capable native software systems operating directly over **Windows Internals**. Every input capture layer, vector-clamping curve, and Shared Memory IPC telemetry bridge is built for sub-millisecond determinism without bloated third-party middleware.

```text
+-------------------------------------------------------------------------------------+
|                     FN-WORKSTATION REAL-TIME TELEMETRY PIPELINE                     |
+-------------------------------------------------------------------------------------+
|  [Logitech G502 X / PRO X 60] ---> RawInput / DirectInput (Zero-Latency Capture)    |
|               |                                                                     |
|               v                                                                     |
|  [fn_physics_engine] ------------> C++20 / Lua 5.5 Vector Clamping & Deadzone       |
|               |                    (Internal DZ: 0.05 | Curve Exp: 1.40 - 1.45)     |
|               v                                                                     |
|  [Shared Memory IPC] ------------> Local\FN_PHYSICS_SHM (Lock-Free Ring Buffer)     |
|               |                                                                     |
|               +---> [RocketSim 16-Arena RL] (PyTorch / CUDA GTX 1660 Ti)            |
|               +---> [WikiLife Core] ------> Tree-Structured Archival (main)         |
+-------------------------------------------------------------------------------------+
```

---

## 02 // Official Technical References & Standards Registry

| Subsystem / Domain | Stack & Implementation | Official Reference Standard |
| :--- | :--- | :--- |
| **Systems & Native Extensions** | `C++20`, `pybind11` (`physics_core.pyd`), `CMake`, `Ninja` | [ISO C++20 Standard](https://isocpp.org/std/the-standard) · [pybind11 Docs](https://pybind11.readthedocs.io/) |
| **Windows Kernel & IPC** | `RawInput`, `DirectInput`, `Shared Memory` (`CreateFileMappingW`) | [Microsoft Win32 IPC Docs](https://learn.microsoft.com/en-us/windows/win32/ipc/interprocess-communications) · [Raw Input API](https://learn.microsoft.com/en-us/windows/win32/inputdev/raw-input) |
| **Embedded Scripting & Curves** | `Lua 5.4 / 5.5`, `FN PRO Lua Engine v9.4.0`, Logitech G HUB SDK | [Lua 5.4 Reference Manual](https://www.lua.org/manual/5.4/) · [Logitech G Developer Lab](https://www.logitechg.com/en-us/innovation/developer-lab.html) |
| **Physics & RL Simulation** | `RocketSim`, `pyrocketsim`, 16-Arena Actor-Critic (`rl_actor_critic_v1.pt`) | [RocketSim Official Repo](https://github.com/ZealanL/RocketSim) · [PyTorch Stable Docs](https://pytorch.org/docs/stable/index.html) |
| **Collision & Rigid Body** | Continuous Collision Detection (`CCD`) & Trajectory Solvers | [Jolt Physics Documentation](https://jrouwe.github.io/JoltPhysics/) |
| **Replay Binary Telemetry** | `.replay` Bitstream Deserialization & Match Analytics | [rrrocket Parser](https://github.com/nickbabcock/rrrocket) · [Ballchasing API](https://ballchasing.com/doc/api) |
| **Shell & Toolchain Governance** | `PowerShell 5.1 / 7`, `MSYS2 UCRT64`, `WSL2 Ubuntu` | [PowerShell Docs](https://learn.microsoft.com/en-us/powershell/) · [MSYS2 Documentation](https://www.msys2.org/docs/what-is-msys2/) |
| **Workstation & Mobile Hardware** | `ASUS SM-H610` / `Intel i5-12400F` / `HONOR X6c (NIC-LX2)` | [Intel ARK i5-12400F](https://www.intel.com/content/www/us/en/products/sku/134587/intel-core-i512400f-processor-18m-cache-up-to-4-40-ghz/specifications.html) · [HONOR X6c Official Specs](https://www.honor.com/mea-ar/support/phones/honor-x6c/) |
| **Knowledge & Repo Governance** | `WikiLife Core` (4 Paths / 12 Branches / `ADR-0001..0013`) | [wiki-live-core Architecture](https://github.com/userfn-git/wiki-live-core) · [GitHub Docs](https://docs.github.com/en/communities) |

---

## 03 // Unified Multi-Node Hardware & Device Baseline

### Node A — Primary Workstation (`FN-WORKSTATION` / PC)

| Subsystem | Component & Model | Technical Specifications |
| :--- | :--- | :--- |
| **Host & OS** | `FN-WORKSTATION` · Microsoft Windows 11 Pro | Version `25H2` (OS Build `26200`, 64-bit, `HVCI` Enforced) |
| **Motherboard** | ASUS `SM-H610` | UEFI BIOS `4003` (Custom Q-Fan & PCIe Power Tuning) |
| **Processor (CPU)** | 12th Gen Intel Core `i5-12400F` | 6 Cores / 12 Threads @ 2.50 GHz (Boost up to 4.40 GHz) |
| **Graphics (GPU)** | NVIDIA GeForce `GTX 1660 Ti` | Locked 240 FPS Frame Pacing & CUDA Compute |
| **Memory (RAM)** | **32 GB** Physical DDR4 | Dual-Channel High-Throughput Configuration |
| **Storage Array** | Kingston & ADATA NVMe SSDs | BitLocker-Encrypted Partitions (`D:\projects` Isolated Workspace) |
| **Peripherals** | Logitech `G502 X` + Logitech `PRO X 60` + `240Hz` Display | Sub-Millisecond RawInput & Low-Latency Visual Pipeline |

### Node B — Mobile Client (`HONOR X6c` / Android)

| Subsystem | Component & Model | Technical Specifications |
| :--- | :--- | :--- |
| **Device & Model** | **HONOR X6c** (`NIC-LX2` / `TAC: 86567207`) | Certified Mobile Client Node (IMEI1 Verified & Redacted) |
| **Operating System** | **Android 15** (`MagicOS 9.0`) | Official HONOR Mobile OS Environment |
| **SoC / Processor** | MediaTek `Helio G81 Ultra` (12nm Octa-Core) | 2x Cortex-A75 @ 2.0 GHz + 6x Cortex-A55 @ 1.7 GHz |
| **Graphics (GPU)** | ARM `Mali-G52 MC2` | Dual-Core Mobile Graphics Engine |
| **Display** | `6.61"` TFT LCD (`120Hz` Refresh Rate) | `1604 x 720` Resolution, 1010 nits Peak Brightness |
| **Battery & Power** | `5300 mAh` Li-Polymer | `35W` HONOR SuperCharge Wired |
| **Connectivity** | Wi-Fi 5 Dual-Band (`802.11ac`), Bluetooth `5.1`, `NFC` | USB Type-C 2.0 (OTG) · `IP64` Dust & Splash Resistant |

---

## 04 // Competitive Mechanics & Telemetry (`Rocket League`)

<p>
  <img src="https://img.shields.io/badge/HANDLES-fnpro.space%20%7C%20FN3__2-1E3E62?style=flat-square&logo=epicgames&logoColor=00F5D4" alt="Handles"/>
  <img src="https://img.shields.io/badge/INPUT-100%25%20KBM%20(RawInput)-1E3E62?style=flat-square&logo=logitechg&logoColor=00F5D4" alt="KBM"/>
  <img src="https://img.shields.io/badge/FRAME%20PACING-240%20FPS%20LOCKED-1E3E62?style=flat-square&logo=nvidia&logoColor=00F5D4" alt="240FPS"/>
  <img src="https://img.shields.io/badge/CURVE-DZ%200.05%20%7C%20EXP%201.40--1.45-1E3E62?style=flat-square" alt="Curve"/>
</p>

- **Core Mechanics:** `Speedflips`, `Fast Aerials`, `Flip Resets`, `Chain Dashes`, `Stalls`, and precision `Wall-to-Ground` recoveries.
- **Deterministic KBM Control Matrix (`TAInput.ini`):** `W/A/S/D` Movement · `LeftMouseButton` Boost · `RightMouseButton` Jump · `LeftShift` Powerslide & Air Roll · `Q/E` Directional Air Roll · `C / MiddleMouseButton` Rear View.

---

## 05 // Ecosystem & Active Repositories

| Repository / Engine | Scope & Architecture | Status |
| :--- | :--- | :--- |
| **[`userfn-git/main`](https://github.com/userfn-git/main)** | **Primary Hub (This Repo):** Unified PC & Mobile hardware registry, official references, and governance baseline. | `ACTIVE` |
| **[`userfn-git/wiki-live-core`](https://github.com/userfn-git/wiki-live-core)** | **Cognitive & Knowledge Engine:** 4-Path, 12-Branch tree-structured archival and CI/CD governance system. | `ACTIVE` |
| **`fn_physics_engine` & `RL_Master_Engine`** | **Physics & Telemetry Suite:** `C++20` / `Lua 5.5` / `Python` Shared Memory IPC (`Local\FN_PHYSICS_SHM`) engine. | `PRODUCTION` |

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:1E3E62,50:0B192C,100:04070D&height=110&section=footer" width="100%" alt="Footer" />
</div>
