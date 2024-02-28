# Activity 5

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




