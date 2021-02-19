# Install-Ubuntu-on-Hyper-V

# Instruction
Installing Ubuntu on Hyper Visor is pretty straight forward. The only problem is that the VM does not load as fullscreen.  Ill show you step by step on how to do this.


# Configure full screen 
Once you installed Ubuntu

== Click on the bottom Left corner button
type in Terminal to open Terminal
Start terminal
Type in:
sudo nano /etc/default/grub
enter user password to access the root files

Change the GRUB_CMDLINE_LINUX_DEFAULT=”quiet splash” line to GRUB_CMDLINE_LINUX_DEFAULT=”quiet splash video=hyperv_fb:1920x1080”
Hold CNRTL, ^, E to exit file
Click yes

in termminal 
type in:
sudo update-grub
Restart your VM, enter Full Screen mode and enjoy.
