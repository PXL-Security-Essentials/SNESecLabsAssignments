# FTP
During a penetration test, you discovered an FTP server that is accessible over the network.

## Challenge
Your goal is to gain access to the FTP server using **Hydra** and then access the files stored on the server.

The **Security Essentials** course covers the basic Hydra syntax and explains how to use the tool.

**Hint:**
The FTP username is `ftpadmin`.

## Prerequisites
Before starting:
1. Enable **ProtonVPN**.
   Hydra can generate a large amount of repeated network traffic, which may trigger firewall protections. Using a VPN routes your Hydra traffic through the VPN tunnel.
2. Run the Hydra command from **Kali Linux**.
3. Use **Kali Linux** to connect to and access the FTP server.

## FTP Commands
Once you have the correct credentials, you can use the following commands to interact with the FTP server:
- **Connect to the FTP server:**

  ```bash
  ftp x.x.x.x
  ```

- **List the files on the server:**

  ```bash
  ls
  ```

- **Download a file:**

  ```bash
  get file.txt
  ```

- **Exit the FTP session:**

  ```bash
  bye
  ```

### Goal

Use Hydra to obtain the FTP credentials, connect to the FTP server, and download the files available on the server.

