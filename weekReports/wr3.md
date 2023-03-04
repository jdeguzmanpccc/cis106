---
Name: Jerome De Guzman
Semester: Spring 23
Course: CIS106
---

# Week Report 3

## Summary of Presentations

### Introduction to Linux
**What is an operating system?**
An operating system provides all fundamental software features of a computer. An OS enables you to use the computer's hardware providing you the basic tools that make the computer useful. All of those features relay on the OS's kernel. Other OS features are owed to additional programs that run atop the kernel.

**Aside from a kernel, what other parts make an operating system?**
* **Command-Line Shells**
  * this was the de facto way odf using computers before the Graphical Interface was invented. CMDs work by typing commands in a shell. In Linux, the entire system can be control via the CLI. 

* **Graphical User Interfaces**
  * GUIs rely on icons, menus, and a mouse pointer for the user interaction. Linux relies on a GUI known as the X Window System in combination with desktop environment program suites.

* **Utility and Productivity Programs**
  * Tools like web browsers, document processors, and text editors.

* **Libraries**
  * Libraries are collections of programming functions that can be used by a variety of programs.

**What is a Linux distribution?**
A complete Linux system package is called a Linux Distribution.
* **A Linux Kernel**
  * Different distributions use different versions of the  Linux Kernel.
* **Core Unix Tools**
  * For instance, the GNU tool set, the X window System, a Desktop Environment, disk partitioning tools, etc.
* **Supplement Software**
  * For instance, server applications, user applications, and more.
* **Startup Scripts** 
  * These are scripts that differentiate different distributions they range from launching dozens of programs at startup to even modify the way the desktop environment behaves.
* **An Installer**
  * Different distributions use different installers and mange software differently as well. One of the key elements is the package manager a distribution uses.

**What is Ubuntu?**
Ubuntu is a Linux distribution, freely available with both community and professional support.

The Ubuntu community is built on the ideas enshrined in the Ubuntu Manifesto:
*   The software should be available free of charge.
*   The software tools should be usable by people in their local language and despite any disabilities.
*   People should have the freedom to customize and alter
*   Their software in whatever way they see fit

**Define the following terms: Open Source, Closed source, free software**
**Open Source -**  the software may be distributed for a fee or free. The source code is distributed with the software.
**Closed Source -** the software is not distributed with the source code. The user is restricted from modifying the code.
*   **Freeware:** the software us free but the source code is not available.
*   **Shareware:** the software is free on a trial basis.
**Free Software -** the software is distributed with the source code. The software can be free of charge or obtained by a fee. 

**What are the 4 freedoms defined by the free software foundation?**
* **Freedom 0:** use the software for any purpose
* **Freedom 1:** examine the source code and modify it as you see fit
* **Freedom 2:** redistribute the software
* **Freedom 3:** redistribute your modified software

### The basics of Virtualization
**What is virtualization?**
* Virtualization is defined as creating virtual versions of something.
* It is often used to let multiple OSs run on one physical machine at the same time.
* Allows administrators to divide the hardware and create multiple computers inside a single physical computer.

**List 3 benefits of virtualization**
* Allows running multiple OSs on one machine without dual booting.
* Allows applications to be tested before installing them ona host machine.
* Reduces costs by decreasing the physical hardware that must be purchased for a network.

**What is a hypervisor?**
**Hypervisor/Virtual Machine Manager (VMM):** Software or Hardware in charge of creating, managing, and running virtual machines.
* There are two types of Hypervisors:
  * **Type 1(bare-metal hypervisor):** This type of hypervisor runs directly on the hardware. The hypervisor is basically the operating system for the physical machine. Type 1 has better performance than Type 2, because there is no host OS involved and the sytem is dedicated to supporting virtualization. 
  * **Type 2:** This hypervisor is an application that runs on top of an operating system. This is most commonly used in client-side virtualization. The host OS consumes resources and a host OS failure means that the virtual machines will fail as well. 

