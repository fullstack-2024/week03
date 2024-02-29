# Activity 5: Adding a User in Linux

#### 1. Open Terminal:
   - Open the terminal on your Linux system. You can usually find it in the applications menu or by searching for "Terminal".

#### 2. Add User:
   - Use the `sudo adduser` command followed by the desired username to add a new user. For example, to add a user named "exampleuser":
     ```bash
     sudo adduser exampleuser
     ```

#### 3. Set Password (Optional):
   - If you want to set a password for the new user, you can do so using the `passwd` command:
     ```bash
     sudo passwd exampleuser
     ```
   - Follow the prompts to set and confirm the password.

#### 4. Provide User Information (Optional):
   - The `adduser` command will prompt you to provide additional information for the user, such as their full name, room number, etc. You can fill in these details or press `Enter` to skip.

#### 5. Verify User Addition:
   - To verify that the user has been added successfully, you can list the users on the system. Use the `cat` command to view the contents of the `/etc/passwd` file, which contains user account information:
     ```bash
     cat /etc/passwd
     ```

#### Additional Notes:

When using the `sudo adduser` command in Linux, by default, it creates a home directory for the new user. The home directory is typically located under the `/home` directory and has the same name as the username. 

However, if you want to specify a custom home directory for the user, you can do so by using the `--home` or `-d` option followed by the desired path when adding the user.

Here's how you can add a user with a custom home directory:

```bash
sudo adduser --home /path/to/custom/home exampleuser
```

Replace `/path/to/custom/home` with the desired path for the user's home directory and `exampleuser` with the username you're adding.

For example, if you want to add a user named "exampleuser" with a home directory located at `/srv/users/exampleuser`, you would run:

```bash
sudo adduser --home /srv/users/exampleuser exampleuser
```

This command will create the user "exampleuser" with a home directory located at `/srv/users/exampleuser`.

If you don't specify a custom home directory, `sudo adduser` will create the home directory for the user automatically under `/home/username`, where "username" is the name of the user being added.

> You can specify additional options with the `adduser` command to customize the user creation process, such as setting the home directory, user groups, etc. Refer to the manual page (`man adduser`) for more information.