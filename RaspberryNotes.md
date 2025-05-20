Add files to boot, to enable ssh and wifi connection 
add ssh file (no extension)

add wpa_supplicant.conf file (below)

------------------------------------------------------
country=CA
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1


network={
    ssid="Network_name"
    password="whateverthepasswordis"   #Wifi password
}

(Have multiple network blocks to connect to multiple networks, the PI will connect to whichever one works in the moment)

------------------------------------------------------
# REMOTE access into raspberry from PC

1. open terminal on PC
2. command: ssh username@hostname.local 
3. say yes and enter password
4. Now you are in the RP 
-----------------------------------------------------------------------------------------------
# Common PI commands:
**sudo apt-get update (updates all of the applications on the pi)**
**sudo apt-get up (same as above)**

cat your_file.py (to see contents of file on terminal)

rm myscript.py  (DELETE file)

checking wireless interface name: 
ip a

## Using a virtual environment

activate: **source venv/bin/activate**

installing the dht library: pip install adafruit-circuitpython-dht

Deactivating: **deactivate**


return SSID of network pi is connected to: 
iwgetid -r

-----------------------------------------------------------------------------------------------

# How to change WIFI settings within the PI

1. sudo nano /etc/wpa_supplicant/wpa_supplicant.conf   (goes into wpa_supplicant file which connects to network!)

2. Press Ctrl+O to save the file.
   Press Enter to confirm.
   Press Ctrl+X to exit Nano.
3. sudo wpa_cli -i wlan0 reconfigure   (Tell wifi system to re read rhe config file and apply new settings)

(might have to change settings for it to reconfigure)

-----------------------------------------------------------------------------------------------

# Connecting VSCODE to the PI

Use remote connection
1. add an ssh file in C:\Users\<YourUsername>\.ssh\config on Windows
2. Ctrl+Shift+P on vscode then type and Select "Remote-SSH: Connect to Host..."
3. chose host, press linux 
4. log in with PI password

-----------------------------------------------------------------------------------------------
# Start VcXsrv for PC server to run the GUI remotely!

After installation, open VcXsrv. You can do this by searching for “VcXsrv” in the Windows Start menu.

In the configuration window, select "Multiple windows".

Ensure "Start no client" is selected.

Click Next through the default options, then click Finish.

VcXsrv will start and run in the background (you may see its icon in the system tray).

-----------------------------------------------------------------------------------------------

# Using PuTTY (session should be saved)

Session: 

enter hostname

port: 22

connection> ssh> X11   enable X11 forwarding:
x display location: enter localhost:0.0

-----------------------------------------------------------------------------------------------
# CO2 Sensor 
On pi in terminal (outside venv)

sudo apt update

sudo apt install -y pigpio python3-pigpio

sudo systemctl enable pigpiod    **Make sure pigpiod daemon starts now and at each boot**

sudo systemctl start pigpiod

Then inside VENV install pigpio package for pwm version of using sensor 

pip install pigpio

-----------------------------------------------------------------------------------------------
# VOC sensor

Connecting through USB-C 

Board comes up as: ttyACM0

Verify device node: ls -l /dev/ttyACM0

Then you can launch minicom from your normal shell (even while your venv is active) with:
    minicom -D /dev/ttyACM0 -b 9600
you can see your boards command menu with this**

To exit: Ctrl-A then X, confirm.

