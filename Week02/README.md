SK Digital Solutions – Enterprise Infrastructure Plan

Project Overview

This project presents an initial Enterprise IT Infrastructure Plan for SK Digital Solutions, a newly established software development company with 20 employees. The project focuses on planning the company's hardware, software, network infrastructure, system administration requirements, security, backup strategy, and future expansion.

The goal is to create a reliable and organized IT infrastructure that supports the daily operations of the company.

Learning Objectives

Through this project, I learned how to:

* Analyze organizational IT requirements.
* Prepare professional hardware, software, and network inventories.
* Design an enterprise network topology.
* Identify the responsibilities of different system administration roles.
* Develop practical infrastructure recommendations.
* Create technical documentation using Markdown.
* Plan security, backup, and future infrastructure expansion.

Company Scenario

SK Digital Solutions is a newly established software development company operating from a single office floor.

The company has 20 employees distributed among four departments:

| Department             | Employees |
| ---------------------- | --------: |
| Information Technology |         5 |
| Human Resources        |         4 |
| Finance                |         5 |
| Sales                  |         6 |
| **Total**              |    **20** |

The company initially has no computers, server, network, Internet infrastructure, or security policies. Therefore, the entire IT infrastructure must be planned and designed from the beginning.

Hardware Inventory Summary

The proposed hardware infrastructure includes:

| Hardware               | Quantity |
| ---------------------- | -------: |
| Desktop Computers      |       16 |
| Laptop Computers       |        4 |
| Server                 |        1 |
| Router                 |        1 |
| Managed Network Switch |        1 |
| Network Printers       |        2 |
| UPS                    |        2 |
| Wireless Access Points |        3 |
| NAS Storage            |        1 |
| External Backup Drives |        2 |
| Monitors               |       20 |

The hardware inventory provides computing devices for all 20 employees and establishes the necessary server, networking, printing, storage, and backup infrastructure.

Software Inventory Summary

The proposed software environment includes:

| Software           | Main Purpose                         |
| ------------------ | ------------------------------------ |
| Windows 11 Pro     | Employee operating system            |
| Ubuntu Server      | Server operating system              |
| Microsoft Office   | Business productivity                |
| Visual Studio Code | Software development                 |
| Git                | Version control                      |
| GitHub Desktop     | Git/GitHub management                |
| VirtualBox         | Virtual machine testing              |
| Google Chrome      | Web browsing and application testing |
| Microsoft Defender | Endpoint security                    |
| AnyDesk            | Remote technical support             |
| 7-Zip              | File compression and extraction      |

These software items correspond to the software requirements specified in the Week 2 module.

Network Inventory Summary

The proposed network infrastructure includes:

| Network Equipment      |    Quantity |
| ---------------------- | ----------: |
| ISP Modem/ONT          |           1 |
| Router                 |           1 |
| Firewall               |           1 |
| Managed Switch         |           1 |
| Wireless Access Points |           3 |
| Patch Panel            |           1 |
| CAT6 Cable             | 1 bulk roll |
| RJ45 Connectors        |         100 |

The network is designed to provide secure and reliable connectivity for all departments and infrastructure devices.

Enterprise Network Diagram

The network follows this general topology:

```text
                         INTERNET
                             |
                      [ ISP MODEM/ONT ]
                             |
                         [ ROUTER ]
                             |
                        [ FIREWALL ]
                             |
                    [ MANAGED SWITCH ]
                      /      |      \
                     /       |       \
                [SERVER]   [NAS]   [PRINTER]
                                   
                             |
                    [WIRELESS ACCESS POINTS]
                       /       |       \
                      /        |        \
                    IT         HR       FINANCE
                                         |
                                       SALES
```

The complete network diagram should be saved in the `diagrams/` folder and exported as both PNG and PDF, as required by the module.

![Enterprise Network Diagram](diagrams/network-diagram.png)

System Administration Roles

The project covers four important IT roles:

1. Helpdesk Technician – Provides first-level technical support and troubleshooting.
2. Network Administrator – Manages network connectivity, routers, switches, wireless infrastructure, and network security.
3. Linux System Administrator*– Manages Linux servers, users, permissions, services, and system security.
4. Cloud Administrator – Manages cloud infrastructure, services, storage, access, and cloud security.

These professionals work together to maintain reliable IT operations within the organization.

Infrastructure Recommendations

The recommended infrastructure for SK Digital Solutions includes:

* Business-grade fiber Internet with approximately 300–500 Mbps.
* A dedicated server with 32 GB ECC RAM and RAID 1 storage.
* A 3-2-1 backup strategy.
* Firewall and endpoint security.
* Strong password policies and multi-factor authentication.
* Regular system updates and backups.
* Infrastructure designed for future expansion.

These recommendations are intended to provide a secure, reliable, and scalable foundation for the company's current 20 employees.

Technologies Used

The project uses or proposes the following technologies:

* Windows 11 Pro
* Ubuntu Server
* Microsoft Office
* Visual Studio Code
* Git
* GitHub Desktop
* VirtualBox
* Google Chrome
* Microsoft Defender
* AnyDesk
* 7-Zip
* TCP/IP networking
* CAT6 Ethernet
* Gigabit Ethernet
* Wireless networking
* Draw.io
* GitHub

Challenges Encountered

The main challenges encountered during the project were determining appropriate hardware quantities, selecting suitable software, designing the network topology, and ensuring that the proposed infrastructure could support both current requirements and future expansion.

Designing the network was particularly challenging because the Internet connection, firewall, router, switch, server, wireless access points, printers, and departments needed to be connected logically.

Reflection

This project taught me that proper infrastructure planning is essential before deploying an organization's IT systems. I learned how to identify hardware and software requirements, design a network, plan security and backups, and document technical decisions.

The project also improved my understanding of how different system administration roles work together. Most importantly, I learned that a System Administrator should plan proactively rather than only respond to problems after they occur.


Prepared for: ITEP 414 – System Administration and Maintenance
Project: Week 2 Portfolio Project
Company: SK Digital Solutions
Prepared by: SK Briddon T. Dumlao
