# Installation of Ubuntu
## 5 reasons why Linux ?💻
### 1. High security🔐
Linux is less vulnerable to threats and different types of attacks (hacks) over 'Windows OS'.
When you have Windows installed, you need to download/purchase an Antivirus program to keep your computer safe from hackers and malware. However, Linux does not require the use of such Anti-Virus programs. Of course, a couple of software tools still exist to help you keep your system free from threats, but it is often unnecessary when you have a Linux system.
### 2. Open source 🏆
The aspect that makes linux different from other operating systems is that it falls under FOSS(Free and open source software) i.e., it's source code is freely available.
The developer community benefits from this as its members have the freedom to view and modify the source code, which is not possible in other OSs.
### 3. Runs on any hardware 💿💾
With 'Linux', you could even utilize one of your oldest computer systems to achieve a task. However, that does not mean that every Linux distribution would work with 256 MB of RAM coupled with an outdated processor. However, there are options which you can install on such low-end systems as well (such as Puppy Linux).Whereas windows requires a higher hardware configuration (minimum hardware requirements) in order to support different updates.
### 4.Customisation 🔧⚙
One major advantage of using Linux is 'customization'. 'Linux' is perfect tewaking system’s looks. There are numerous choices for wallpapers, desktop icons and panels. 
For any task, right from the GUI interface and file managers, to DVD burners and browsers, around four to six options are available for any particular software. The Linux versions of most popular browsers are also available.
### 5. Great community support👩🏻‍💻
There's no need of hiring any expert while facing issues or threats. We can find solutions of the threats just by a web search, or post it to let others solve the problem. A reply with a detailed explanation of the solution is given that resolves a problem at completely no cost!

## Steps followed while installing Ubuntu

#### Step-1
Allot space to install the software and make sure that at least a minimum of 25 GB of free storage space, or 5 GB for a minimal installation is available.

#### Step-2
Install 'Ubuntu' 
##### ( 📃Resource: https://ubuntu.com/#download )

#### Step-3
Create a bootable USB stick using a utility such as Universal USB Installer (BIOS compatible) or Rufus (UEFI compatible).

#### Step-4
Place the USB stick or DVD in the appropriate drive, reboot the machine and instruct the BIOS/UEFI to boot-up from the DVD/USB by pressing a special function key (usually    F12, F10 or F2 depending on the vendor specifications).Once the media boot-up a new grub screen should appear on your monitor. From the menu select Install Ubuntu and hit Enter to continue.

#### Step-5
After the boot media finishes loading into RAM you will end-up with a completely functional Ubuntu system running in live-mode.
On the Launcher hit on the second icon from top, Install Ubuntu 19.04 LTS, and the installer utility will start. Choose the language you wish to perform the installation and click on the Continue button to proceed further.

#### Step-6
Next, choose the first option “Normal Installation” (out of ‘Normal installation’ and ‘Minimal installation’) and hit on the Continue button again.Beneath the installation-type question are two checkboxes; one to enable updates while installing and another to enable third-party software (enabling both "Download updates" and "Install third-party software" is recomended).

#### Step-7
Use the checkboxes to choose whether you’d like to install Ubuntu alongside another operating system, delete your existing operating system and replace it with Ubuntu, or — if you’re an advanced user — choose the ’Something else’ option.

#### Step-8
After configuring storage, click on the ‘Install Now’ button. A small pane will appear with an overview of the storage options you’ve chosen, with the chance to go back if the details are incorrect.Click Continue to fix those changes in place and start the installation process.

#### Step-9
If you are connected to the internet, your location will be detected automatically. Check your location is correct and click ’Forward’ to proceed.

#### Step-10
Fill in the login details.

#### Step-11
The installer will now complete in the background while the installation window teaches you a little about how awesome Ubuntu is.

#### Step-12
After everything has been installed and configured, a small window will appear asking you to restart your machine. Click on Restart Now and remove either the DVD or USB flash drive when prompted.
### 🎉🎊 Congratulations!You have successfully installed Linux operating system!
##### 💿📚Reference: https://ubuntu.com/tutorials/install-ubuntu-desktop#11-installation-complete

## Challenges I faced while installing Ubuntu
While installing the software I had a pop-up window on my screen that said "Disable intel RST".

## Solution
The most important aspect of Linux is that it has a 'Great community support'.
I searched my issue in the community and found the solution with a detailed explanation.

There were 2 solutions to my problem:
### Solution_1
Switch your disk setting in the BIOS from RAID to AHCI.
(But, there was a shortcoming in this process as making that switch comes with some problems though, as Windows will no longer boot.)
### Solution_2
#### Step-1
Right-click the Windows Start Menu. Choose Command Prompt (Admin).
#### Step-2
If you don’t see Command Prompt listed, it’s because you have already been updated to a later version of Windows.  If so, use this method instead to get to the Command Prompt:
#### Step-3
Click the Start Button and type cmd
#### Step-4
Right-click the result and select Run as administrator
#### Step-5
Type this command and press ENTER: bcdedit /set {current} safeboot minimal
#### Step-6
If this command does not work for you, try bcdedit /set safeboot minimal
#### Step-7
Restart the computer and enter BIOS Setup (the key to press varies between systems).
#### Step-8
Change the SATA Operation mode to AHCI from either IDE or RAID (again, the language varies).
#### Step-9
Save changes and exit Setup and Windows will automatically boot to Safe Mode.
#### Step-10
Right-click the Windows Start Menu once more. Choose Command Prompt (Admin)
#### Step-11
Type this command and press ENTER: bcdedit /deletevalue {current} safeboot
#### Step-12
If you had to try the alternate command above, you will likely need to do so here also: bcdedit /deletevalue safeboot

##### Reboot once more and Windows will automatically start with AHCI drivers enabled.
##### 📚Reference: https://askubuntu.com/questions/1281127/disable-rst-for-installing-ubuntu-20-4-dual-boot

### I've followed "Solution_2" to resolve my issue. Now I have successfully dual booted my laptop with "Ubuntu".







