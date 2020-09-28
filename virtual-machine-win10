# enable Hyper-V on Windows 10
## Verifying Hyper-V support
1. Open Start.
2. Search for Command Prompt and click the top result.
3. Type the following command and press Enter:

```
systeminfo.exe
```
4. Under Hyper-V Requirements, if the result reads Yes, then you can run Hyper-V.
> If the command displays No under Hyper-V Requirements, then your hardware doesn't support this feature, or you need to make sure to enable it manually.

## Enabling Hyper-V
1.  Open Control Panel.
2.  Click on Programs.
3.  Click on Turn Windows features on or off.
4.  Check the Hyper-V option making sure: Hyper-V Management Tools and Hyper-V Platform are also selected.
5.  Click OK to begin the process.
6.  After the installation completes, click Restart now to apply the changes.

#  How to create a virtual machine using Hyper-V

> Once you've completed adding the virtualization layer to Windows 10, you'll need to create a virtual machine for the Linux distribution you want to use.
However, before you do that, you must create a virtual switch to allow the VM to connect to the internet.

## Creating a virtual switch
> Use the following steps to configure a virtual switch on Hyper-V:

1.  Open Start.
2.  Search for Hyper-V Manager and click the top result.
3.  Click on the Action menu.
4.  Select New and click on Virtual Switch Manager.
5.  On the left pane, select New virtual network switch.
6.  On the right, select External.
7.  Click the Create Virtual Switch button.
8.  Enter a new descriptive name for the switch (e.g., MyVirtualSwitch).
9.  Under connection type, make sure your network adapter is select on External network.
10. Click Apply.
11. Click OK.

## Creating a virtual machine
> After creating the virtual switch, you can proceed to create a new virtual machine:

1.  Open Start.
2.  Search for Hyper-V Manager and click the top result.
3.  Click on the Action menu.
4.  Select New and click on Virtual Machine.
5.  Click the Next button.
6.  Enter a descriptive name for your virtual machine (e.g., vm-ubuntu).
7.  Use the default location to store your virtual machine, or check the Store the virtual machine in a different location option to select a different path.
8.  Click Next to continue.
9.  You can leave the default Generation 1 option selected. Or you can select Generation 2 if you want a UEFI-based firmware.
10. Click Next.
11. Select the amount of RAM to allocate for your virtual machine. In the case of Ubuntu, you need a minimum of 2GB of memory.
You can allocate as much memory as you want, but this setting will always depend on the physical memory available on your computer.
12. Click Next.
13. Use the drop-down menu to select the virtual switch you created earlier.
14. Click Next.
15. You can leave all the default settings to create a virtual hard drive, but under Size make sure to allocated at least 25GB of storage, which is the minimum required to run Ubuntu.
16. Click Next to continue.
17. On Installation options, select the Install an operating system from a bootable CD/DVD-ROM option.
18. Select the Image file (.iso) option.
19. Select the path for the ISO file with the Ubuntu installation files.
20. Click Next.
21. Click Finish.

## How to install Ubuntu Linux using Hyper-V on Windows 10

> The last step is to start the virtual machine and install the Linux distribution you want to use.

1.  On Hyper-V Manager, under Virtual Machine, right-click the newly created device, and select Connect.
2.  Click the Start (power) button.
3.  Select your language.
4.  Click the Install Ubuntu button.
5.  Check the Install third-party software for graphics and Wi-Fi hardware, Flash, MP3 and other media option.
6.  Click Continue.
7.  Select the Something else option.
8.  Click Continue.
9.  Double-click the /dev/sda drive.
10. Click Continue.
11. Double-click free space.
12. Under "Use as," use the drop-down menu and select Swap area to create a swap partition.
13. Under "Size," select the amount of space for the swap partition, which should be about 2x of the amount of RAM allocated for the virtual machine.
14. Click OK.
15. Double-click free space again.
16. Select the amount of space to allocate for the installation.
17. Under "Mount point," use the drop-down menu and select root /.
18. Click OK.
19. Select the ext4 partition from the list.
20. Click the Install Now button.
21. Click Continue to install Ubuntu.
22. Select your time zone.
23. Click Continue.
24. Select the keyboard layout.
25. Click Continue.
26. Create a user account with your information.
27. Click Continue.
28. Restart the virtual machine to finish the setup.

Quick Tip: If during the final restart process, you get a message to remove the installation and press Enter, but hitting the key won't restart the VM, just click the Turn off button and then turn it back on again.

After completing the steps, you can just turn on the VM and start using Ubuntu Linux alongside Windows 10.

While we're focusing this guide setting up Ubuntu, you can also refer to these instructions to run other distributions of Linux.

> https://www.windowscentral.com/how-run-linux-distros-windows-10-using-hyper-v
