# 10 min. novice guide - Setting Up Remote Connection to Raspberry Pi using VNC Server and Viewer

## Rationale of this guide
This guide serves as a short walkthrough in setting up Raspberry Pi remote connection (installed with Raspbian OS) using VNC Server and VNC Viewer. 
Once the setup is done, the Raspberry Pi can be connected remotely to your laptop or mobile installed with VNC viewer.
<br>
<br>

## How do I benefit from this guide?
- Understand how to set up a new Raspberry Pi for remote connection via other devices. 
- Before starting this guide, make sure the Raspberry Pi is installed with Raspbian OS and your device is installed with [VNC Viewer](https://www.realvnc.com/en/connect/download/viewer/). 
- Make sure you have registered a free account in VNC too. [Register here](https://manage.realvnc.com/en/)
<br>

## Walkthrough
1)	Update the Raspberry Pi to the latest version: 
-	Run command: sudo apt-get update
-	Run command: sudo apt-get dist-upgrade
-	Run command: sudo reboot 

2)	Change the Raspberry Pi hostname & password
-	Goto preferences -> Raspberry Pi Config -> System 
-	Change hostname
-	Click “Change Password”
> Remember the **hostname** & **password** as you need it to login into your Pi later

> Want to enter simpler password instead? 
> - Run command: sudo -s 
> - Run command: passwd user

3)	Enable VNC:
-	Goto preferences -> Raspberry Pi Config -> Interfaces 
-	Enable VNC

4)	Configure timezone:
-	Goto preferences -> Raspberry Pi Config -> Localisation 
-	Click Set Timezone: Asia : Kuala Lumpur

5)	Set up VNC server
-	Open VNC Server (Icon VNC at the top-right corner)
-	Select setting toolbar (in the header) -> Licensing
-	Sign in to your Real VNC account 
-	Select direct connection and cloud connection

6)	Initiate remote connection from your device
>	Remember to install VNC viewer on your device  
-	Open VNC viewer and enter the **hostname** previously customized in the search bar 
-	Sign in to the pi (username: pi; **password**: as customised previously)
-	After sign in, make sure you had rename the Raspberry Pi in the dashboard (address book) to your updated hostname for easier login in the future
<br>
<br>

#### Copyright disclaimer
The resources mentioned in this guide (if any) are purely for learning purpose. No copyright infringement intended.
