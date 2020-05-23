![Image of the Black and White Raspberry Pi Foundation Logo](resources/README/pi-logo.png)

1. [Full Part List](part-list.md "Full Part List")
1. [Full Specifications](specs.md "Full Specifications")
1. [Full Dimensions, CAD Files, and Drawings](dimensions.md "Dimensions, 3D models, etc.")
1. [Backup Server](backup-server.md "Backup Server")
5. [Tips and Tricks to Save Time When Setting Up](save-time.md "Time-Saving Tips and Tricks")
---

**Full Specifications Below:**

* Main Computing Device: **Raspberry Pi Compute Module 3+**. Currently, the CM3+ is the latest version. As the Raspberry Pi Foundation comes out with newer versions, This guide will be updated accordingly.
  * CPU Cores per Compute Module: 4
  * CPU Core Configuration: 4x ARM Cortex-A53
  * CPU Base Frequency: 1.2 GHz
  * Supports Clock Frequency Boosting: No
  * Overclockable: Yes
  * Instruction Set: ARMv8-A 64-bit
  * Total Compute Modules in Cluster: 4032
  * Total CPU Cores in Cluster: 16128
  
* Mainboard: Turing Pi. This Mainboard holds 7 Raspberry Pi Compute Modules. It has rear IO for the master node in slot 1, GPIO Pins for every Compute Module, MicroSD Card slots for every Compute Module, and uses just one ethernet port to give ethernet to all the Compute Modules. They still get their own IP Address, so no worries there.
  * Number Needed for the whole cluster: 576
  * Power Consumption Per Mainboard: 40 Watts MAX 
  * Dimensions: 6.7 x 6.7 in.(120 x 120mm)(Length x Width). This is the size of a Mini-ITX Desktop-class motherboard.
