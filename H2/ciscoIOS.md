# Cisco IOS Lab
In this challenge, you will connect to a Cisco IOS router via SSH using an account with limited privileges.

Once connected, retrieve the password hash of a higher-privileged user and attempt to crack it using the provided password list, ITadminpwlist.txt. After recovering the password, log in to the router via SSH using the higher-privileged account. Finally, erase the startup configuration and reboot the router.

## 1. SSH Connection

Connect to the virtual Cisco IOS router via SSH using the following credentials:

- **Username:** `readonly`
- **Password:** `readonly`

## 2. Retrieve the Hash

Once connected to the Cisco IOS CLI, run a command to display the password hashes for the users on the system. Identify the username and hash belonging to the higher-privileged user.

## 3. Crack the Hash

Use Hashcat and the provided password list to crack the higher-privileged user's hash.

Download the password list here: [ITadminpwlist.txt](https://raw.githubusercontent.com/PXL-Security-Essentials/SNESecLabsAssignments/refs/heads/main/H2/ITadminpwlist.txt)

## 4. Log In with the Higher-Privileged Account

Once you have recovered the higher-privileged user's password, connect to the virtual Cisco IOS router via SSH using that account. You will receive the first flag.
