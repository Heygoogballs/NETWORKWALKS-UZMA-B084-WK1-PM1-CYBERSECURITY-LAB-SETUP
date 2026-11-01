# 🔐 Cybersecurity Lab Setup
### NetworkWalks Cybersecurity Program | Week 1 | Project PM1

## 📌 Project Overview

This project documents the setup of a virtual cybersecurity laboratory using Oracle VirtualBox and Kali Linux.

The aim was to create a controlled environment for practising network analysis, cybersecurity investigations, vulnerability assessment and ethical hacking techniques.

The environment uses a private NAT Network, allowing virtual machines to communicate within the lab.

## 🎯 Project Objectives

- Install and configure Oracle VirtualBox.
- Set up Kali Linux as a virtual machine.
- Create a dedicated NAT Network.
- Configure the Kali Linux network adapter.
- Verify IP addressing and connectivity.
- Prepare the environment for future cybersecurity investigations.
- Document the configuration and troubleshooting process.

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| Oracle VirtualBox | Virtualisation platform |
| Kali Linux | Cybersecurity testing environment |
| Windows 11 | Host operating system |
| NAT Network | Virtual machine connectivity |
| Linux Terminal | Network configuration and testing |

## 🖥️ Lab Environment

| Component | Configuration |
|-----------|---------------|
| Host operating system | Windows 11 |
| Virtualisation platform | Oracle VirtualBox |
| Security operating system | Kali Linux |
| Virtual network | NAT Network |
| Kali Linux IP | 10.0.0.4 |
| Target VM IP | 10.0.0.5 |
| Network range | 10.0.0.0/24 |

## 🪜 Lab Setup Procedure

### Step 1: Install Oracle VirtualBox

Installed Oracle VirtualBox to create and manage virtual machines on my computer.

VirtualBox provides an isolated environment for practising cybersecurity techniques without directly affecting the host operating system.

**Evidence:** Screenshot of VirtualBox installed and running.

### Step 2: Set Up Kali Linux

Imported and configured Kali Linux in VirtualBox.

Kali Linux provides tools commonly used for cybersecurity investigations, network analysis and penetration testing.

**Evidence:** Screenshot of the Kali Linux virtual machine running.

### Step 3: Configure the NAT Network

Created a NAT Network in VirtualBox using the following network range:

`10.0.0.0/24`

The NAT Network allows virtual machines connected to the same network to communicate.

**Evidence:** Screenshot showing the NAT Network configuration.

### Step 4: Configure Kali Linux Networking

Connected the Kali Linux virtual network adapter to the NAT Network.

Checked the network configuration to identify the IP address assigned to Kali Linux.

**Observed Kali IP address:** `10.0.0.4`

**Evidence:** Screenshot showing the network adapter settings and Kali Linux IP address.

### Step 5: Configure the Target Virtual Machine

Configured a target virtual machine for authorised cybersecurity testing.

The target machine was connected to the same NAT Network as Kali Linux.

**Observed target IP address:** `10.0.0.5`

**Evidence:** Screenshot showing the target VM configuration.

### Step 6: Test Network Connectivity

Verified network communication between Kali Linux and the target machine.

The objective was to confirm that both virtual machines could communicate before beginning security investigations.

**Evidence:** Screenshot of the connectivity test.

## 🔧 Troubleshooting Experience

During the setup, I encountered difficulty understanding the difference between NAT and NAT Network configurations in VirtualBox.

I investigated the network adapter settings and checked how the virtual machines were connected.

This helped me understand that virtual machines must be attached to the appropriate network for the intended communication to work.

## 💡 What I Learned

This project strengthened my understanding of:

- Virtualisation and isolated testing environments.
- Configuring virtual machines in VirtualBox.
- The difference between NAT and NAT Network.
- IPv4 addressing and private networks.
- Verifying network connectivity.
- Troubleshooting virtual machine network settings.
- The importance of documenting technical configurations.

## 🔒 Security and Ethical Considerations

This environment was created for educational purposes and authorised cybersecurity practice only.

All security investigations should be performed on systems that I own or have explicit permission to test.

## 📚 Training Information

**Programme:** NetworkWalks Cybersecurity Program

**Batch:** B084

**Week:** 1

**Project:** PM1 – Cybersecurity Lab Setup
