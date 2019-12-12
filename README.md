Bluscrn's Cisco Helper Scripts V0.1

*sudo priveleges are required for this script to run*

*console access is needed, edit main.menu <serial=$(ls /dev/ttyUS*)> to properly reflect your serial port*

*opening minicom is recommended in order to watch Cisco output*
Install minicom <sudo apt install minicom> or <sudo dnf install minicom>
<sudo minicom -s>

Edit the creds.var file with your username and password 
install tftp-hpa <sudo apt install tftp-hpa> or <sudo dnf install tftp-hpa>

Run main.menu <bash main.menu>

Option 1 opens the IOS upload menu
    Creates basic network and tftp's file of your choice into Cisco device
    r1-4.sh and s1-6.sh are utilized
    interface commands in these scripts may need to be adjusted depending on hardware configuration
Option 2 will tftp and extract an archive of your choice (CME firmware or any .tar)
Option 3 runs crypto.sh (Use at your own risk)
Option 4 copies file of your choice to flash then start
Option 5 generates SSH keys
Option 9 Sets tftp root as a variable (run this first, only needs to run once)
Option 0 Input IP of your computer here (run this first, only needs to run once)


V0.1 - *Untested* edits to call variables and make scripts more universal