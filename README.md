# ufw_configuration.sh
set up a basic firewall using UFW on a linux system
Objective

The objective of this task is to set up a basic firewall using UFW (Uncomplicated Firewall) on a Linux system. The firewall is configured to allow SSH traffic while denying HTTP traffic, ensuring secure access to the system.

Tools Used
UFW (Uncomplicated Firewall)

Steps Performed
1. Install UFW

sudo apt update
sudo apt install ufw

This installed the firewall package on the system.

2. Allow SSH traffic

sudo ufw allow ssh

SSH (port 22) was allowed to ensure remote access to the system.

3. Deny HTTP traffic

sudo ufw deny http

HTTP (port 80) traffic was blocked to prevent unauthorized web access.

4. Enable the firewall

sudo ufw enable

The firewall was activated and set to start automatically on system boot.

5. Check firewall status

sudo ufw status verbose

Confirmed that:

SSH (port 22) is allowed

HTTP (port 80) is denied

screenshot
<img width="922" height="504" alt="inten task2 ed" src="https://github.com/user-attachments/assets/db7a5de5-8bc8-4080-b3eb-fa6b24e60dfe" />

Result

The firewall is now active and configured correctly:

Incoming SSH connections are allowed.

Incoming HTTP connections are blocked.

All other traffic follows the default UFW policy.
