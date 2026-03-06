*This project has been created as part of the 42 curriculum by aramos.*

# NetPractice

## Table of Contents

1.	[Description](#description)
2.	[Project Goals](#project-goals)
3.	[Installation](#installation)
4.	[Instructions](#instructions)
5.	[Usage](#usage)
6.	[Project Structure](#project-structure)
7.	[Networking Concepts Covered](#networking-concepts-covered)
8.	[Submission Requirements](#submission-requirements)
9.	[Troubleshooting](#troubleshooting)
10.	[Resources](#resources)
11.	[License](#license)

---

# Description

**NetPractice** is a project from the **42 curriculum** designed to introduce the fundamentals of computer networking and TCP/IP through practical exercises.

The project provides simulated network configurations that must be corrected in order to allow devices to communicate between them and/or the internet properly. Each exercise displays a network diagram with incorrect or incomplete parameters such as IP addresses, subnet masks, or gateways. The idea is to modify these values until the network functions correctly.

---

# Project Goals

The main objectives of this project are:

* Understand how **IP addressing** works.
* Learn how **subnet masks** define network ranges.
* Understand the role of a **default gateway** in routing traffic.
* Learn how devices communicate through **routers and switches**.
* Practice diagnosing and fixing networking configuration errors.
* Develop logical reasoning for network troubleshooting.

---

# Installation

1. Download the project archive from the NetPractice project page.
2. Extract the archive into a folder.

Example:

```bash
tar -xvf netpractice.tar
cd netpractice
```

---

# Instructions

## Running the Training Interface

The NetPractice exercises run through a local web interface.

### Method 1 — Using the provided script (recommended)

Run the following command inside the project folder:

```bash
./run.sh
```

This script will:

* Start a local web server
* Automatically open the NetPractice interface in your browser

### Method 2 — Running the server manually

If `run.sh` does not work, you can start the server manually:

```bash
python3 -m http.server 49242
```

Then open your browser and navigate to:

```
http://localhost:49242
```

You can use a different port if desired.

---

# Usage

Once the interface is open:

1. Enter your **login** in the login field.
2. Select a **training level** or use the **evaluation tab** for a random configuration.
3. Each level shows a **broken network diagram**.
4. Modify the **unshaded fields** (IP addresses, masks, gateways, etc.).
5. Click **Check again** to test if the configuration works.
6. When the configuration is correct, the next level will unlock.

Repeat this process for **all 10 levels**.

---

# Networking Concepts Covered

This project focuses on several fundamental networking concepts:

### TCP/IP Addressing

Understanding how devices identify themselves within a network using IPv4 addresses.

### Subnet Masks

Subnet masks determine which portion of an IP address refers to the network and which refers to the host.

Example:

```
IP Address:  192.168.1.10

                        Network portion
                         ^
                         |
Subnet Mask: 255.255.255.0
             |----------|
                  |
                  V
              Host portion
```

### Default Gateway

The **default gateway** allows devices to communicate with other networks through a router.

### Routers

Routers connect multiple networks together and forward packets between them.

### Switches

Switches connect multiple devices within the same network and forward frames using MAC addresses.

### OSI Model

Understanding how networking tasks are separated into layers, including:

1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

---

## Online Learning Resources

* https://www.cloudflare.com/learning/network-layer/what-is-an-ip-address/
* https://www.geeksforgeeks.org/computer-network-tutorials/
* https://developer.mozilla.org/en-US/docs/Glossary/TCP
* https://tryhackme.com/room/introtonetworking
* CompTIA A+, Network+ and Security+ Study Guide

## Concepts Studied in This Project

* TCP/IP addressing
* Subnet masks
* Default gateways
* Routers
* Switches
* Network routing
* OSI model layers
* Network troubleshooting

## AI Usage

AI tools were used in this project to assist with:

* Structuring the README documentation
* Clarifying networking concepts
* Improving explanations and formatting

All networking configurations and solutions were completed manually and verified to ensure full understanding of the concepts involved.

---

# License

This project is part of the **42 School curriculum** and is intended for educational purposes.

