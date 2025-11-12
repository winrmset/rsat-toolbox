## Download RSAT (Remote Server Administration Tools)

Download the latest version from Releases page:        
https://github.com/wevtutil/RSAT/releases/tag/1.412

RSAT allows IT administrators to remotely manage Windows Server roles and features from a system running Windows 10 or a later supported Windows client version. This toolkit is essential for professionals working with server infrastructure, especially when performing tasks related to active directory download and other network management operations.

## System requirements

* Requires .NET Framework 4.6 or higher
* Minimum supported operating systems: Windows 10 or Windows Server 2016
* Not supported on Windows Home editions
* Administrator privileges required for installation

## Introduction

RSAT cannot be installed on computers running the Home or Standard editions of Windows. It is only supported on Professional or Enterprise editions of the Windows client OS. Unless the download page explicitly states compatibility with a beta, preview, or prerelease version of Windows, a full (RTM) version of the operating system is required for installation and reliable functionality. Some users have tried to bypass the RSAT MSU restrictions to install it on unsupported editions or builds of Windows; however, such actions violate the Windows end-user license agreement and may result in instability.

Installing RSAT resembles the process of installing Adminpak.msi on client machines running Windows 2000 or Windows XP. Yet, there is a key distinction: on Windows 7, the tools are not automatically ready after installation. You must manually activate the tools you need through the Control Panel. To proceed, open **Start** > **Control Panel** > **Programs and Features**.

In RSAT packages designed for Windows 10, all tools are automatically enabled once the installation is complete. To disable any components you don’t intend to use on Windows 7, open **Turn Windows features on or off** and deselect them.

For Windows 7 users, it is necessary to manually enable the tools associated with the specific roles and features you wish to manage after installing the RSAT package. These active directory tools and other components provide essential functionality for remote server administration.

If you’re managing roles or features on remote servers running Windows Server 2012 R2 or newer, you don’t need to install extra utilities. Simply open the Add Roles and Features Wizard in Windows Server 2012 R2 or later, then on the **Select Features** screen, expand **Remote Server Administration Tools**, choose the required components, and complete the wizard to finish installation.

## RSAT for Windows 10, version 1809 or later versions

> **Note**
> The **Turn Windows features on and off** dialog in Control Panel is no longer available.

Installing RSAT on Windows 10 version 1809 and newer differs slightly from earlier releases. RSAT is now integrated into the operating system itself and can be installed directly via **Optional Features**. This integration simplifies deployment and ensures the latest versions of the tools are automatically aligned with system updates, making active directory download and other administrative configurations more efficient.
