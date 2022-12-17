# Creating Desktop Environment for linux VM using Gnome

- Creating a Gnome Desktop enviroment to add on your of Linux shell after creating a linux instance.
  - This may be very useful when need to use a linux Desktop environment when you only have access to CLI.
  - Linux Desktop environment come with many useful tools, such us Libre Office, VLC, Audacity and much more.

- Note: This steps are also valid for AWS or Other RDP services. use to set up Kali GUI on virtual Machines.

## 1-Requirements:
- Linux instances
- Network connectivity for downloads

## 2-Step By Step Procedures:

- Login SSH using in terminal
- ssh username@IP
- Enter Password 

####  Update the linux system

       sudo apt-get update && sudo apt dist-upgrade

- Execute the following Commands:
    - apt-get install xrdp
    
    <br/>
<img src="https://github.com/sanfofana/multipurpfiles/blob/main/Screen%20Shot%202022-12-17%20at%2012.48.19%20PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

    - systemctl enable xrdp
    
    - echo xfce4-session>~/.xsession


<img src="https://github.com/sanfofana/multipurpfiles/blob/main/Screen%20Shot%202022-12-17%20at%201.02.26%20PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
    
    - service xrdp restart

## 3-Finally install GNOME Desktop

       apt-get install -f gdm3
       
<img src="https://github.com/sanfofana/multipurpfiles/blob/main/Screen%20Shot%202022-12-17%20at%201.02.45%20PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

## 4- Connect to your graphical interfaces using RDP 
- Note: After completing all the previous steps, make sure to create and allow an RDP connection to your in Azure Ressource group.
- You can do this by creating an inbound rule in NSG, then you can connect using RDP.

<img src="https://github.com/sanfofana/multipurpfiles/blob/main/Screen%20Shot%202022-12-17%20at%201.17.19%20PM.png" height="45%" width="70%" alt="Disk Sanitization Steps"/>

<img src="https://github.com/sanfofana/multipurpfiles/blob/main/Screen%20Shot%202022-12-17%20at%201.26.04%20PM.png" height="45%" width="70%" alt="Disk Sanitization Steps"/>
<br />
