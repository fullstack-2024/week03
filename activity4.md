# Activity 4

## Part 1/3: VirtualBox Guest Additions

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

## Part 2/3: Recap

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

## Part 3/3: `nano` text editor

Below are the instructions for using the `nano` text editor to write, append, and save text:

#### 1. Writing Text:

1. Open the terminal on your Linux system.

2. Navigate to the directory where you want to create or edit a file.

3. Type the following command to open a file named `example.txt` using `nano`:
   ```bash
   nano example.txt
   ```

4. You will see the `nano` text editor interface. Start typing your text directly into the editor.

5. Once you have finished writing your text, press `Ctrl` + `O` to save the changes.

6. You will be prompted to confirm the file name. Press `Enter` to confirm.

7. Press `Ctrl` + `X` to exit `nano`.

#### 2. Appending Text:

1. Open the terminal on your Linux system.

2. Navigate to the directory where the file you want to append text to is located.

3. Type the following command to open the file `example.txt` using `nano`:
   ```bash
   nano example.txt
   ```

4. You will see the `nano` text editor interface with the content of the file displayed.

5. Move the cursor to the position where you want to append text.

6. Start typing your additional text.

7. Once you have finished appending text, press `Ctrl` + `O` to save the changes.

8. Press `Enter` to confirm the file name.

9. Press `Ctrl` + `X` to exit `nano`.

#### 3. Miscellaneous:

- **Navigation:** Use arrow keys to move the cursor around the text.
- **Editing:** Use `Backspace` to delete characters and `Ctrl` + `K` to delete entire lines.
- **Search:** Press `Ctrl` + `W` to search for text within the file.
- **Help:** Press `Ctrl` + `G` to display the help menu within `nano`.

#### Additional Notes:
- If you are creating a new file, `nano` will prompt you to confirm the file name when saving.
- Remember to use `Ctrl` + `O` to save changes and `Ctrl` + `X` to exit `nano`.
- `nano` displays a footer with common commands at the bottom of the screen for reference.

Follow these instructions to effectively use the `nano` text editor for writing, appending, and editing text files on your Linux system.


## Ref

- https://linuxiac.com/ubuntu-with-virtualbox/