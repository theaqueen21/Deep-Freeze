# Deep Freeze Enterprise: The Ultimate Reboot to Restore Solution
![Deep Freeze](https://github.com/user-attachments/assets/2b97a2e7-7058-4aa5-a3ea-2c4dc38d72a4)


## Introduction
Deep Freeze is a patented system management and protection software developed by Faronics. It is designed to preserve the desired computer configuration by restoring the system to its original state upon every reboot. This makes it an essential tool for managing and protecting endpoints, particularly in environments like public workstations, educational institutions, and business settings where consistency and security are paramount.

## Key Features of Deep Freeze

### 1. Automatic Restoration
Deep Freeze ensures that any changes made to a system during a session, whether intentional or accidental, are completely undone upon reboot. This feature is critical for maintaining system integrity in public access computers, where users often make changes that could affect subsequent users.

### 2. Malware and Security Protection
By reverting all changes at each reboot, Deep Freeze effectively eliminates malware and other security threats. This includes zero-day threats, which are particularly dangerous because they exploit previously unknown vulnerabilities.

### 3. Configuration Management
Deep Freeze prevents configuration drift by ensuring that every restart restores the system to its predefined state. This is especially useful in environments where maintaining a consistent configuration across multiple machines is necessary.

### 4. License Compliance
Deep Freeze helps organizations achieve software license compliance by automatically removing unauthorized software installations with every reboot.

### 5. User Empowerment
Despite its robust protection, Deep Freeze allows end users unrestricted access to the system during their session, knowing that any changes will be reversed.

### 6. Cloud Management
Deep Freeze offers cloud-based management, allowing administrators to deploy, configure, and manage Deep Freeze across a network remotely. This includes the ability to freeze and thaw systems from the Deep Freeze Administrator mobile app.

### 7. ThawSpace
ThawSpace is a feature that allows administrators to create virtual partitions on a frozen drive, enabling users to save work or important data that persists even after a reboot. This is particularly useful in environments where users need to retain data across sessions.

### 8. Power Management Integration
Deep Freeze integrates with power management tools, allowing administrators to schedule shutdowns, restarts, and [Wake-on-LAN](./Wake-On-LAN.md) actions either on-demand or on a scheduled basis.

### 9. Windows Update Management
Deep Freeze simplifies the management of Windows Updates by allowing updates to be downloaded and installed even when the system is in a frozen state. Administrators can schedule maintenance windows for these updates, ensuring that systems remain up-to-date without compromising the frozen configuration.

## Deep Freeze Console

The Deep Freeze Console is a powerful tool that allows administrators to manage multiple workstations from a centralized interface. Here’s a detailed look at its features and functionality:

### 1. Console Interface Overview
The Deep Freeze Console interface includes the following key components:
- **Network and Groups Pane:** Displays the network and workstation groups, allowing administrators to organize and manage computers.
- **Workstations Pane:** Provides detailed information about each workstation, including the operating system version, the version of Deep Freeze installed, and the current status (Frozen or Thawed).
- **Toolbar:** Contains icons for common tasks such as rebooting, shutting down, updating, and managing workstations. The toolbar becomes active when a workstation is selected in the Workstations pane.

### 2. Managing Workstation Status
In the Workstations pane, the status of each workstation is clearly indicated as either Frozen (ready for public use) or Thawed (ready for updates or changes). The Version column shows the Deep Freeze version installed, and any version mismatch between the Console and the workstation is highlighted in red. This visual cue helps administrators quickly identify and resolve potential issues.

### 3. Performing Common Tasks
- **[Reboot Thawed/Frozen:](./Frozen-Thawed.md)** Allows administrators to thaw a workstation to perform updates or install new software and then refreeze it for public use.
- **[Run Windows Update:](./Windows-Updates.md)** Manually initiates a Windows Update session and it will automatically refreeze after the update is complete.
- **[Update Deep Freeze Clients:](./Upgrade.md)** Pushes updates from the Deep Freeze Console to connected workstations. This process involves multiple reboots(Usually 2) but ensures that all systems are running the latest version of Deep Freeze.
- **[Managing the ThawSpace:](./Formatting-Deleting-The-ThawSpace.md)** Managing the ThawSpace is an important task for administrators, especially when you need to clear or repurpose the space.

### 4. Automating Maintenance Tasks
Deep Freeze can automate routine maintenance tasks, including Windows Updates. These tasks can be scheduled to run at specified times, reducing the need for manual intervention. For example, public computers can be left on over the weekend, allowing the scheduled task to reboot the computer, apply updates, and then power off the system, ready for use on the next workday.

> **Important Note:** The Windows Update Maintenance task was initially configured to execute periodically at 12 AM, specifically targeting times when the client PCs were idle and not in active use. This scheduling was intended to ensure minimal disruption to users while keeping the systems up-to-date. However, over the course of more than a month, it became evident that the task was not functioning as intended. Despite the configuration settings, the updates were not being applied consistently or reliably during the designated maintenance window.This prolonged period of malfunction highlights a significant issue with the Auto Maintenance Feature in its current form. Our testing experience suggests that this feature cannot be relied upon to manage Windows Updates effectively. The inconsistency in execution undermines the primary goal of maintaining system security and performance through timely updates. As a result, alternative methods or additional configurations may be necessary to ensure that updates are applied as required without user intervention.

![Tasks](https://github.com/user-attachments/assets/f62ba3a5-a7ce-44d9-b858-34428d725eef)

### 5. Remote Management and Security Enhancements
- **[Remote Launch:](./Remote-Launch.md)** Allows administrators to launch applications on selected computers directly from the Console or even push executables and launch them remotely.
- **MBR Protection:** Provides enhanced security by protecting the Master Boot Record from rootkit injections and other alterations.

## How Deep Freeze Works

Deep Freeze uses patented technology that redirects information being written to the hard drive to an allocation table, leaving the original data intact. When the computer restarts, the allocation table is discarded, restoring the computer to its original state, down to the last byte. This technology ensures that the system is always returned to its desired configuration, regardless of what happens during a session.

![Patent](https://github.com/user-attachments/assets/eb3c7cc6-e751-4590-86c5-e2a588b52fdf)

## Supported Platforms

Deep Freeze is compatible with both Windows and Mac operating systems. Supported platforms include:

### Windows
- Windows 7 (32 or 64-bit)
- Windows 8.1 (32 or 64-bit)
- Windows 10 (32 or 64-bit)
- Windows 11 (32 or 64-bit)

### Mac
- **HFS+ File System:**
  - OS X Mavericks 10.9.x
  - OS X Yosemite 10.10.x
  - OS X El Capitan 10.11.x
  - macOS Sierra 10.12
  - macOS High Sierra 10.13
- **APFS File System:**
  - macOS Mojave 10.14
  - macOS Catalina 10.15
  - macOS Big Sur 11
  - macOS Monterey 12
  - macOS Ventura 13
  - macOS Sonoma 14

## Conclusion

Deep Freeze is an indispensable tool for IT administrators tasked with managing and protecting public or shared computers. By ensuring that every reboot restores the system to its original state, Deep Freeze reduces IT costs, increases productivity, and enhances security. Its features, including cloud management, ThawSpace, and comprehensive Windows Update management, make it a versatile solution for a wide range of environments.

For more information and to see how Deep Freeze can benefit your organization, visit [Faronics](https://www.faronics.com).
