# Telnet

During a penetration test, you discovered a Telnet server that is accessible over the network. This SecLab challenge was completed as a class exercise during Week 2 of the course.

## Challenge
Your goal is to gain access to the telnet server using **Hydra** and then access the files stored on the server.

## Prerequisites
Before starting:
1. Enable **ProtonVPN**.
  Hydra can generate a large amount of repeated network traffic, which may trigger firewall protections. Using a VPN routes your Hydra traffic through the VPN tunnel.
2. Run the Hydra command from **Kali Linux**.
3. Use **Kali Linux** to connect to and access the Telnet server.

> #### Configure and connect to the VPN
>
> All information on how to configure and connect to the VPN: [SecLabs - Proton VPN](https://pxl-student:2025_PXL!@pxl-securityessentials-sne.code-coaching.dev/cursus/0-labsetup/vpn.html)

### Goal
1. Use Hydra on Kali Linux to obtain the Telnet credentials.
2. Connect to the Telnet server and download the files available on the server.

Download and use the following password list [telnet challenge - passwordlist](https://raw.githubusercontent.com/PXL-Security-Essentials/SNESecLabsAssignments/refs/heads/main/H1/telnetpwdlist.txt)

**Hint:**
The telnet username is `admin`.

> #### Hydra syntax
>
> Check the online course for an example of the Hydra syntax: [Security Essentials Course - Hydra](https://pxl-student:2025_PXL!@pxl-securityessentials-sne.code-coaching.dev/cursus/1-cybersecurityconcepts/hydra.html)

### Telnet Commands

Once you have the correct credentials, you can use the following commands to interact with the Telnet server:
- **Connect to the telnet server:**

  ```bash
  telnet x.x.x.x
  ```

- **List the files on the server:**

  ```bash
  ls
  ```

- **Open a file:**

  ```bash
  cat file.txt
  ```