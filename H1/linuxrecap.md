 # Linux recap

 In this challenge, you will connect to a Linux virtual machine using SSH. Your goal is to explore the system using basic Linux commands and locate **six flags**.

 ## SSH Connection

 Connect to the virtual machine using SSH with the following credentials:

 - **Username:** `admin`
- **Password:** `SecurityEssentials2026`

 ## Flag 1 — Admin Home Directory

 Start by exploring the home directory of the `admin` user.

 Your first flag is located somewhere in this directory.

 Use basic Linux commands to inspect the contents of the directory and locate the flag.

 ## Flag 2 — Hidden Files

 There is another flag hidden in the `admin` user's home directory.

 Linux files and directories whose names start with `.` are hidden by default.

 Inspect the `admin` home directory again, this time making sure that hidden files are also displayed.

 Locate and open the file containing the second flag.

 ## Flag 3 — Download a File

 Use `wget` to download the following file to the virtual machine:

```
https://raw.githubusercontent.com/PXL-Security-Essentials/SNESecLabsAssignments/refs/heads/main/H1/third.txt
```

 After downloading the file, inspect its contents to find the third flag.

 ## Flag 4 — Search with `find`

 The fourth flag is located somewhere under the `/var` directory.

 Use the Linux `find` command to search through `/var` and its subdirectories for a file named:

```
fourth.txt
```

 Once you locate the file, open it and retrieve the fourth flag.

 ## Flag 5 — Switch User

 Next, switch from the `admin` user to the `john` user.

 The credentials for `john` are:

 - **Username:** `john`
- **Password:** `SecurityEssentials2027`

 After switching users, verify which user you are currently logged in as.

 Once you have successfully switched to `john` and verified your current user, you will find the fifth flag.

 ## Flag 6 — John's Home Directory

 Finally, explore the home directory belonging to the `john` user.

 Use the basic Linux commands you have learned to inspect the directory and locate the final flag.

 ## Objective

 By the end of the challenge, you should have found **six flags**:

1. **Flag 1** — `admin`'s home directory
2. **Flag 2** — A hidden file in `admin`'s home directory
3. **Flag 3** — The downloaded `third.txt` file
4. **Flag 4** — `fourth.txt` somewhere under `/var`
5. **Flag 5** — After successfully switching to `john`
6. **Flag 6** — `john`'s home directory