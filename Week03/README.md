# Week 03 — Enterprise Server Deployment and Operating System Installation

## Project Overview

This Week 03 portfolio project focuses on the deployment and configuration of an enterprise Linux server for **ABC Startup Solutions**.

The project involves installing **Ubuntu Server LTS** in a virtual machine, configuring essential server settings, enabling secure remote administration through SSH, verifying server functionality, comparing BIOS and UEFI firmware technologies, documenting the Ubuntu boot process, installing Windows Server Evaluation, and comparing Windows Server, Ubuntu Server, and Rocky Linux.

This project demonstrates foundational System Administration skills including virtualization, Linux server deployment, system configuration, verification, troubleshooting, technical documentation, and operating-system analysis.

> **Note:** Actual IP addresses, command results, and screenshots should be replaced with the results from the student's own virtual machine.

## Learning Objectives

By completing this project, I aim to:

- Explain the purpose of operating systems in enterprise environments.
- Differentiate between BIOS and UEFI firmware.
- Explain the stages of the computer boot process.
- Compare Ubuntu Server, Windows Server, and Rocky Linux.
- Install Ubuntu Server in a virtual machine.
- Configure essential Linux server settings.
- Enable secure remote administration using SSH.
- Verify server functionality using Linux commands.
- Document an operating-system deployment professionally.
- Develop troubleshooting and system-administration skills.

## Virtual Machine Specifications

| Component | Configuration |
|---|---|
| Virtual Machine Name | `Ubuntu-Server-Week03` |
| Operating System | Ubuntu Server LTS |
| RAM | 4 GB |
| CPU | 2 Virtual Processors |
| Storage | 40 GB VDI/VMDK |
| Network | NAT |
| Optical Drive | Ubuntu Server ISO |
| Hostname | `server01` |
| SSH | OpenSSH Server |

## Installation Summary

The Ubuntu Server virtual machine was created using the required specifications. During installation, the following configurations were completed:

1. English was selected as the installation language.
2. The appropriate keyboard layout was configured.
3. Network configuration was set to DHCP unless otherwise instructed.
4. The hostname was assigned as `server01`.
5. A non-root administrative user was created.
6. Guided disk partitioning using the entire virtual disk was selected.
7. OpenSSH Server was enabled.
8. No additional packages were installed unless required.
9. The installation was completed and the server was restarted.

## Initial Configuration

The initial server configuration includes:

| Setting | Configuration |
|---|---|
| Hostname | `server01` |
| Network | DHCP / NAT |
| Storage | 40 GB |
| Administrative Access | Non-root user with `sudo` |
| Remote Administration | OpenSSH Server |

## Server Verification

The server was verified using the following procedures:

| Verification | Command | Expected Result |
|---|---|---|
| Hostname | `hostname` | `server01` |
| IP Address | `ip addr` | Assigned IP address displayed |
| Internet Connectivity | `ping -c 4 google.com` | Successful replies |
| Package Update | `sudo apt update` | Package information updated |
| Package Upgrade | `sudo apt upgrade -y` | Available updates installed |
| SSH Service | `systemctl status ssh` | `active (running)` |

### Evidence

Screenshots are stored in the `screenshots/` directory.

Recommended evidence:

- VM configuration
- Ubuntu language selection
- Keyboard configuration
- Network configuration
- Hostname configuration
- User account configuration
- Disk partition configuration
- OpenSSH installation
- Successful login
- `hostname` command
- `ip addr` command
- Internet connectivity test
- System update
- SSH service status

## BIOS vs UEFI Highlights

| Category | BIOS | UEFI |
|---|---|---|
| Definition | Traditional firmware interface | Modern firmware interface |
| Partition Style | Commonly MBR | Commonly GPT |
| Disk Support | Traditionally limited by MBR | Supports very large disks with GPT |
| Security | Limited built-in security | Supports features such as Secure Boot |
| Boot Management | Legacy boot process | Modern boot manager |
| Modern Usage | Mostly legacy systems | Standard on modern computers |

UEFI has largely replaced BIOS because modern systems require support for larger storage devices, modern partitioning schemes, improved boot management, and stronger security features. UEFI works well with GPT and provides features such as Secure Boot.

## Ubuntu Boot Process

The Ubuntu Server boot sequence documented in this project is:

```text
Power On
    ↓
BIOS / UEFI Initialization
    ↓
Boot Device Detection
    ↓
Boot Loader (GRUB)
    ↓
Linux Kernel
    ↓
init / systemd
    ↓
Services Start
    ↓
Login Prompt
```

### Boot Process Flowchart

The completed flowchart is stored in the `diagrams/` directory.


The exported PDF version should also be submitted according to the Week 03 requirements.

## Windows Server Installation Summary

For the bring-home activity, Windows Server Evaluation is installed in a separate virtual machine.

The required tasks are:

- Install Windows Server Evaluation.
- Assign a computer name.
- Create an administrator password.
- Log in successfully.
- Capture screenshots of the installation.


## Operating System Comparison

