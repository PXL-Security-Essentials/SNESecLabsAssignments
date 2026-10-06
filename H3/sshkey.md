# Protect SSH Lab
In this lab, you will secure an SSH server by replacing password-based authentication with public-key authentication.

You will work from a Kali Linux machine and configure the SSH server so that you can authenticate using a private key rather than a username and password.

## Goal

### 1.Generate an SSH key pair
On your Kali Linux machine, create a public and private SSH key pair. Keep the private key secure and do not transfer it to the SSH server.

### 2.Configure public-key authentication
Transfer the public key to the SSH server and place it in the appropriate location/configuration so that the server can use it to authenticate your user account.

### 3.Test SSH authentication
Connect to the SSH server using your private key. Verify that you can successfully authenticate without providing your account password.

The connection should use your private key and the appropriate user and server address.

### 4.Disable password authentication
Once public-key authentication has been successfully tested, modify the SSH server configuration to disable password-based login.

### 5.Test SSH connection
Reconnect to the SSH server to test your configuration.