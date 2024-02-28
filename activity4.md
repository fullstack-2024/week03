# Activity 4

To install VirtualBox Guest Additions on Lubuntu, follow these steps:

1. **Update Software Packages:**
   Run the following commands in your Lubuntu virtual machine to update software packages:
   ```bash
   sudo apt update
   sudo apt upgrade
   ```

2. **Install Required Packages:**
   After the upgrade completes, install necessary packages for building kernel modules:
   ```bash
   sudo apt install build-essential dkms linux-headers-$(uname -r)
   ```

3. **Mount Guest Additions CD Image:**
   From the Virtual Machine menu bar, navigate to “Devices” and click on “Insert Guest Additions CD image.” This action mounts the Guest Additions ISO file inside your Lubuntu virtual machine.

4. **Run Guest Additions Installer:**
   Navigate to the directory where the CD image is mounted and run the installer:
   ```bash
   cd /media/"your_user_name"/VBox_GAs_7.0.14
   sudo ./VBoxLinuxAdditions.run
   ```

   This command will execute the Guest Additions installer. Follow the prompts to complete the installation.

5. **Restart System:**
   - After the installation is complete, restart your system to ensure that the changes take effect:
   ```bash
   sudo reboot
   ```
  - **Configure VirtualBox Settings:**
   With Guest Additions installed, you can enable clipboard sharing and drag-and-drop functionality between your Lubuntu guest OS and your host OS. Open VirtualBox Manager and click on “Settings.” Then, go to “General” -> “Advanced” and enable the relevant optionssami
    from the drop-down menu.

Following these steps will install VirtualBox Guest Additions on your Lubuntu virtual machine, providing enhanced features and better integration with the host OS.

- Ref: https://linuxiac.com/ubuntu-with-virtualbox/