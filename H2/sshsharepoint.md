1. Locate the SSH key in the document library on the SharePoint site. This key can be used to connect to the server via SSH; however, it is protected by a passphrase.
2. Check the SharePoint site for hints or clues regarding the password's format.
3. Use John the Ripper to extract the hash from the SSH key.
4. Next, use Hashcat to crack the extracted hash.
5. Finally, log in to the SSH server using the SSH key and the recovered passphrase.

Access the virtuel Sharepoint environment by:
- http://x.x.x.x:8080
- username: M365Admin@nodecraft.be
- password: NodeCraft3!
