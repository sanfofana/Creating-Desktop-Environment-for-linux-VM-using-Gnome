# Creating-Desktop-Environment-for-linux-VM-using-Gnome

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

- First update the linux system
    - Command: sudo apt-get update and apt dist-upgrade

- Execute the following Commands:
    - apt-get install xrdp
    - systemctl enable xrdp
    - echo xfce4-session(right angle bracket)~/.xsession   (as shown in video. Check video)
    - service xrdp restart

## 3-Finally install GNOME Desktop
       apt-get install -f gdm3
