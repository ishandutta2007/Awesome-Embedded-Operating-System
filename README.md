# Awesome-Embedded-Operating-System

# Awesome-Embedded-Operating-System

**Curated List of Commercial Platforms & Open-Source GitHub Projects**
*Focused on Real-Time Operating Systems (RTOS), Embedded Linux & Safety-Certified Kernels*
**Last updated: October 2026**

This repository tracks notable **commercial platforms** and **open-source projects** for **Embedded Operating Systems**. These tools help developers build firmware for microcontrollers, IoT devices, industrial controllers, and safety-critical systems—where deterministic behavior, small footprint, and real-time guarantees matter.

**Examples** include Windows IoT, FreeRTOS, Zephyr RTOS, Embedded Linux, VxWorks, QNX Neutrino, RIOT OS, ThreadX, Contiki-NG, and Mbed OS (the category leaders).

**Open-source emphasis**: The open-source embedded OS ecosystem is **exceptionally mature and production-proven**. **FreeRTOS** has been open source for over 20 years under the MIT license and is actively maintained by AWS with Long Term Support (LTS) releases . **Zephyr RTOS** reached **version 4.4** in April 2026 with support for OpenRISC, WireGuard, and Wi-Fi Direct . **Eclipse ThreadX** provides a vendor-neutral, **safety-certified** RTOS under the MIT license . **RT-Thread 5.3.0** (September 2026) added **Rust language support**, device-tree-based device models, and DVFS . **Apache NuttX 9.0** (September 2026) added RISC-V 64, x86_64, and ELF64 support .

## 📖 Table of Contents

