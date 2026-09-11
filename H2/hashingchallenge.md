# Hashing Challenge
You have obtained the credentials for a server. Connect to the server, locate the password hashes, crack them, and validate your results.

### Goal

1. Connect to the server via SSH.
2. Find out where the password hashes for the local Linux users are stored.
3. Use Hashcat to crack the hashes with the following wordlist: [Hashing Challenge - passwordlist](https://raw.githubusercontent.com/PXL-Security-Essentials/SNESecLabsAssignments/refs/heads/main/H2/leakedpassdb.txt).
4. Navigate to the password verification page at [http://x.x.x.x:8080](http://x.x.x.x:8080), replacing `x.x.x.x` with the IP address provided above.
5. If the password is correct, you will receive a flag. Enter the flag below.


> #### Hashcat syntax
> The online course provides a comprehensive explanation of how to use Hashcat, including practical examples: [Security Essentials Course - Hashcat](https://pxl-student:2025_PXL!@pxl-securityessentials-sne.code-coaching.dev/cursus/2-hashing/hashcat.html)
