# Pi0_cameraStream
tutorial on how to connect a Pi camera to a Pi 0
Materials:
1) Pi Zero (refer to this diagram): ![zero-w-ports](https://user-images.githubusercontent.com/64620878/153735453-37cab166-d3c8-494b-bfec-f9d016103335.jpg)
2) Ribbon cable![IMG-3165](https://user-images.githubusercontent.com/64620878/153735462-ede12947-24c7-4985-bd99-b18b787d19c8.jpg)
3) HDMI cable![IMG-3164](https://user-images.githubusercontent.com/64620878/153735470-b7b01379-6aef-411d-a5be-61ad4980fe73.jpg)
4) HDMI mini connector ![IMG-3168](https://user-images.githubusercontent.com/64620878/153735474-d28a93f7-4f6d-468f-91a1-e67d858cc2b0.jpg)
5) Monitor
6) cable mouse
7) cable keyboard
8) laptop

Steps

Initial Setup
connect the pi zero to the power in cable through the PWR in Port
Connect the HDMI cable to the HDMI mini connector and connect the male end of the HDMI mini connector to the HDMI port of the pi zero
Get your monitor (make sure it's plugged in) connect your HDMI cable to the Hdmi port of your monitor 
Turn on your pi zero( button should be on the power cable)

Enabling Camera and SSH
Open up terminal and type sudo raspi-config
Open interfacing options and enable camera
Next go to Interfaces and enable SSH
Go back to terminal and type ifconfig, the second line should be the Pi 0’s ip address (it should be something like 192….)
Go to your laptop and open terminal. Type ssh pi@”the ip address” (make sure that your laptop and pi 0 are on the same wifi)
Password is raspberry
Type yes

Connecting the Camera
Connect the ribbon cable to the Camera (metal to metal) and connect the other end of the ribbon cable to the Pi 0’s camera port (metal to metal)


![2016-05-15-16 32 19-500x375](https://user-images.githubusercontent.com/64620878/153738258-09239336-ec68-4e2c-8e21-a18802943c8c.jpg)


Streaming video
 Download  the following into the laptop terminal:
sudo apt-get update

sudo apt-get upgrade

sudo apt-get install libatlas-base-dev

sudo apt-get install libjasper-dev

sudo apt-get install libqtgui4

sudo apt-get install libqt4-test

sudo apt-get install libhdf5-dev

sudo pip3 install Flask

sudo pip3 install numpy

sudo pip3 install opencv-contrib-python

sudo pip3 install imutils

sudo pip3 install opencv-python

	

