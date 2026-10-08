# 💻 Bare-Metal Windows 11 Deployment & Disk Partitioning (Lenovo Hardware)

## 📌 Overview
This project documents a bare-metal installation, disk partitioning layout, and baseline system initialization of **Windows 11** on physical Lenovo laptop hardware. It demonstrates practical hands-on technical skills in BIOS/UEFI firmware configuration, storage drive management, operating system installation via bootable media, and post-installation driver verification.

---

## 🎯 Lab & Deployment Objectives
* **Bootable Media Preparation:** Create a bootable Windows 11 USB installer using standard system utility tools.
* **Firmware Configuration:** Access and configure Lenovo BIOS/UEFI settings to modify boot priority and system modes.
* **Storage Allocation & Partitioning:** Execute a clean disk partition strategy (System, OS, and Data partitions) using Windows Setup Disk Management tools.
* **Post-Deployment Verification:** Initialize user profiles, install cumulative Windows Updates, and verify hardware device drivers via Device Manager.

---

## 🛠️ Hardware & Tools
* **Target Hardware:** Lenovo Laptop System
* **Installation Media:** Windows 11 Bootable USB Drive
* **Firmware Interface:** Lenovo UEFI/BIOS Utility
* **Core Competencies:** Bare-Metal OS Deployment, Disk Partitioning (GPT/MBR), Driver Management, Hardware Troubleshooting

---

## 📑 Detailed Step-by-Step Implementation

### Phase 1: Installation Media & Firmware Setup
1. Created a clean **Windows 11 bootable USB drive** using official installation tools.
2. Intercepted the boot sequence on the physical Lenovo laptop by entering the **NOVO Button / Function Key (F12/F2)** menu.
3. Accesses the **UEFI/BIOS menu** to verify storage controller modes and boot device order.
4. Selected the bootable USB drive as the primary boot target.

### Phase 2: Disk Partitioning & Operating System Installation
1. Launched the Windows 11 setup installer from the physical USB drive.
2. Navigated to the custom disk management screen to examine the internal drive layout.
3. Cleaned existing unallocated space and executed a custom disk partitioning plan:
   * Allocated dedicated space for System Boot / Recovery partitions.
   * Defined primary partition parameters for the Operating System (`C:` drive).
   * Formatted remaining unallocated space for localized data storage.
4. Selected the primary OS partition and completed the Windows 11 installation workflow.

### Phase 3: Post-Installation & Hardware Initialization
1. Configured initial Out-Of-Box Experience (OOBE) settings including user account creation, region, and privacy options.
2. Performed system health and connectivity checks.
3. Executed **Windows Update** to fetch security patches and system updates.
4. Accessed **Device Manager (`devmgmt.msc`)** to inspect all hardware devices and verify that all Lenovo system drivers (Chipset, Network, Graphics, Audio) were properly installed without yellow warning flags.

---

## 🧠 Key Skills Demonstrated
* **Physical Systems Deployment:** Hands-on experience with bare-metal physical hardware installation rather than virtual environments.
* **Disk & Storage Management:** Understanding GPT disk layouts, partition
