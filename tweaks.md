![Image of the Black and White Raspberry Pi Foundation Logo](resources/README/pi-logo.png)

1. [Full Part List](part-list.md "Full Part List")
1. [Full Specifications](specs.md "Full Specifications")
1. [Full Dimensions, CAD Files, and Drawings](dimensions.md "Dimensions, 3D models, etc.")
1. [Backup Server](backup-server.md "Backup Server")
5. [Tips and Tricks to Save Time When Setting Up](save-time.md "Time-Saving Tips and Tricks")
6. [Additional Recommended Software Tweaks](tweaks.md "Additional Software Tweaks")
---

For the guaranteed success and the maximum performance possible, here are some software tweaks that I think you will find very useful in no particular order:

* **Setting the GPU memory split to 16MB.** This is done to increase the amount of RAM that is available to the system. Because we will not be installing an Operating System that has a GUI, there is not need to have huge amounts of RAM dedicated to the GPU. **To do it, follow the following steps:**

  * SSH into the Pi, or connect it directly to a monitor with a mouse and keyboard.
 
  * In the SSH terminal for the Compute Module, type ```sudo raspi-config``` along with the Compute Module's password when prompted. This will bring up the Raspberry Pi configuration utility. Once there, go to ```Advanced Options``` > ```Memory Split```. Once inside that option, delete all the numbers in the field and type 16. This will set the GPU memory to 16MB. The default is 64MB.
  
  * Now, just reboot the Compute Module for the settings to take effect

* **Enable SSH before turning it on.** This is a *REQUIRED* step for this cluster. Without SSH, it will be very hard for you to control the Compute Module. **To do it, follow the following steps:**
  * After you have flashed the MicroSD card that will go into the Compute Module, You'll have to locate the boot directory, on my Mac it's in /Volumes/boot. If you're on a Mac, open Terminal (Applications > Utilities > Terminal) and type: ```cd /Volumes/boot```
  
  * All you have to do is create an empty file called ssh. Do this by typing ```touch ssh``` after you go into the boot directory using the above command. If this file exists, ssh will be enabled when the pi is booted.
  
  * Connect the Pi to a power source to power it on. As long as the Pi is connected via an Ethernet cable (or wifi), you should now be able to ssh in to the Pi.

* **Save Commands that may be used frequently in separate script files (.sh files).** This is a very handy thing to do. For example, if you have a command that shuts down all the nodes in the cluster, and you use it quite frequently, then it might be a good idea to save that in a script that is called ```shutdown-nodes.sh```. You could have a collection of these commands called ```Utilities```.
