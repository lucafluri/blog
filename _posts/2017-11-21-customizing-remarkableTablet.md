---
layout: post
title: Customizing the ReMarkable Tablet
author: Luca Fluri
published: true
---
**[Last Updated: 2017-11-21]**

# Getting Access  

1. On your ReMarkable go to **Settings/About/Copyrights and Licenses/General Information**
2. Under GPLv3 Compliance note the **username** (default = root) and **password** (its possible to change the password later)
3. Note the IP Address depending on how you want to connect to your device (USB is easier)
  - **USB**: [10.11.99.1](//10.11.99.1/) is the default Address (It's the same for the USB webinterface)
  - **WIFI**: The other IP Address
4. Connect via a **SFTP** Client (I recommend [FileZilla](https://filezilla-project.org/)) to the ReMarkable using the before noted IP Address, username and password (It has to be via SFTP not FTP. The Tablet currently only supports a SSH connection and SFTP is a FileTransferProtocol based on SSH)

# Files
There are several interesting or useful files to note:  
  - `/home/root/.bash.rc` (containing variable and color declarations, dont mess with it)
  - `/home/root/.config/remarkable/xochitl.conf` (Settings, ssh password, safed wifi networks)
  - `/usr/share/remarkable` (All Splashscreens, Templates and WebUI files)
  - `/home/root/.local/share/remarkable/xochitl` (Looks like all the thumbnail jpg for pdfs)


# Customizing
## SSH Password
One easy configuration is changing the ssh password for easier connection.     Just change the *DeveloperPassword* variable in `/home/root/.config/remarkable/xochitl.conf` to your new password.  

```
[General]
DeveloperPassword=SSHPASSWORD
Onboarding=false
OnboardingBanner=false
RightHanded=true

...
```

## Splashscreens
Under `/usr/share/remarkable` and `/usr/share/remarkable-shutdown` are all Splashscreens located. These are just png files that are displayed (i.e. the shutdown or sleeping screen). Note that all pngs concerning the shutdown are stored 2 times, if you change one you also want to change the other.  
Now you could draw up your own version and replace it (Remember to back up all the files).  

My sleeping screen for instance has this as background:
![Moon](https://i.imgur.com/JnjoF0w.jpg)

## Templates
Under `/usr/share/remarkable/templates` can all the templates be found. It's very similar to the Splashscreens, all are just pngs that are used as base layer in notebooks. Changing them is the same as for the Splashscreens (Remember to back up all the files).

## Further Resources
 - [https://www.reddit.com/r/RemarkableTablet/](https://www.reddit.com/r/RemarkableTablet/)
 - [http://www.remarkablewiki.com](http://www.remarkablewiki.com)
