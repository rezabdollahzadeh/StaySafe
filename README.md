# StaySafe 

StaySafe is a Android app to warn people of dangerous animals in the area.

## Why StaySafe?

StaySafe is the android application to the IoT based, Image Processing project on Raspberry Pi. This app notifies users about the location where the leopard has been detected in real-time and also provides an SOS button and Emergency Contacts. This way, users can stay away from areas where leopards are detected frequently.
 
<p align = "center"> <br/>
<img align="left" src="images/main_screen.png" alt="Main Screen" width="350px" height="739px">
<img align="right" src="images/leopard_detected.png" alt="Leopard Detected" width="350px" height="739px">
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/></p>

## The Motivation
StaySafe was created as part of 'Safty and Security in IIITDM Jabalpur', a project for DS302 - Engineering Design. Primarily, the idea was made because of all the security concerns related to wild animals, in this case, leopards.

## Working
The applicaion conains a map with location of every Security Guard Checkpoint marked as a flag. If at any point, a leopard is detected, it is updated in the Firebase Database under 'leopard/level' is marked "1". After 2 minutes, this data value will turn zero automatically.

<p align = "center"> <br/>
<img align="center" src="images/database.png" alt="Database">
<br/>
 
 The Image Processing that is used to detect leopaprds can be found on [this repository](https://github.com/arnav-deep/leopard-detection).

Whenever 'leopard/level' equals to "1", a notification is pushed by the app.
