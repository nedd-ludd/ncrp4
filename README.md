# Raspberry Pi 4 - Home Server with Nextcloud

## Contents

[Project Overview](#project-overview) |
[Project Background](#project-background) |
[Getting Started](#getting-started) |
[Testing](#testing) |
[Project Brief & Timeframe](#project-brief) |
[Technologies Used](#technologies-used) |
[Result](#result) |
[Development Lifecycle](#development-lifecycle) |
[Wins](#wins) |
[Challenges](#challenges) |
[Bugs & Future Improvements](#bugs-and-future-improvements) |
[Key Learnings](#key-learnings) |
[Supporting Info](#supporting-info)

# Project Overview

This project involves setting up a self-hosted cloud computing solution using a Raspberry Pi 4 and Nextcloud. The server aims to centralise file storage, calendars, and task management while prioritising privacy and open-source principles. 

<span style="color:red">**GOAL-FOCUSED ALERT:**</span>  
This README documents the journey and setup process for others interested in replicating or learning from this endeavour.

![Diagram Placeholder](images/architecture.png)  
Basic architecture of the setup.

# Project Background

The motivation for this project stems from the increasing cost and data privacy concerns of commercial cloud storage solutions. By leveraging affordable hardware and open-source software, this project explores how to create a reliable and secure home cloud server. 

# Getting Started

To recreate this project, please follow the steps outlined below:

## Prerequisites

- Raspberry Pi 4 (or better) with a microSD card (32GB+ recommended)
- Power supply for Raspberry Pi
- External storage (USB drive or SSD)
- Static IP or dynamic DNS for remote access
- [Nextcloud software](https://nextcloud.com/install/)
- Relevant privileges for network and device setup

## Installation Steps

1. **Set up Raspberry Pi OS**:
   - Download Raspberry Pi OS and flash it to the microSD card using [Raspberry Pi Imager](https://www.raspberrypi.com/software/).
   - Enable SSH and configure Wi-Fi/network settings before booting.

2. **Install and Configure Nextcloud**:
   - Use `curl` or `wget` to download and install Nextcloud.
   - Configure storage paths for external drives.
   - Secure with HTTPS using `certbot` or similar.

3. **Set Up Git Repository**:
   - Clone the project repository:
     ```bash
     git clone https://github.com/yourusername/home-server-nextcloud.git
     ```
   - Commit project files (e.g., scripts, configs, and documentation).

4. **Configure Networking**:
   - Assign a static IP to the Raspberry Pi.
   - Forward relevant ports (e.g., 443 for HTTPS) on your router.
   - Optionally, configure dynamic DNS for remote access.

5. **Customise Features**:
   - Integrate calendars, tasks, and other apps via Nextcloud plugins.
   - Set up user accounts and permissions.

[Back to Top](#project-overview)

# Testing

1. **Basic Functionality**:
   - Verify local access to Nextcloud through the browser.
   - Test external access via dynamic DNS or static IP.

2. **Data Upload/Download**:
   - Upload files of varying sizes and verify download performance.

3. **Calendar & Task Syncing**:
   - Link with client apps (e.g., Thunderbird, iOS, Android).

4. **Error Logging**:
   - Use logs (`journalctl`, Nextcloud admin panel) to identify issues.

[Back to Top](#project-overview)

# Project Brief

## Goal

To create an open-source, self-hosted cloud server capable of securely managing files, calendars, and tasks for personal use.

## Functional Requirements

- Host files securely with user authentication.
- Enable calendar and task synchronisation.
- Provide web-based and mobile access.

## Non-Functional Requirements

- Maintain low power consumption.
- Minimise costs using free/open-source solutions.
- Ensure a reliable and intuitive user experience.

## Deliverables

- A fully configured Raspberry Pi server.
- A GitHub repository containing setup scripts and documentation.

## Timescale

Initial setup and testing: ~2 weeks, with ongoing improvements as needed.

[Back to Top](#project-overview)

# Technologies Used

| **Type**                     | **Technologies**              |
|-------------------------------|-------------------------------|
| **Operating Systems**         | Raspberry Pi OS              |
| **Server Software**           | Nextcloud                    |
| **Languages/Scripts**         | Bash, Python                 |
| **Networking Tools**          | Dynamic DNS, Port Forwarding |
| **Version Control**           | GitHub                       |

[Back to Top](#project-overview)

# Result

This section will outline the project's outcome, including screenshots of the functional Nextcloud interface and file syncing tests.

[Back to Top](#project-overview)

# Development Lifecycle

## Planning

- Research hardware and software requirements.
- Outline an iterative development plan focusing on MVP.

## Execution

- Install Raspberry Pi OS and ensure stable operation.
- Set up Nextcloud and test core functionalities.

[Back to Top](#project-overview)

# Wins

- Successfully hosted a private cloud server.
- Learned about Nextcloud and Raspberry Pi capabilities.

# Challenges

- Managing permissions and SSL certificates.
- Network stability during initial testing.

# Bugs and Future Improvements

- Issue: Occasional downtime during heavy file transfers.
- Improvement: Automate backup scripts and enhance monitoring.

# Key Learnings

- Improved understanding of self-hosting.
- Practical experience with Nextcloud and network configurations.

# Supporting Info

Links to useful articles, documentation, and community forums will be added here.

[Back to Top](#project-overview)
