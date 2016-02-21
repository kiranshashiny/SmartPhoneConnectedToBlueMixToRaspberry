# SmartPhone App communicating to IBM BlueMix using MQTT, and sending to devices like Raspberry Pi
# and controlling a DC geared motor, and a LED remotely.

This project was about connecting the Smartphone to IBM Bluemix thru MQTT and connecting to Raspberry Pi at the other end.

Here I have used concepts from Evothings - which has developed the Workbench to create Apps for SmartPhone, 
MQTT Broker from IBM Bluemix, to receive Publish commands from the Smartphone, and the Raspberry Pi which is configured to receive and act on the commands being sent from the Smartphone.

I have combined functionality to handle LEDs and some motor controls of a small geared 12V DC motor.
The motor is powered and energized by a L293D chip which has ability to control 2 motors based on signals from the Raspberry Pi.

The Raspberry Pi I have is a Model B, is the device that I have configured on the IBM Bluemix IoT dashboard.
