# SharePoint SSH access
Access the SharePoint environment to find the username and SSH private key required to connect to the SSH server. The private key is protected by a passphrase. Extract its hash, recover the passphrase, and use the key to log in to the SSH server.

## SharePoint access

Connect to the virtual SharePoint environment using these credentials:
- **URL:** `http://x.x.x.x:8080`
- **Username:** `M365Admin@nodecraft.be`
- **Password:** `NodeCraft3!`

## Goal
1. Find the SSH username on the SharePoint server.
2. Locate the SSH private key in the SharePoint site's document library.
3. Use John the Ripper to extract the passphrase hash from the private key.
4. Look for hints on the SharePoint site about the passphrase's format.
5. Use Hashcat and the identified format to recover the passphrase.
6. Log in to the SSH server with the private key and recovered passphrase.
