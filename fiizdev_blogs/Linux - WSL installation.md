![[Pasted image 20250307155735.png]]

As you know this blog will be about preparation for second part of **Journey into 'How to be hacker'** if you haven't read the first part, feel free to read it [here](https://tinyurl.com/P1-journey). Let's install linux!

**FYI: im doing this tutorial on Windows 10, so it might have different feature with Windows 11**
## Is my computer support WSL?
Before you start to install WSL, you need to know if your computer support WSL, most latest laptop and computers with windows 10/11 is support, anything below than Windows 10 you might want to run linux on virtual machine.

> ***WSL 2 requires Windows 11, or Windows 10 version 1903 or higher, with Build 18362 or higher, for x64 systems, and Version 2004 or higher, with Build 19041 or higher, for ARM64 systems**.* - Google


This tutorial will be based on Microsoft installation manual
- [Manual installation steps for older versions of WSL](https://learn.microsoft.com/en-us/windows/wsl/install-manual)


## Enable the Windows Subsystem

### Step 1 :- enable wsl
Before installing Linux we need to enable 'Windows Subsystem', to do that open Powershell as Administrator:

press `[Win Key]` and search for 'powershell', right click and click 'run as administrator', or you can click the 'Run as administrator' on the right box
![[Pasted image 20250307152831.png]]

When powershell terminal window is open, paste this command into your powershell terminal:
```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```
![[Pasted image 20250307153313.png]]

### Step 2 :- check build version
Next is upgrading to WSL 2, for that you need to check the Windows OS Build:

press `[Win Key] + [R]` and type 'winver'

![[Pasted image 20250307153651.png]]

this window will pop up:
![[Pasted image 20250307153718.png]]

you can see there on the  'OS Build ...', that is the build number, so this is the note from microsoft:

> Builds lower than 18362 do not support WSL 2. Use the [Windows Update Assistant](https://www.microsoft.com/software-download/windows10) to update your version of Windows. The Windows version 1903 support is also only for x64 systems. If you are using an Arm64 version of Windows, you will need to upgrade to Windows 10 version 2004 or later for full access to WSL 2. For more info, see [WSL 2 support coming to Windows 10 Versions 1903 and 1909](https://devblogs.microsoft.com/commandline/wsl-2-support-is-coming-to-windows-10-versions-1903-and-1909).

So basically based on my build number that i can upgrade my WSL to WSL 2, but if your computer is lower than '18362' try update your windows, you still can use WSL but the feature might be different than WSL 2.

### Step 2.1 :- update windows
To update the WSL to WSL 2 we need to go to the Windows Update, press `[Win Key] + [S]` type 'update', click the 'Check for updates'.
![[Pasted image 20250307154344.png]]

Just wait for the update to download the new update and click the 'Install Now'.
![[Pasted image 20250307154459.png]]

After installation done, you'll need to restart your computer or you can click the 'Restart Now' button after the installation is done.

### Step 3 :- Enable Virtual Machine feature
Open Powershell as administrator like how you open it on the step 1, paste this command to your powershell terminal window:
```
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```
![[Pasted image 20250307155405.png]]

Restart you computer.

## Download the Linux kernel update package
Open again Powershell as administrator and we need to update the wsl, paste this command on you Powershell terminal windows:
```
wsl.exe --update
```
![[Pasted image 20250307160055.png]]

**Before you go into next step, if you're using Windows on Virtual Box, enable 'Nested VT-x/AMD-v' in Settings > System > Processor, on the Acceleration set the 'Paravirtualization Interface' to 'KVM' and don't set the default version to '2'**

and next is set the WSL to version 2 or WSL 2, copy & paste this command:
```
wsl --set-default-version 2
```
![[Pasted image 20250307160151.png]]

## Install Linux distro
It's time for the Linux installation, for the Journey i'll be using Ubuntu distro there are a lot of Linux flavor that you can use and it have different use for it. To keep it simple for next journey we gonna use Ubuntu

Open 'Microsoft Store' and search for 'ubuntu'
![[Pasted image 20250307160555.png]]

we'll use the 'LTS' version, LTS means Long Term Support your ubuntu will be receive updates for 5 years including security updates.

Click the Ubuntu with LTS prefer the latest version of Ubuntu at the time im writing this tutorial its 22.04.5 LTS. then click 'Get'

![[Pasted image 20250307160957.png]]

Wait for the Installation to finish, and Launch the Ubuntu! after done installation..

## Virtual Box (0x80370102)

well i got an error with my Ubuntu.. since im running my windows on Virtual Machine(vbox) there might be some problem with it :(

![[Pasted image 20250307161601.png]]

**if you use virtual machine, go to your window vm > settings > system > acceleration, there's options for Paravirtualization Interface, select 'KVM' and on Processor enable 'Nested VT-x/AMD-v'**

**Don't set your WSL to version 2 if you're in Virtual Box**

![[Pasted image 20250307164559.png]]

![[Pasted image 20250307164618.png]]

## Ubuntu Setup
Congrats on finish installing your WSL and Linux, lets go on setting up Ubuntu:
![[Pasted image 20250307164951.png]]

You will see this box pop up when you lunch the Ubuntu, for the first time it will take few minutes to install some stuff and then it will ask for UNIX username, just type any username you want i prefer its in characters and no numbers or special characters, and type the password for your linux user, make sure you remember this password. after done setting up user and password for your linux and its ready to go!

![[Pasted image 20250307165328.png]]
## First time..
What do you need to do when its the fresh install of linux, you need to do update and upgrade. to do that you will not using and GUI like windows doing update, its just command.

First is update, this will update your linux repo for latest version of updates, type this command on your Ubuntu terminal:
```
sudo apt update
```

The command output will be look like this, don't worry about the wordings and numbering..
![[Pasted image 20250307170014.png]]

Then you going to do upgrade, this command will upgrade the Ubuntu programs, type this:
```
sudo apt upgrade -y
```
Let the upgrade do its work, don't worry about it..

## sudo? apt?
In windows, if you want to run something as Administrator like Powershell on this tutorial you'll need to right click on it and click 'Run as Administrator', but in Linux we use 'sudo' to run a command as Administrator or root you need to start it with 'sudo'.

So in Linux they use 'root' as the most privilege user in system, but in windows there are 'System' and 'Administrator', mostly for windows user they use 'Administrator' privilege.

what is apt? not the apt apt apt - Rose and Bruno mars song, the apt in the linux.. apt is the package tool, use for installing program, update, and remove. in Windows you have windows update, and Add or Remove Program

## End :D
i guess that's all, hopefully everything is good with the WSL installation. see ya on the second part of the Journey into 'How to be hacker'