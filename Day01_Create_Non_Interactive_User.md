# Day 01 – Create Non-Interactive User (xFusionCorp)

## Task
The system admin team at xFusionCorp Industries required a user with a non-interactive shell
for a backup agent tool.

## Requirements
- User name: john
- Server: App Server 3
- Shell: Non-interactive

## Solution

### Step 1: Connect to App Server 3
```bash
ssh stapp03

Step 2: Create the user with non-interactive shell
sudo useradd -s /sbin/nologin john

Step 3: Verify user shell
getent passwd john


Expected output:

john:x:UID:GID::/home/john:/sbin/nologin

Step 4: Validate login restriction
su - john


Expected:

This account is currently not available.

Result

User john was successfully created with a non-interactive shell.


Save the file (**CTRL + S**).

---

# ✅ Part 4: Commit using VS Code Git Tool (NO terminal)

### 1️⃣ Open Source Control
- Click the **Source Control icon** (🔀) on the left sidebar  
  OR  
- Press:
```text
Ctrl + Shift + G