**What is virtualbox**
It is a powerful x86 and **AMD64/Intel64** virtualization product for enterprise as well as home use. It is extremely feature rich, high performance product for enterprise customers, it is also the only professional solution that is freely available as **Open Source Software** under the terms of the GNU General Public License (GPL) version 3.

### Exploring Desktop Environments
**What is a desktop environment? (Provide 3 examples)**
A desktop environment is an implementation of the desktop metaphor made of a bundle of programs running on top of a computer operating system, which shares a common GUI, sometimes described as a graphical shell. 
**Desktop Environment Examples:** 
* GNOME
* KDE
* MATE

**List 4 common elements of desktop environments**
* **Favorites Bar -** This window area contains popular icons, which are typically used more frequently. These icons can be removed or added as desired.
* **Launcher -** This program(s) allows you to search for applications and files. It can also allow certain actions, such as start or open, to be performed on the search results. 
* **Menus -** These windows are typically accessed via an icon. They contain files and/or programs lists as well as sub-lists of additional files and/or programs selections.
* **Panels -** They are slim and typically rectangular areas that are located at the very top or bottom of a desktop environment's main window. They can also be at the desktop's far left or right. They often contain notifications, system date and/or time, program icons, and so on.

**What is Ubuntu’s default desktop environments?**
The default desktop in Ubuntu is GNOME 3. It is used not only by Ubuntu but also by several other Linux distributions, such as **Debian**, **Fedora**, **Red Hat Enterprise Linux**, and **Oracle Linux**. The official GUI for GNOME 3 is called GNOME Shell.

**What are the official flavors of Ubuntu?**
* Ubuntu GNOME
* Kubuntu
* Lubuntu
* Ubuntu Budgie
* Ubuntu Kylin
* Ubuntu MATE
* Ubuntu Studio
* Xubuntu
* Edubuntu
* Mythbuntu
 
### What is a Shell?
**What is Bash?**
The GNU bash shell is a program that provides interactive access to the Linux system. It runs as a regular program and is normally started whenever a user logs in into a terminal.

**How do you access the Linux CLI?**
There are two ways to access the CLI:
* Terminal Emulator 
* Linux Console

**What is a console terminal?**
* A virtual console is a terminal session that runs in Linux system memory
* It can be accessed using a simple keystroke combination. Usually you must hold down the Ctrl+Alt key combination and then press a function key(F1 through F7) for the virtual console you want to use.
* Text mode virtual consoles use the whole screen and start with the text login screen displayed.
* You can keep the virtual console active and switch between other virtual consoles without losing your active session. You can have multiple active sessions running at the same time. 

**What is a terminal emulator?**
A terminal emulator is a program that allows you to access the Linux CLI. 
Some terminal emulators are:
* GNOME Terminal
* Konsole
* Terminology
* RXVT-Unicode
* TILIX

**Provide 3 examples of Linux commands**
* **clear -** clears the terminal screen
* **date -** displays the current time and date 
* **df -** displays the current amount of free space on our disk drives 

### Managing Software 
**Which command is used for updating ubuntu**
sudo apt update

**Which command is used for installing software. Provide an example.**
sudo apt install
sudo apt install screenfetch -y

**Which command is used for removing software. Provide an example.**
sudo apt remove
sudo apt remove flameshot -y

**Which command is used for searching for software. Provide an example.**
apt search
apt search "web browser" - it will search for all programs that matches the text in quotes

**Definition of the following terms:**
* **Package** - archives that contain binaries of software, configuration files, and information about dependencies. (In Windows, these are commonly **.exe** files)
* **Library** - reusable code that can be used by more than one function or program
* **Repository** - a large collection of software available for download.
  * **Ubuntu repositories**:
    * Main - Canonical-supported free and open-source software
    * Universe - Community-maintained free and open-source software
    * Restricted - Proprietary drives for devices
    * Multiverse - Software restricted by copyright or legal issues