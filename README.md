# Ubuntu-checklist-CAP-CyberPatriot
A private checklist for Ubuntu operating system
Bascically I've compiled a list of things needed to be done based on previous competitions and practice image answer keys for Ubuntu


From powerpoints fron CyberPatriot https://docs.google.com/document/d/1dDJA3Go5ujMKW9vBFOBttLSg1UTz-xcX7ElfGnN37OM/edit  https://s3.amazonaws.com/cpvii/Training+materials/Unit+Eight+-+Ubuntu+Security.pdf


Basic Graphical User Interface (GUI) security

User settings 
Go to system settings (in menu bar click the gear with the wrench)
then go to user accounts(it's at the lower right hand corner and has two people)
click unlock(it's on the top right hand corner and has a unlocked lock)
it will ask you for a password(password is password)
switch user from administrator to standard(click next to account type the first one)
change passwords (by clicking next to passwords on the astericks)

Enabiling updates (do enabiling updates first but don't update version will mess with scoring)

First click the Ubuntu button(it's the first thing on the menu bar it's also reddish and has a ring with 3 circles)
Then search update manager(it's "Update Manager"  
If that doesn't show anything then try goint to the top bar at the top right and click the gear icon and go to software update and then at the lower right hand corner click settings)
To set automatic updates first go to the updates tab(it's on the top bar and is the third one from the left)
then make sure automaticlly check for updates is set for daily(it is the first setting with a dropdown menu)
then apply changes(don't click revert it resets all the settings to defult)
lastly update all availible settings do this at the end because it will take time(go to the main update manager window which is just the first tab)
Make sure you don't update the version of ubuntu this will mess up the scoring and will disqualify you

How to turn firewall on

You may need to install updates on ubuntu first but don't update the version
first install Gufw to do this you can go to termianl(to go to termianl just click the first button on the menu and typr terminal than click the terminal image not the xterm or uxterm but termianl
Than type :apt-get install gufw
remenber no caps and spaces after get , install 
if this doesn't work then you many need to go to root so type :sudo su 
then enter  apt-get install gufw 
if it still doesn't work then exit root by typing exit then type sudo apt-get install gufw
if it prompts you to confirm that you want to type capital y
then go to the ubuntu button (it's the fisrt on the menu)
and search firewall configuration
then click the unlock on the gufw window when it pops up if it doesn't the go to the ubuntu button and dearch gufw
The default (and recommended rules) governing traffic are
to Deny all incoming traffic and Allow all outgoing traffic so on the window where there is a sheild with the colors red green and white make status on and incoming set to deny and outgoing set to allow. then open or block ports by clicking on the simple or advanced tabs




Allowing ports

got to termianl by clicking the ubuntu button and serching termianl and click on it not xterm or uxterm
and type the command sudo kill $(sudo lsof -t -i:3000)
this will close port and the numbers 3000 stand for the port you want to close so if you want to close the ssh port you type sudo kill $(sudo lsof -t -i:22)
because ssh connects to port 22
all the ports that need to be blocked are TCP port 21 — FTP (File Transfer Protocol)


TCP port 22 — SSH (Secure Shell)


TCP port 23 — Telnet


TCP port 25 — SMTP (Simple Mail Transfer Protocol)


TCP and UDP port 53 — DNS (Domain Name System)


TCP port 443 — HTTP (Hypertext Transport Protocol) and HTTPS (HTTP over SSL)


TCP port 110 — POP3 (Post Office Protocol version 3)


TCP and UDP port 135 — Windows RPC


TCP and UDP ports 137–139 — Windows NetBIOS over TCP/IP


TCP port 1433 and UDP port 1434 — Microsoft SQL Server






