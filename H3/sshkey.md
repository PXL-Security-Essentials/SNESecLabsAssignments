# Protect SSH Lab
In this lab, you will secure an SSH server by replacing password-based authentication with public-key authentication.

You will work from a Kali Linux machine and configure the SSH server so that you can authenticate using a private key instead of a username and password.

## Overview of commands and files

Here is an overview of the commands and files you will use during this lab. Replace `x.x.x.x` with the IP address of your challenge, `username` with the username provided in the lab, and `nameofkey` with the name you used when running `ssh-keygen`.

| Command / File | Description |
| --- | --- |
| `ssh-keygen` | Generates a public/private SSH key pair on your local host. |
| `ssh-copy-id -i nameofkey username@x.x.x.x` | Copies the public key to the SSH server so the user can authenticate without a password. |
| `ssh -i nameofkey username@x.x.x.x` | Connects to the SSH server using the specified private key and username for authentication. |
| `sudo systemctl restart ssh` | Reloads the OpenSSH server configuration after changes are made to `sshd_config`. |
| `~/.ssh/authorized_keys` | The file on the server that stores the authorized public keys used for SSH authentication. |
| `sshd_config` | The SSH server configuration file where you can change authentication and security settings. |

## Goal

### 1. Generate an SSH key pair
On your Kali Linux machine, create a public/private SSH key pair. Keep the private key secure and do not transfer it to the SSH server. During key generation, configure a passphrase. A passphrase adds an extra layer of security: even if your private key is stolen, an attacker will still need the passphrase before they can use it to authenticate.

### 2. Configure public-key authentication
Transfer the public key to the SSH server using `ssh-copy-id`.

### 3. Test SSH authentication
Connect to the SSH server using your private key.

- `ssh -i nameofyourkey PXL@x.x.x.x`

If prompted for credentials, use:

- **Username:** `PXL`
- **Password:** `Xfactor!`

If you successfully copied the public key using `ssh-copy-id`, you will receive the first flag.

### 4. Check the public key
Open the file on the SSH server where the public key is stored. This file contains the second flag.

### 5. Disable password authentication
Harden the SSH configuration by allowing authentication only through the public/private key pair. Use `nano` to edit the `sshd_config` file and disable password-based login.

Save the changes and restart the SSH service.

### 6. Test the SSH connection
Reconnect to the SSH server using your private key. If you configured password authentication correctly, you will receive the third flag.
