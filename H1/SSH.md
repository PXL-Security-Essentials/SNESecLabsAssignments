# SSH
During a penetration test, you discovered an accessible SSH server.

## Challenge
Your goal is to gain access to the SSH server using **Hydra** and then access the files stored on the server.

## Prerequisites
Before starting:
1. Enable **ProtonVPN**.
   Hydra can generate a large amount of repeated network traffic, which may trigger firewall protections. Using a VPN routes your Hydra traffic through the VPN tunnel.
2. Run the Hydra command from **Kali Linux**.
3. Use **Kali Linux** to connect to and access the FTP server.

> #### Config and connect with VPN
> All information how to configure and connect with VPN: [SecLabs - Proton VPN](https://pxl-student:2025_PXL!@pxl-securityessentials-sne.code-coaching.dev/cursus/0-labsetup/vpn.html)
> 

### Goal
1.Use Hydra on Kali Linux to obtain the SSH credentials
2.Connect to the SSH server and look for files on the server.

Download and use the following password list [SSH challenge - passwordlist](https://raw.githubusercontent.com/PXL-Security-Essentials/SNESecLabsAssignments/refs/heads/main/H1/sshpwdlist.txt)

**Hint:**
During the previous challenge (FTP Hydra), you found a list of SSH usernames on the FTP server. Use this usernamelist as part of your Hydra attack.

> #### Hydra syntax
> Check the online course for an example of the Hydra syntax: [Security Essentials Course - Hydra](https://pxl-student:2025_PXL!@pxl-securityessentials-sne.code-coaching.dev/cursus/1-cybersecurityconcepts/hydra.html)
> 

### FTP Commands
Once you have the correct credentials, you can use the following commands to interact with the FTP server:
- **Connect to the SSH server:**

  ```bash
  ssh username@x.x.x.x
  ```
