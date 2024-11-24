# Standard Operating Procedure (SOP): How to Set Up a Windows Server

**Company Name:** Himsha  
**Company Address:** 130 Henlow Bay, Manitoba  
**Phone Number:** 204-730-3494 
**Version:** 1.0  
**Written by:** Himanshu  
**Approved by:** Felix 
**Date:** 11/24/2024

---

## Purpose
This document is here to help to set up a Windows Server. To setup server, follow the steps carefully to make sure everything works right. This guide covers everything from installing Windows Server to setting up basic features. It is a step-by-step recipe to get your server up and running.

## Who Should Use This?
This guide is for IT people who are setting up new servers. You should use this when setting up a server for the first time or if you need to install a fresh copy of Windows Server. If you’re unsure or new to servers, this document is for you!

## Definitions
- **Windows Server**: A special version of Windows designed to run on computers that manage a network or perform important tasks like hosting websites or storing data.
- **Active Directory (AD)**: A system that helps manage users and devices in a network.
- **DNS**: Translates website names into IP addresses so computers can find each other.
- **DHCP**: Automatically gives devices an IP address when they connect to the network.

---

## Steps to Set Up Windows Server

### Step 1: Pre-Setup Stuff
1. **Check System Requirements**: Make sure the server hardware is good enough for Windows Server. You’ll need at least:
   - A 1.4 GHz 64-bit processor
   - 8 GB of RAM 
   - 80 GB or more free space on the hard drive
   - A network adapter (for internet and network connections)

2. **Prepare Installation Media**: Get your Windows Server installation ready on a USB or DVD.

---

### Step 2: Install Windows Server
1. **Boot from USB or DVD**: Plug in the installation media and restart the server. Set it to boot from USB/DVD in the BIOS settings.

2. **Select Your Language and Region**: Choose your language, region, and keyboard layout.

3. **Install Windows Server**: Click **Install Now** to start the installation.

4. **Enter Product Key**: If you have a product key, enter it when prompted. You can skip this by clicking i don't have product key.

5. **Choose Edition**: Pick the version of Windows Server you need (Standard or Datacenter, for example).

6. **Choose the Installation Drive**: Pick the drive to install Windows on. You can create partitions here if needed.

7. **Wait for Installation**: The installation will take a while. The server will restart a few times, so don’t worry if it reboots.

---

### Step 3: Set Up the Server
1. **Set an Admin Password**: After installation, you will be asked to set up an admin password. Make sure it is a strong one.

2. **Configure Network Settings**: 
   - Set a static IP address if needed.
   - Enter DNS servers if necessary.

3. **Give Your Server a Name**: Name the server something unique, like `Server01` or `FileServer`—whatever makes sense for your setup.

4. **Activate Windows**: If you didn’t enter the product key earlier, do it now to activate Windows.

---

### Step 4: Add Roles and Features
1. **Open Server Manager**: Once everything is installed, open **Server Manager** from the Start menu.

2. **Add Roles and Features**: Click on **Manage** > **Add Roles and Features**. Follow the wizard to install important roles like:
   - **Active Directory** if you want to manage users
   - **DNS** if the server will handle name resolution
   - **DHCP** if the server will assign IP addresses to other devices

3. **Configure Active Directory**: If you are setting up Active Directory (AD), you will need to promote the server to a Domain Controller and create a new domain or join an existing one.

4. **Set Up DNS**: If you chose to install DNS, configure it so the server can resolve domain names.

---

### Step 5: Finalize the Setup
1. **Install Windows Updates**: After the server is running, go to **Windows Update** and install all the latest updates to keep things secure.

2. **Set Up the Firewall**: Make sure the server firewall is configured to allow the necessary services but block unnecessary ones.

3. **Install Antivirus Software**: If not already installed, add antivirus software to secure the server.

4. **Create User Accounts**: Create user accounts in Active Directory and assign appropriate roles and permissions.

5. **Test the Server**: 
   - Check network connectivity.
   - Test if DNS and DHCP are working properly.
   - Ensure the server can join the domain and authenticate users.

---

## Resources
- [Windows Server Documentation](https://docs.microsoft.com/en-us/windows-server/)
- [Active Directory Setup Guide](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview)
- [Windows Server Updates](https://learn.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh852339(v=ws.11))
- [Server Hardware Requirements](https://docs.microsoft.com/en-us/windows-server/get-started/hardware-requirements)


---

**End of SOP**
