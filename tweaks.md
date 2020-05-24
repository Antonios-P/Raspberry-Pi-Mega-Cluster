![Image of the Black and White Raspberry Pi Foundation Logo](resources/README/pi-logo.png)

1. [Full Part List](part-list.md "Full Part List")
1. [Full Specifications](specs.md "Full Specifications")
1. [Full Dimensions, CAD Files, and Drawings](dimensions.md "Dimensions, 3D models, etc.")
1. [Backup Server](backup-server.md "Backup Server")
5. [Tips and Tricks to Save Time When Setting Up](save-time.md "Time-Saving Tips and Tricks")
6. [Additional Recommended Software Tweaks](tweaks.md "Additional Software Tweaks")
---

For the guaranteed success and the maximum performance possible, here are some software tweaks that I think you will find very useful in no particular order:

* **Setting the GPU memory split to 16MB.** This is done to increase the amount of RAM that is available to the system. Because we will not be installing an Operating System that has a GUI, there is not need to have huge amounts of RAM dedicated to the GPU. *Insert how this can be done here*

* **Enable SSH before turning it on.** This is a *REQUIRED* step for this cluster. Without SSH, it will be very hard for you to control the Compute Module. *Insert how this can be done here.*

* **Save Commands that may be used frequently in separate script files (.sh files).** This is a very handy thing to do. For example, if you have a command that shuts down all the nodes in the cluster, and you use it quite frequently, then it might be a good idea to save that in a script that is called ```shutdown-nodes.sh```. You could have a collection of these commands called ```Utilities```.
