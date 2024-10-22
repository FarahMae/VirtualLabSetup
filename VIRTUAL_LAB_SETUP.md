# Virtual Lab Setup Guide

## Step-by-Step Guide to Setting Up a Virtual Lab with Kali Linux

### Step 1: Prepare Your Environment

1. **Check System Requirements**:
   - Ensure your computer has at least:
     - **8 GB of RAM** (more is better for multiple VMs).
     - **Dual-core CPU** or better.
     - **At least 100 GB of free disk space**.

2. **Download and Install Virtualization Software**:
   - **[VirtualBox](https://www.virtualbox.org/wiki/Downloads)** (free and open-source):
     - Go to the VirtualBox download page.
     - Download the version for your operating system (Windows, macOS, or Linux).
     - Follow the installation instructions.

### Step 2: Download Kali Linux and Other VMs

1. **Visit the NetAcad Website**:
   - Go to **[NetAcad Lab Downloads](https://www.netacad.com/resources/lab-downloads?courseLang=en-US)**.
   - Browse the available resources and find the VMs you wish to download, including Kali Linux.

2. **Download the VMs**:
   - Download the VMs to your local machine.
   - Note the location where the files are saved.

### Step 3: Set Up Kali Linux in VirtualBox

1. **Open VirtualBox**:
   - Launch the VirtualBox application.

2. **Create a New VM**:
   - Click on **"New"** to create a new virtual machine.
   - **Name**: Enter a name (e.g., "Kali Linux").
   - **Type**: Select **"Linux"**.
   - **Version**: Select **"Debian (64-bit)"**.
   - Click **"Next"**.

3. **Allocate RAM**:
   - Allocate at least **2 GB of RAM** (more if possible).
   - Click **"Next"**.

4. **Create a Virtual Hard Disk**:
   - Choose **"Create a virtual hard disk now"**.
   - Select **"VDI (VirtualBox Disk Image)"**.
   - Choose **"Dynamically allocated"**.
   - Set the size (recommended: at least **20 GB**).
   - Click **"Create"**.

5. **Configure VM Settings**:
   - Select your VM and click **"Settings"**.
   - Under **System**:
     - Adjust the boot order if necessary (set **Hard Disk** first).
   - Under **Storage**:
     - Click on **"Empty"** under **Controller: IDE**.
     - Click the disk icon on the right and select the downloaded Kali ISO file.
   - Under **Network**:
     - Ensure **Adapter 1** is enabled and set to **NAT** or **Bridged Adapter**.

6. **Start the VM**:
   - Click **"Start"** to boot the VM.
   - Follow the installation prompts for Kali Linux:
     - Choose **Graphical Install** and follow the on-screen instructions to set up the OS.

### Step 4: Set Up Additional VMs

1. **Repeat the Process**:
   - For each additional VM you downloaded, repeat Steps 3.1 to 3.6, adjusting settings as necessary for each operating system.

### Step 5: Networking Configuration

1. **Configure Networking**:
   - If you need networking between your VMs, go to **Settings** for each VM and configure the network settings:
     - Use **Internal Network** to allow VMs to communicate with each other.
     - Use **Bridged Adapter** if you want the VMs to connect to your local network.

### Step 6: Test Your Setup

1. **Start Each VM**:
   - Boot each VM to ensure they run correctly.

2. **Check Connectivity**:
   - Use `ping` commands or other network tools within the VMs to ensure they can communicate with each other.

### Step 7: Project Implementation

1. **Define Your Project**:
   - Outline the goals of your virtual lab (e.g., penetration testing, network security training).

2. **Document Your Steps**:
   - Keep a log of configurations, tests, and findings for future reference or project reports.

### Step 8: Snapshots and Backups

1. **Create Snapshots**:
   - After configuring each VM, take a snapshot in VirtualBox (Right-click on the VM > Snapshots > Take).

2. **Regular Backups**:
   - Backup your VM files periodically to avoid data loss.

### Additional Resources

- **[VirtualBox User Manual](https://www.virtualbox.org/manual/UserManual.html)**: For detailed configuration and usage tips.
- **[Kali Documentation](https://www.kali.org/docs/)**: For information on using Kali Linux effectively.
