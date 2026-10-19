# GnuPG
In this lab you will learn the gpg commandline tools to encrypt and decrypt data symmetric and assymetric
The online Security Essentials course has all the commands needed to complete the challenge:

## Connect to the lab environment

1. Open the lab environment at http://x.x.x.x:8080.
2. On the page that opens, enter your PXL student email address in this format: `firstname.lastname@student.pxl.be`.

## 1. Symmetric Decryption

1. Click the green button to download the encrypted file.
2. Copy the downloaded file, `SymmetricDecryption.txt.gpg`, to the home directory of your Kali Linux machine.
3. Decrypt the file using the GPG command-line tools. You will need the passphrase displayed on the online platform.
4. Open the decrypted file and copy its contents (plaintext) into the website.
5. If you have completed all the steps correctly, the first flag will be displayed.

## 2. Symmetric Encryption

1. Create a new text file on your own computer and name it `SymmetricChallenge.txt`.
2. Copy the text displayed in the challenge and paste it into `SymmetricChallenge.txt`. Make sure you do not add any extra characters, spaces, or line breaks.
3. Transfer the file `SymmetricChallenge.txt` to your Kali Linux machine.
4. Encrypt the file using the GPG command-line tools. Use the AES-256 algorithm and the provided passphrase.
5. Upload the encrypted file to the online platform.
6. If you have completed all the steps correctly, the second flag will be displayed.

## 3. Asymmetric Decryption

1. Generate a new GPG key pair in Kali Linux using the settings specified on the online platform.
2. Export the public key using the appropriate GPG command.
3. Transfer the exported public key to your own computer and upload it to the online platform.
4. Download the encrypted file, `AsymmetricDecryption.txt.gpg`, from the online platform.
5. Transfer `AsymmetricDecryption.txt.gpg` to your Kali Linux machine and decrypt it using the GPG command-line tools.
6. Open the decrypted file and copy the plaintext into the online platform.
7. If you have completed all the steps correctly, the third flag will be displayed.

## 4. Asymmetric Encryption

1. Create an empty text file on your own computer and name it `SeclabsAssymetric.txt`.
2. Copy the text displayed on the online platform and paste it into `SeclabsAssymetric.txt`. Make sure you do not add any extra characters, spaces, or line breaks.
3. Transfer the file `SeclabsAssymetric.txt` to your Kali Linux machine.
4. Download the public key from the online platform and place it in the home directory of your Kali Linux machine.
5. Open a terminal in Kali Linux and use the appropriate GPG command to import the public key.
6. Encrypt `SeclabsAssymetric.txt` using the imported public key. Specify `encryptionlabs@seclabs.be` as the recipient's email address.
7. Transfer the encrypted file, `SeclabsAssymetric.txt.gpg`, back to your own computer and upload it to the online platform.
8. If you have completed all the steps correctly, the fourth flag will be displayed.