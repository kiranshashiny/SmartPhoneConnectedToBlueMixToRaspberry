# SmartPhone App publishing to IBM BlueMix using MQTT. Raspberry Pi Microcontroller at the other end subscribing to these commands from IBM Bluemix MQTT Broker and controlling a DC geared motor, and a LED.

This project is about connecting the Smartphone application to IBM Bluemix thru MQTT and connecting to Raspberry Pi at the other end.
In this project I have a LED, and a DC motor connected to the Raspberry Pi and can be controlled by the SmartPhone App.

Here I have used a IDE from Evothings http://evothings.com/ - which has developed the Workbench to create Apps for SmartPhone, 
MQTT Broker from IBM Bluemix to receive Publish commands from the Smartphone, and the Raspberry Pi which is configured to receive and act on the commands being sent from the Smartphone. The LED and the motor is connected to the GPIO ports of the Raspberry Pi.

I have combined functionality to handle LEDs and some motor controls of a small geared 12V DC motor.
The motor is powered and energized by a L293D chip which has ability to control 2 motors based on signals from the Raspberry Pi.

The Raspberry Pi I have is a Model B, is the device that I have configured on the IBM Bluemix IoT dashboard.

First, some background to my account in IBM Bluemix:
- I have created an account in IBM Bluemix.
- Created an application using the default IoT Boilerplate. 

<img src="https://cloud.githubusercontent.com/assets/14288989/13202146/66075b4e-d8b5-11e5-9730-95bfa982e7ad.png" width="200">
- Added a service called "IBM Watson IoT platform" 
- Added my Raspberry pi device to it and set it the IoTFoundation to listen to commands being published by Applications, and devices.

<img src="https://cloud.githubusercontent.com/assets/14288989/13202270/966552dc-d8ba-11e5-9809-8b92020a77a1.png" width ="400">
<br>

Evothings: is a IDE for development of Mobile Apps for Android and iOS, and in this blog I have an Android developed.
Here are some interesting links and a sample snapshot of the Evothings workbench.

<img src="https://cloud.githubusercontent.com/assets/14288989/13202278/df960f50-d8ba-11e5-9d25-0b72f2c212e2.png" height ="200" width ="800">
<img src="https://cloud.githubusercontent.com/assets/14288989/13202269/966111d6-d8ba-11e5-80ac-e617f3bf2850.png" width ="400">
<img src="https://cloud.githubusercontent.com/assets/14288989/13202267/96607cc6-d8ba-11e5-93bf-d5fdc8eaae1a.png" width ="400">


and lastly my application running on the Smartphone. <br>
<img src="https://cloud.githubusercontent.com/assets/14288989/13202336/1d042956-d8bd-11e5-9496-21b592d9fd7e.png" width ="400">

To recreate this environment: Install the Evothings workbench and drag and drop the index.html into the "My Apps" section of Evothings IDE.
Install the Evothings App on your handheld device like an Android or an iOS, Connect and click on 'Run'. This automatically will load the code into the Smartphone and install the application.

One can modify the Connect, disconnect, On, Off, forward, Backward and other methods, and or add new sections to suit their needs.

The hardware in this Raspberry pi project that are demostrated were a) LED b) DC motors:

<img src="https://cloud.githubusercontent.com/assets/14288989/13202397/0367bfa6-d8bf-11e5-83da-44a8976e36aa.png" width ="400">
<img src="https://cloud.githubusercontent.com/assets/14288989/13202396/0364eb50-d8bf-11e5-8060-db3cb40ff3c7.png" width ="400">

