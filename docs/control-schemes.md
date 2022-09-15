# Control Schemes
This page will detail the various ways to interface with Tello and Tello EDU drones. This page will only provide a brief description of how to communicate

## DJI Tello App
The simplest option for getting your drone flying is to use the [Tello App](https://www.dji.com/au/downloads/djiapp/tello). This app is available for both Android and IOS devices. With this app you will be able to control the drone using on screen control sticks, view a live feed from the camera, and perform various functions. The [Tello user manual](https://dl-cdn.ryzerobotics.com/downloads/Tello/Tello%20User%20Manual%20v1.4.pdf) details these functions.

## Tello SDK
The tello SDK is the lowest level at which you can interact with the drone. It uses UDP packets to send commands to the drone. Once connecting to the drone's wifi access point (AP), in a default configuration the user can send text commands through UDP port `8889` to `IP 192.168.10.1`.

## Programming
### Droneblocks
This is the most basic method for programming the Tello drones. [Droneblocks](https://learn.droneblocks.io/) uses block coding to abstract the aforementioned SDK functions with simple drag and drop programming. It includes a simulator for testing code without a drone and is a very good introduction to learning the basic principles of programming without having to learn complex syntax. It is comparable to other products like scratch.

### djitellopy
DJITellopy is a python library for working with the tello drones.