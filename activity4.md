# Activity 4

## Part 1

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

## Part 2


Use Linux commands to create the following directory hierarchy:

```sh
config
  - db.js
controllers
  - todoTaskController.js
  - userController.js
middleware
  - customMiddleware.js
  - requireAuth.js
models
  - todoTaskModel.js
  - userModel.js
routers
  - todoTaskRouter.js
  - userRouter.js
.env
README.md
server.js
``` 

<details>

<summary>Here's a step-by-step guide to creating the specified directory hierarchy using Linux commands</summary>

```bash
# Create main directories
mkdir config controllers middleware models routers

# Create files inside each directory
touch config/db.js
touch controllers/todoTaskController.js
touch controllers/userController.js
touch middleware/customMiddleware.js
touch middleware/requireAuth.js
touch models/todoTaskModel.js
touch models/userModel.js
touch routers/todoTaskRouter.js
touch routers/userRouter.js
touch .env
touch README.md
touch server.js

# Verify directory structure
ls -R
```

This set of commands will create the specified directory structure with empty files. You can run these commands in your Linux terminal to create the desired hierarchy. After executing these commands, you can use the `ls -R` command to verify that the directory structure has been created correctly.

</details>


- Ref: https://linuxiac.com/ubuntu-with-virtualbox/