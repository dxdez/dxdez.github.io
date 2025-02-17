---
layout: post
title:  "Setup Windows 11 in KVM"
date:   2025-02-12 10:26:24 -0500
---

To set up a KVM virtual machine to run Windows 11, follow these steps:

1. Install the necessary dependencies: Ensure that you have the latest version of your Linux distribution installed and configured on your system. You'll also need to install QEMU/KVM and libvirt packages for virtualization purposes. 
Follow the instructions in "How Do I Properly Install KVM on Linux" for installation and configuration.

2. Download Windows 11 ISO: Visit the Microsoft website and download the official ISO file for Windows 11. Save this file to a location where you can easily find it later.

3. Create a new virtual machine: Open your virtualization management tool, such as `virsh` or `Virt-Manager`, and create a new VM. Configure the following settings:
   - Name: Provide a unique name for your Windows 11 VM.
   - Memory: Allocate the desired amount of memory (RAM) for your virtual machine. For better performance, allocate at least 4GB or more.
   - CPU: Select an appropriate number of virtual CPUs based on your system's capacity and the requirements of Windows 11.
   - Disk Space: Allocate enough disk space for your VM. A minimum of 64GB is recommended for a smooth experience with Windows 11.
   - Network: Choose between NAT or Bridged network settings depending on your requirement.

4. Add the Windows 11 ISO as a virtual CD/DVD drive: In the VM settings, add the downloaded Windows 11 ISO file to the virtual optical drive. This allows you to boot from the ISO when starting the VM.

5. Install VirtIO drivers: Download the appropriate Virtio drivers package for your Windows 11 guest and mount it as a floppy disk or an additional CD/DVD drive during installation. Follow instructions in "How Do I Properly Install a 
Windows 11 Virtual Machine on KVM" for detailed guidance.

6. Start the virtual machine: Power on your newly created VM using your virtualization management tool. The system should boot from the Windows 11 ISO and begin the installation process. Follow the prompts to install Windows 11 in 
the VM.

7. Configure device drivers: Once the installation is complete, you will need to update the Virtio drivers for optimal performance. Visit the Microsoft Update Catalog website to download the latest drivers for your virtual hardware 
(CPU, network, graphics, etc.) and install them on your Windows 11 guest OS.

8. Install additional software: After updating device drivers, install any other necessary software or applications on your new Windows 11 VM. You can use RDP (Remote Desktop Protocol) to connect to your VM from another computer for 
easier access to the desktop environment.

Further reading:
* [How to Properly Install a Windows 11 Virtual Machine on KVM](https://sysguides.com/install-a-windows-11-virtual-machine-on-kvm)
* [How Do I Properly Install KVM on Linux](https://sysguides.com/install-kvm-on-linux#3-04-install-virtio-drivers-for-windows-guests-)
* [KVM Clients and Drivers](https://johnsiu.com/blog/win-kvm/)

