### 1. **Directory and Script Name:**

- **Directory Name:** `user-management-scripts`
- **Script Name:** `create_user.sh`

### 2. **GitHub Repository Name:**

- **Repository Name:** `user-management-bash-script`

### 3. **README File for GitHub:**

Below is the content for the README file. You can customize it further if needed:

---

# User Management Bash Script

## Overview

This repository contains a simple Bash script (`create_user.sh`) to automate user account creation on a Linux system. The script ensures that the user is created with a random password and forces them to change the password upon their first login.

### Key Features:

- Ensures the script runs with root privileges.
- Allows user creation with a comment field.
- Generates a random password for the user.
- Forces password reset upon the first login.
- Displays the created user's username, password, and the system hostname.

## Script Details

### Usage:

```bash
sudo ./create_user.sh USER_NAME [COMMENT]...
```

- `USER_NAME` : The name of the user to be created.
- `[COMMENT]` : Optional comment describing the user.

### Example:

```bash
sudo ./create_user.sh john_doe "John Doe - Developer"
```

### Output:

After the user is created, the following information will be displayed:

- Username
- Password (randomly generated)
- Hostname (system on which the user was created)

### Prerequisites:

- This script must be executed with `sudo` or as the `root` user.

### Directory Structure:

```
user-management-scripts/
├── create_user.sh
└── README.md
```

### Notes:

- The password generated is a 12-character random string.
- The script forces the user to change the password upon their first login.

## How to Use

1. Clone this repository:
    ```bash
    git clone https://github.com/Jameel-25/user-management-bash-script.git
    ```

2. Navigate to the script directory:
    ```bash
    cd user-management-bash-script
    ```

3. Run the script as `root` or using `sudo`:
    ```bash
    sudo ./create_user.sh USER_NAME [COMMENT]...
    ```

## License

This project is licensed under the MIT License.

---

### 4. **Steps to Upload to GitHub:**

1. **Initialize the Repository:**
   - Run the following commands inside your `user-management-scripts` directory:

   ```bash
   cd user-management-scripts
   git init
   git add .
   git commit -m "Initial commit: added user creation script and README"
   ```

2. **Push to GitHub:**
   - Assuming you've already created the repository on GitHub with the name `user-management-bash-script`, run the following commands:

   ```bash
   git remote add origin https://github.com/yourusername/user-management-bash-script.git
   git branch -M main
   git push -u origin main
   ```
