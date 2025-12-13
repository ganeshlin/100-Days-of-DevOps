# Day 02 – Create Temporary User with Expiry Date (xFusionCorp)

## Task
As part of the Nautilus project, a temporary user account was required for a developer
with time-bound access.

## Requirements
- User name: kareem (lowercase)
- Server: App Server 2
- Expiry date: 2024-01-28

## Solution

### Step 1: Connect to App Server 2
```bash
ssh stapp02

Step 2: Create user with expiry date
sudo useradd -e 2024-01-28 kareem

Step 3: Verify account expiry
sudo chage -l kareem


Expected output:

Account expires : Jan 28, 2024

Step 4: Verify user creation
getent passwd kareem

Result

Temporary user kareem was successfully created with an expiry date.