| Feature | Windows Server | Ubuntu Server | Rocky Linux |
|---|---|---|---|
| Licensing | Proprietary / commercial | Open-source | Open-source |
| User Interface | GUI available | Primarily command-line/server focused | Primarily command-line/server focused |
| Package Management | Windows Update and Windows package mechanisms | APT / `.deb` | DNF / RPM |
| Security | Microsoft enterprise security ecosystem | Linux permissions, SSH, firewall and security tools | SELinux, Linux permissions, firewall and security tools |
| Typical Enterprise Use | Active Directory, Microsoft workloads, file/print services | Web, cloud, databases, development, infrastructure | Enterprise Linux workloads and RHEL-compatible environments |
| Advantages | Strong Microsoft ecosystem integration | Flexible, open-source, widely used for servers | Enterprise-oriented Linux platform |
| Disadvantages | Licensing and resource considerations | Requires Linux administration knowledge | Requires Linux administration knowledge |

## Challenges Encountered

Potential challenges during the deployment included:

- Configuring the virtual machine correctly.
- Selecting the correct network configuration.
- Identifying the assigned IP address.
- Verifying Internet connectivity.
- Confirming that OpenSSH Server was installed and running.
- Understanding the relationship between firmware, bootloader, kernel, and system services.

## Troubleshooting

| Problem | Possible Cause | Solution |
|---|---|---|
| VM does not start | Incorrect ISO or VM configuration | Check VM settings and ISO attachment. |
| No network connection | Incorrect virtual network adapter | Verify NAT or Bridged configuration. |
| SSH unavailable | SSH not installed or running | Check `systemctl status ssh` and OpenSSH installation. |
| Incorrect hostname | Configuration error | Verify using `hostname`. |
| `apt update` fails | Network or DNS issue | Test connectivity and check network configuration. |
| Cannot log in | Incorrect credentials | Verify username and password. |
| Boot problem | Firmware or bootloader issue | Check BIOS/UEFI boot order and GRUB configuration. |

## Best Practices

- Use a strong administrative password.
- Avoid routine root-account usage.
- Use SSH for secure remote administration.
- Keep the server updated.
- Install only required packages.
- Maintain reliable backups.
- Document configuration changes.
- Apply appropriate access-control and security policies.
- Keep technical documentation updated.
- Verify services after configuration changes.

## Technologies Used

- Ubuntu Server LTS
- Oracle VirtualBox or VMware Workstation
- OpenSSH
- Linux command-line utilities
- BIOS / UEFI
- GRUB
- systemd
- Windows Server Evaluation
- Rocky Linux
- GitHub
- Draw.io or another diagramming tool

## Repository Structure

```text
BSIT-SystemAdministration-Portfolio/
│
├── Week03/
│   ├── InstallationGuide.pdf
│   ├── ProfessionalInstallationManual.pdf
│   ├── BIOS_vs_UEFI.pdf
│   ├── BootProcessFlowchart.pdf
│   ├── screenshots/
│   ├── diagrams/
│   ├── README.md
│   └── references/
```

## Portfolio Deliverables

- [ ] Ubuntu Server installed
- [ ] Hostname configured
- [ ] Keyboard configured
- [ ] Disk partition configured
- [ ] SSH installed and running
- [ ] Login verified
- [ ] Internet connectivity verified
- [ ] System updated
- [ ] BIOS vs UEFI comparison completed
- [ ] Boot process flowchart completed
- [ ] Windows Server Evaluation installed
- [ ] Windows Server vs Ubuntu Server vs Rocky Linux comparison completed
- [ ] Installation Guide completed
- [ ] Professional Installation Manual completed
- [ ] Screenshots added
- [ ] README.md completed
- [ ] GitHub repository updated
- [ ] LinkedIn reflection posted

## Reflection

This project helped me understand the practical process of deploying an enterprise server from the beginning. I learned that installing an operating system is only one part of system administration. A server also needs correct network, storage, hostname, user-account, remote-access, and update configurations before it can be considered ready for use.

Working with Ubuntu Server improved my confidence with Linux command-line administration. Commands such as `hostname`, `ip addr`, `ping`, `apt`, and `systemctl` provide useful ways to verify whether a server is configured and operating correctly. I also learned that verification should be performed after installation instead of assuming that a successful installation automatically means that every service is working.

The BIOS and UEFI comparison gave me a better understanding of the technologies involved before an operating system starts. Learning the sequence from firmware initialization to boot-device detection, GRUB, the Linux kernel, systemd, services, and the login prompt helped me understand how administrators can approach boot-related troubleshooting.

Another important lesson was the value of technical documentation. A professional installation guide allows another administrator to reproduce the same configuration without depending on the original administrator's memory. Documentation also provides evidence that configuration and verification tasks were completed.

The most challenging part of the project was connecting the theoretical concepts with the actual virtual-machine environment. Network configuration, SSH verification, and understanding the boot process required careful attention to each step. This helped develop a more systematic approach to troubleshooting.

Overall, Week 03 strengthened my foundational skills in Linux server deployment, virtualization, system verification, firmware concepts, troubleshooting, and technical documentation. These skills will be useful as I continue developing my capabilities as a System Administrator.

## References

- ITEP 414 – System Administration and Maintenance, Week 3 Portfolio Project: Enterprise Server Deployment and Operating System Installation.
- Ubuntu Server documentation for the Ubuntu Server LTS version used.
- Microsoft Windows Server documentation for the Windows Server Evaluation version used.
- Rocky Linux documentation for the release used in the operating-system comparison.
