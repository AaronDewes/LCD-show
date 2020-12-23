# LCD screen drivers

### Installation on Ubuntu
https://github.com/lcdwiki/LCD-show-ubuntu

### Installation on Kali Linux
https://github.com/lcdwiki/LCD-show-kali

### Installation on RetroPie
https://github.com/lcdwiki/LCD-show-retropie

## Installation on the Raspberry Pi
  
This tutorial assumes you already have Raspbian installed.

### Step 1: Download the scripts
Use SSH to connect the Raspberry Pi. 
When you're successfully connected to the Raspberry Pi, run these commands:

```
sudo rm -rf LCD-show
git clone https://github.com/AaronDewes/LCD-show.git
chmod -R 755 LCD-show
cd LCD-show/
```
  
### Step 2: Install the drivers

Now install the driver for your screen using the script that fits for it.

For example, this installs the driver for a 2.4” screen. 

```
sudo ./LCD24-show
```


# How to rotate the display direction

The display direction can be easily rotated if the drivers are installed using this script:

```
cd LCD-show/
sudo ./rotate.sh 90
```

After execution, the system will automatically restart, and the display screen will rotate 90 degrees to display and touch normally.<br>
( ' 90 ' can be changed to 0, 90, 180 and 270, respectively representing rotation angles of 0 degrees, 90 degrees, 180 degrees, 270 degrees)<br>
(If the rotate.sh prompt cannot be found, use Method 1 to install the latest drivers)



