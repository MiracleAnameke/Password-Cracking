# Password Cracking

## Introduction
This lab exercise delves into password cracking, focusing on understanding and using tools like John the Ripper and LC6 to crack passwords. You will set up a Windows 7 virtual machine and use various methods to attempt to crack the passwords of several user accounts, learning about the effectiveness and limitations of different password cracking techniques.

## Before You Begin
- Ensure you have a Windows 7 virtual machine (VM) ready.
- Download and install necessary password cracking tools: John the Ripper and LC6.
- Understand the ethical implications and legal context of password cracking - this is an educational exercise and should only be performed in a controlled, authorized environment.

## Setting Up the Lab
1. **Prepare the VM**: Launch the Windows 7 VM, ensuring all necessary tools and files are accessible.
2. **Folder Setup**: Create a dedicated folder named `pwd` off the root of the C drive to hold files and tools related to password cracking.

## Lab Procedure & Screenshots

### PART A – John the Ripper

#### Initial Setup
- Prepare the password file using pwdump7 and store it as `pwdcrack` containing the password hashes.
- Move or copy the `pwdcrack` file into the John the Ripper folder.

#### Cracking Passwords
- Run John the Ripper on the password file to attempt to crack the passwords.
- Observe and record the process, noting any successfully cracked passwords.

**Screenshot 1**: Take a screen capture of the list of username and password hashes.
<img src="https://i.imgur.com/cFTCn74.png" height="400px" width="auto" alt="List of Username and Password Hashes"/>

**Screenshot 2**: Take a screen capture of the list of passwords that have been cracked by John the Ripper.
<img src="https://i.imgur.com/MGZ0l0T.png" height="400px" width="auto" alt="Passwords Cracked by John the Ripper"/>

### PART B – LC6

#### Initial Setup
- Install LC6 from the provided setup file and initiate the password cracking process.

#### Password Cracking with LC6
- Run LC6 and observe the passwords being cracked.
- Explore various cracking methods available in LC6 including dictionary, hybrid, or brute force cracking.

**Screenshot 3**: Take a screen capture of the list of passwords that have been cracked by LC6.
<img src="https://i.imgur.com/MFG7oKO.png" height="400px" width="auto" alt="Passwords Cracked by LC6"/>

**Screenshot 4**: Take a screen capture of the password cracking options available in LC6.
<img src="https://i.imgur.com/clI4GFo.png" height="400px" width="auto" alt="Password Cracking Options in LC6"/>

### PART C - Local Security Policy

#### Security Policy Adjustment
- Modify the Local Security Policy to not store LAN Manager HASH values and observe its effect on password cracking.
- Change a user's password and use LC6 to crack it, noting the difference in cracking complexity when LAN Manager Hash is not stored.

**Screenshot 5**: Take a screen capture of the list of passwords cracked with the modified security policy.
<img src="https://i.imgur.com/ddR1ZPk.png" height="400px" width="auto" alt="Passwords Cracked with Modified Security Policy"/>

## Conclusion
This lab provides hands-on experience with password cracking tools, demonstrating the process of cracking and the effectiveness of various methods. It emphasizes the importance of strong, complex passwords and the role of security policies in protecting user accounts. Always ensure to conduct such exercises within ethical boundaries and legal frameworks.