- [🔓 Commercial Platforms](#-commercial-platforms)
- [🔓 Open-Source GitHub Projects](#-open-source-github-projects)
- [🤝 How to Contribute](#-how-to-contribute)
- [⚠️ Disclaimer](#-disclaimer)

## 🔓 Commercial Platforms

> **📊 Market Context**: The global embedded operating system market is estimated at **~$15B in 2026**, growing toward **~$30B by 2032**. The sector is **moderately concentrated** — **VxWorks** (Wind River) and **QNX Neutrino** (BlackBerry QNX) dominate safety-critical and automotive segments, while **Windows IoT** serves Microsoft-centric industrial deployments. **Pricing varies dramatically**: QNX charges **per-project license fees** with **runtime royalties** for production units, VxWorks uses **per-developer seat licensing** with **runtime options**, and Windows IoT Core is **free for prototyping** but requires **device licensing for commercial deployment**. **Mbed OS was sunsetted by Arm in July 2026** — no longer actively maintained, though the source remains available under Apache 2.0 . No single vendor holds a winner-take-all position; enterprises typically choose based on certification requirements (ISO 26262, IEC 61508) and hardware ecosystem.

| Platform | Description | Pricing (Starting Tier) | Free Tier Limits | Company Size |
|----------|-------------|------------------------|------------------|--------------|
| **[Windows IoT](https://developer.microsoft.com/en-us/windows/iot)** | **Microsoft's embedded Windows platform.** Windows IoT Enterprise and Windows IoT Core for industrial devices, kiosks, and gateways. | **Windows IoT Core**: Free for prototyping. **Commercial deployment**: Device licensing required (OEM volume pricing). **Windows IoT Enterprise**: Per-device license via OEM. | **Free for prototyping and development** — no production license required until commercial deployment. | **~$281B revenue (Microsoft FY2025)** |
| **[VxWorks](https://www.windriver.com/products/vxworks)** | **The gold standard for safety-critical RTOS.** Certified for DO-178C, IEC 61508, ISO 26262, and FDA Class III. Used in Mars rovers, medical devices, and avionics. | **Per-developer seat license** + **runtime royalties** for production units. **Custom enterprise pricing** — quote required. | **No free tier** for commercial use. **Evaluation license** available on request. | **Private (Wind River, ~$500M+ revenue est.)** |
| **[QNX Neutrino](https://blackberry.qnx.com/)** | **Microkernel RTOS for automotive, medical, and industrial.** Certified for ISO 26262 ASIL D, IEC 61508 SIL 3, and FDA. **Used in 255+ million vehicles.** | **Per-project license** + **runtime royalties**. **Custom enterprise pricing** — quote required. | **QNX Everywhere**: Free for non-commercial use (education, hobby projects). **No free tier for commercial deployment**. | **Part of BlackBerry (~$500M+ revenue est.)** |

## 🔓 Open-Source GitHub Projects

Sorted by relevance to embedded development. Star badge links to each repo's stargazers page.

| Repo | Description | Stars |
|------|-------------|-------|
| **[Zephyr RTOS](https://github.com/zephyrproject-rtos/zephyr)** — **The fastest-growing open-source RTOS.** **Zephyr 4.4** (April 2026) adds **OpenRISC support, WireGuard, Wi-Fi Direct**, and more . Backed by the Linux Foundation with contributions from Intel, Nordic, NXP, Renesas, and STMicroelectronics. Supports ARM, RISC-V, x86, Xtensa, ARC, MIPS, SPARC, and OpenRISC . **Apache-2.0**. | [![Stars](https://img.shields.io/github/stars/zephyrproject-rtos/zephyr?style=social&color=white)](https://github.com/zephyrproject-rtos/zephyr/stargazers) | ~13,000 |
| **[FreeRTOS](https://github.com/FreeRTOS/FreeRTOS)** — **The most widely deployed RTOS.** Open source for **over 20 years** under the **MIT license** . Actively maintained by AWS with **LTS releases** providing security updates and critical bug fixes for two years . Includes kernel plus libraries for TCP/IP, Bluetooth, and OTA updates. Runs on **40+ microcontroller architectures**. | [![Stars](https://img.shields.io/github/stars/FreeRTOS/FreeRTOS?style=social&color=white)](https://github.com/FreeRTOS/FreeRTOS/stargazers) | ~4,000 |
| **[Apache NuttX](https://github.com/apache/nuttx)** — **Apache's mature RTOS for deeply embedded systems.** **NuttX 9.0** (September 2026) added **RISC-V 64, x86_64, and ELF64 support**, plus STM32H747I-DISCO, Sipeed Maix Bit, and many new architectures . **Apache-2.0**. | [![Stars](https://img.shields.io/github/stars/apache/nuttx?style=social&color=white)](https://github.com/apache/nuttx/stargazers) | ~3,500 |
| **[RT-Thread](https://github.com/RT-Thread/rt-thread)** — **Chinese open-source RTOS with IoT focus.** **v5.3.0** (September 2026) added **Rust language support**, device-tree-based device models, **DVFS** (dynamic voltage and frequency scaling), and **VirtIO 1.2** . **Apache-2.0**. | [![Stars](https://img.shields.io/github/stars/RT-Thread/rt-thread?style=social&color=white)](https://github.com/RT-Thread/rt-thread/stargazers) | ~9,000 |
| **[Eclipse ThreadX](https://github.com/eclipse-threadx/threadx)** — **Vendor-neutral, safety-certified RTOS under the MIT license** . **ThreadX v6.4.2** (February 2025) is the latest release . Provides **pre-certified safety packages** for IEC 61508, ISO 26262, and DO-178C. Includes TCP/IP, USB, File System, and GUIX. **MIT**. | [![Stars](https://img.shields.io/github/stars/eclipse-threadx/threadx?style=social&color=white)](https://github.com/eclipse-threadx/threadx/stargazers) | ~2,500 |
| **[RIOT OS](https://github.com/RIOT-OS/RIOT)** — **The friendly, IoT-focused RTOS.** **RIOT-2026.07** (July 2026) fixed 12 issues since 2026.04 . Designed for **wireless sensor networks** and **IoT edge devices** with a focus on energy efficiency, real-time capabilities, and small memory footprint. **LGPL-2.1**. | [![Stars](https://img.shields.io/github/stars/RIOT-OS/RIOT?style=social&color=white)](https://github.com/RIOT-OS/RIOT/stargazers) | ~3,000 |
| **[Contiki-NG](https://github.com/contiki-ng/contiki-ng)** — **The OS for next-generation IoT devices.** **Release 5.0** (December 2024) is the latest . Focused on **low-power wireless** and **constrained devices** with built-in 6LoWPAN, RPL, and CoAP. **BSD-3-Clause**. | [![Stars](https://img.shields.io/github/stars/contiki-ng/contiki-ng?style=social&color=white)](https://github.com/contiki-ng/contiki-ng/stargazers) | ~1,500 |
| **[µC/OS-III](https://github.com/weston-embedded/uC-OS3)** — **Micrium's preemptive, highly portable RTOS.** **µC/OS-II** is **certified for safety-critical applications** in medical, aerospace, and industrial markets . Includes TCP/IP, USB, and File System. Available via Weston Embedded. **Apache-2.0** (source available). | [![Stars](https://img.shields.io/github/stars/weston-embedded/uC-OS3?style=social&color=white)](https://github.com/weston-embedded/uC-OS3/stargazers) | ~500 |
| **[Mbed OS Community Edition (Mbed CE)](https://github.com/mbed-ce/mbed-os)** — **Community fork of Mbed OS.** **Arm sunsetted Mbed OS in July 2026** — no longer actively maintained or supported by Arm . **Mbed CE** is the community-driven continuation. **Apache-2.0**. | [![Stars](https://img.shields.io/github/stars/mbed-ce/mbed-os?style=social&color=white)](https://github.com/mbed-ce/mbed-os/stargazers) | ~200 |

**Additional open-source options worth exploring:**

| Repo | Description |
|------|-------------|
| **[Zephyr LTS](https://github.com/zephyrproject-rtos/zephyr)** — Long-term support releases of Zephyr RTOS for production deployments. |
| **[FreeRTOS LTS](https://github.com/FreeRTOS/FreeRTOS-LTS)** — Long-term support libraries with security updates for two years . |
| **[eCos](https://github.com/ecos-projects/ecos)** — Configurable RTOS for embedded systems, used in industrial and telecom applications. |
| **[BeRTOS](https://github.com/bertos/bertos)** — Modular RTOS for embedded systems with a small footprint. |

## 🤝 How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's commercial or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## ⚠️ Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Embedded OS platforms handle safety-critical systems; certification requirements (IEC 61508, ISO 26262, DO-178C) must be independently verified before deployment.
- **Critical lifecycle notice**: **Mbed OS was sunsetted by Arm in July 2026** — no longer actively maintained. The **Mbed OS Community Edition (Mbed CE)** fork is under active development and recommended for continued use .
- **Open-source reality**: The open-source ecosystem for embedded OS is **exceptionally mature and production-proven**. **FreeRTOS** has been open source for **over 20 years** and is actively maintained by AWS with LTS releases . **Zephyr RTOS** reached **version 4.4** in April 2026 with OpenRISC and WireGuard support . **Eclipse ThreadX** provides a **vendor-neutral, safety-certified** RTOS under MIT license . **Apache NuttX 9.0** added RISC-V 64 and x86_64 support . **RT-Thread 5.3.0** added Rust support . However, **commercial platforms** (VxWorks, QNX Neutrino) provide **pre-certified safety packages** and **long-term support guarantees** that open-source alternatives may lack for the most demanding safety-critical applications. The open-source path is **genuinely viable** for IoT, industrial, and many safety-critical deployments.

---

**Made for embedded engineers, firmware developers, IoT architects, and real-time systems specialists.**
Let's make embedded operating systems more open, transparent, and accessible.
