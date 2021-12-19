# 1. Setup a Linux computer for everyday use
# Table Of Content
- [1. Setup a Linux computer for everyday use](#1-setup-a-linux-computer-for-everyday-use)
- [Table Of Content](#table-of-content)
  - [1.1. Introduction](#11-introduction)
  - [1.2. Machine Specs (Requirements)](#12-machine-specs-requirements)
  - [1.3. Part 1](#13-part-1)
    - [Open Oracle VM VirtualBox Manager](#open-oracle-vm-virtualbox-manager)
    - [Set Name and OS version](#set-name-and-os-version)
    - [Memory Size](#memory-size)
    - [Virtual Hard Disk](#virtual-hard-disk)
    - [Hard Disk File Type](#hard-disk-file-type)
    - [Storage on physical hard disk](#storage-on-physical-hard-disk)
    - [HDD Size](#hdd-size)
  - [1.4. Part 2](#14-part-2)
    - [Move to the VirtualBox Settings](#move-to-the-virtualbox-settings)
    - [Write Description](#write-description)
    - [System setting](#system-setting)
    - [Display Settings](#display-settings)
    - [Storage Settings](#storage-settings)
    - [Audio Settings](#audio-settings)
  - [1.5. Part 3](#15-part-3)
    - [Start the VirtualBox machine](#start-the-virtualbox-machine)
    - [Select Installation Type](#select-installation-type)
    - [Software Update](#software-update)
  - [1.6. Ubuntu Terminal](#16-ubuntu-terminal)
    - [Some useful commands to use in terminal](#some-useful-commands-to-use-in-terminal)
    - [Internet browsing](#internet-browsing)
      - [Install firefox](#install-firefox)
      - [Install Google Chrome](#install-google-chrome)
    - [School Work](#school-work)
      - [Install Libre Office](#install-libre-office)
      - [Install Discord](#install-discord)
      - [Install Zoom](#install-zoom)
  - [TroubleShoot](#troubleshoot)
  - [Work Cited](#work-cited)



## 1.1. Introduction

Linux is an open source operating system. It allows users to use, create, and modify the system without any restriction. Ubuntu is popular linux distribution. It is so light and easy to use that anyone can run this in a virtual machine. A virtual machine allows user to use other operating system inside another OS, where the virtual machine is. Ubuntu is so light and error-proofed that sometimes it is more powerful than the host machine. It is freely available for casual and professional users. Today we are going to learn about how to setup linux (ubuntu) in a virtual machine.

## 1.2. Machine Specs (Requirements)
 In order to install ubuntu, we need to download the Ubuntu ISO file and instal a virtual machine. We are using the Oracle VM VirtualBox 6.1. You can download the latest version of VM ViirtualBox from here: [VirtualbBox](https://www.virtualbox.org/).
 You can also download the Ubuntu ISO from [here](https://ubuntu.com/download/desktop).
 **Also, we have some hardware requirements**.
 * HDD: 50 gb (min 40 gb)
 * RAM: 2 gb (if the computer has more than 8 gb, than 4gb preferable)
 * CPU: 2 cores (or more)
 * Video graphics: 128 MB
 * Network Card: 1 NAT Card
 * Monitor
 * Mouse and keyboard to input commands.
  
  **We are going to install Ubuntu 20.04 version using the ISO files already downloaded in the pc. If you want to download it from a cd, then you will need a CD-Drive**

   

## 1.3. Part 1


  ### Open Oracle VM VirtualBox Manager

   The VM Virtual machine interface has lot of options to modify. From Tools, select *New*

  ![step 1](./vmSetup/vmNew.png)
   Follow the instructions on the screen and drag the installer into the applications folder

   
  ### Set Name and OS version
   The *Name and  operating system* window, select a preferable name. *Machine Folder* is the location the ubuntu system will be stored. Select **Linux** in *Type* and **Ubuntu (64-bit)** (we downloaded the version) in *Version*.

  ![step2](./vmSetup/naming.png)

  ### Memory Size
   Select the size of the RAM 2048 MB (or more). If your computer has more than 8 GB RAM, than increase the size there.
   
   ![step 3](./vmSetup/ram.png)
   
 
  ### Virtual Hard Disk

   There are 2 options. First options allows you to create the vm without a disk. Second options allows to create a virtual hard-disk of any size. Third one allows you to use the already existed virtual hard-disk. Chose what you prefer.

  ![step 4](./vmSetup/vHDD.png)

  ### Hard Disk File Type
   These are the three popular disk format. We are going to use the VDI (Virtual Disk Image) as our ISO file in the same hard disk.
   ![step 5](./vmSetup/insFile.png)

  ### Storage on physical hard disk
   **Dynamically allocated** option uses very small portion of disk space but it will increase accordingly if the file size increases. **Fixed size** just take the whole space assigned to it. We will chose the first one here. 
  ![step 6](./vmSetup/diskAllocation.png)

  ### HDD Size
   Ubuntu takes 25 GB of hard disk. So, in order to run properly, a virtual machine needs at least 40 gb of the hdd, as you will install more softwares later. Increase the size if you have more in your pc. Click *Create*
  ![step 7](./vmSetup/hddSize.png)

## 1.4. Part 2

  ### Move to the VirtualBox Settings
   
   From `General`, select `Advanced` and make both `Shared Clipboard` and `Drag'n'Drop` *Bidirectional* using the dropdown.
   ![8tep 8](./vmSetup/settings.png)

  ### Write Description
   It is a section to write down notes or information about something you might need late. For example: your host name, company name, username, password, etc.
  ![step 9](./vmSetup/description.png)

  ### System setting
   Select `System` from the left menu. In *Motherboard* section, base memory should be at least 2048 MB. Uncheck `Floppy` and `Network` from the *Boot Order* Section.

   ![Step 10](vmSetup/sysMB.png)

   Select *Processor*. Make the `Processor's` 2 or more if available. Uncheck `Enable PAE/NX` if your system is not 64 bit.

   ![Step 11](./vmSetup/sysProc.png)

  ### Display Settings
   From the *Screen* section, increase the `Video Memory` to 128 MB. Check `Enable 3D Acceleration`.
   ![step 12](./vmSetup/display.png)

  ### Storage Settings
   From the *Storage* section, click on `Controller: IDE` under the *Storage device* section. 
   In the *Attributes* section, select the disk drive the ISO file is on. Then click on disk icon > chose from file. Look for the Ubuntu-***.ISO file and select it. Click `ok`. 

   ![Step 13](./vmSetup/selectISO.png) 
   ![Step 14](./vmSetup/selectedFile.png)

  ### Audio Settings

   From Audio settings, uncheck `Enable Audio` as some mac user could face problem for a bug in the code.
  
## 1.5. Part 3

  ### Start the VirtualBox machine
   Click `Start` while selecting the machine. It will ask you to select the start-up disk. This is where your Ubuntu ISO file should be. Select that from the drop-down menu and click on `Start`.

   ![step 15](./vmSetup/selectUbuntu.png)
  
   *Ubuntu will start checking if the system has any errors.*

  ### Select Installation Type
   Ubuntu will ask if you want to try a live version of it before installing it. We are installing the full system so click on `Install Ubuntu`. 
   ![step 16](./vimSetup/select%20lang.png)
   *Select the preferred language.*


  ### Software Update
   It will ask you to whether you want normal installation, or minimal installation. Also, if you want ubuntu to download add ons and stuffs. Check `Normal Installation` and check both for the *Other Options*.
   ![Step 17](./vmSetup/softUp.png)

   *You can also update ubuntu using terminal.*

   **Ubuntu finish software install and update and start shortly with a beautiful simple home screen.** 
   ![done](./vmSetup/done.png)

   - There are a lot of resources on how to setup ubuntu. You can check  this *Youtube* video on [How to Install Ubuntu in a Virtual Machine](https://www.youtube.com/watch?v=x5MhydijWmc)


## 1.6. Ubuntu Terminal
  The best thing about ubuntu is we can do pretty much everything using the terminal. Open by clicking on the left-bottom corner icon, or from the **Aplication** section.

  ![terminal](./vmSetup/openingter.png)
  

  ### Some useful commands to use in terminal
  | Commands | What they do | Example |
  |----------|--------------|-----------|
  | pwd | Shows the current location | pwd |
  | ls | list all the files and directories | ls Documents/ |
  | tac | Display the content of a file in reverse order | tac file1.txt |
  | touch | create files | touch file2.txt |
  | mkdir | create directories | mkdir newFolder |
  | cd | get inside a directory | cd Documents/ | cd ~ (home) |
  | rm | delete files and directories | rm file2.txt
  | cp | copy files and directories | cp file1 file2
  | head | Display first 5 lines of a file | head file1.txt
  | tail | Display last 5 lines of a file | tail file1.txt
  

   *Follow the link for more examples:* [Linux Commands](https://robertalberto.com/linuxcommands/home.html)

  Type: `sudo apt install screenfetch -y` to install screenfetch



  ### Internet browsing
   Ubuntu should have already pre-installed firefox for browsing the internet. In not, you can easily using the graphical application center or the terminal.
   Here are few web browser's download command lines you can try:

  #### Install firefox
   You can browse, download, upload, basically experience the world of web using firefox. Just put the url of a website in the address bar and you can access the content of that site.
     `sudo apt install firefox`
  
   If you do not like firefox, and want to use other web browser, you can just search for it in terminal using `search apt "web browser".


  #### Install Google Chrome
   Google is not open source but it is one of the most popular web browser out there. Navigation system is almost same as firefox or most of the browser.
   First, we will download the developer package to install google chrome. Type the command:

   `wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb`

   ![download package](./vmSetup/ggl1.png)

   **Now install using it from your local folder using the command:**

    `sudo apt install ./google-chrome-stable_current_amd64.deb`

   ![Install Chrome](./vmSetup/ggl2.png)

   **After the installation is done, you can find it in the `application>internet` from the top left corner**

### School Work   

  #### Install Libre Office
   Libre Office is an open source version of Microsoft Office. We can create text documents, presentations and calculation sheets just like  Word, powerpoint and excel with libreoffice.
    
   *Note: There are plenty other word documents software out there. You can search using the say way of searching web browser.*

   First, We have to update the cache in order to install the libreoffice.
   Type: `sudo apt update`

   After updating the cache we will install libre office for that we will insert the following command
   Type: `sudo apt install libreoffcie`

   ![libreoffice](./vmSetup/libreoffice.png)

     

   Press `'Y'` to continue

   *After the installation is complete, you can find it in application.*

  #### Install Discord 
   Discord is a multipurpose online streaming platform. You can stream yourself, watch other streamer, chat with people (audio/video/text). It is is great way of file sharing too. All you have to do is create an account using your email and password. Than find channel to subscribe or stream yourself live.
   Download the file from here:  https://discord.com/download to download the package
   ![download discord(./vmSetup/discord.png)

   Install it from the local disk using the command from your home directory:
   `sudo apt install /Downloads/discord-0.0.14.deb`
   insert the password and press `y`

  #### Install Zoom
   Zoom is an online video calling/meeting application. People around the world use it for online meeting, particularly in schools, colleges, and offices. Multiple people can join in a audio or video conference using zoom. It allows users to share there computer/mobile screen to other people in the meeting.
   Download zoom from here: https://zoom.us/download
   Select the package you want. we are downloading Ubuntu 16.04 version.
   ![zoom](./vmSetup/zoom.png)
   Now install it from your home directory using the command:
  `sudo apt install /Downloads/zoom_amd64.deb`
   Give your password and press `Y` in next steps to finish installation.

   After installation is complete, sign-in or create an account with your email. Join other meeting using meeting-id or create your own meeting and share the id with the targeted participant. You can make the meeting closed or public to matter of your security concern.

## TroubleShoot
 * Use the `man --help` command to open help functions.
  ![manHelp](vmSetup/man.png)

 * Hover on the monitor icon in the top-right corner of the menu bar to get  more help.
 ![help](vmSetup/help.png)
 * Searching online: There are plenty of resources in the web.

## Work Cited

 ProgrammingKnowledge. “How to Install Ubuntu 20.04 LTS on VirtualBox in Windows 10.” YouTube, YouTube, 24 Apr. 2020, https://www.youtube.com/watch?v=x5MhydijWmc.

 “CIS 106: Linux Commands.” Home, robertalberto.com/linuxcommands/home.html.

 Linuxize. “How to Install Google Chrome Web Browser on Ubuntu 20.04.” Linuxize, Linuxize, 24 Apr. 2020, linuxize.com/post/

 Awaisi, Kamran Sattar. “Install LibreOffice on Ubuntu 20.04 and Linux Mint 20.” Linux Hint, 1 Oct. 1969, linuxhint.com/install-libreoffice-ubuntu-linux-mint. 


 