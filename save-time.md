![Image of the Black and White Raspberry Pi Foundation Logo](resources/README/pi-logo.png)

1. [Full Part List](part-list.md "Full Part List")
1. [Full Specifications](specs.md "Full Specifications")
1. [Full Dimensions, CAD Files, and Drawings](dimensions.md "Dimensions, 3D models, etc.")
1. [Backup Server](backup-server.md "Backup Server")
5. [Tips and Tricks to Save Time When Setting Up](save-time.md "Time-Saving Tips and Tricks")
6. [Additional Recommended Software Tweaks](tweaks.md "Additional Software Tweaks")
---

![Image of the Black and White Raspberry Pi Foundation Logo](resources/README/pi-logo.png)

1. [Full Part List](part-list.md "Full Part List")
1. [Full Specifications](specs.md "Full Specifications")
1. [Full Dimensions, CAD Files, and Drawings](dimensions.md "Dimensions, 3D models, etc.")
1. [Backup Server](backup-server.md "Backup Server")
5. [Tips and Tricks to Save Time When Setting Up](save-time.md "Time-Saving Tips and Tricks")
6. [Additional Recommended Software Tweaks](tweaks.md "Additional Software Tweaks")
---

**Below are some helpful tips and tricks to save time when first setting up your Compute Module Cluster:**

* *Get as far as you can with one Compute Module and clone that MicroSD card to the other Modules.* **|** This is talking in terms of setup. If there a piece of software or a setting that needs to be done on all the Compute Modules, instead of manually doing it for every Module, do it on just one and then automate the changes by cloning the MicroSD card.
  * You can use the ```dd``` command to achieve this.
  * Make sure to shrink the file system and compress the image for maximum space efficiency. *More information on how to do this can be found in the wiki.*
  
* *Backup all the MicroSD cards to a central location.* | This is very crucial. Since MicroSD cards don't have Write Endurance like AT ALL, they will eventually fail; much faster than an SSD or Hard Drive. The central location that i have chosen is the backup server which you can get to by visiting the link in the menu.
