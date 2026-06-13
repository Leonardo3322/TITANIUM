# TITANIUM
We are the Titanium team, representing UEISA (Unidad Educativa Instituto San Antonio). We are made up of Leonardo Da Silva, a 5th-year student, and Guillermo Pacheco, a 3rd-year student. We have focused on working hard and together to achieve all our goals, overcome any difficulties we encounter, and support each other in our projects. This robot is one of those projects, and we are very proud to be able to present it to you.
# Índice
* [Repository Contents](#Repository-Contents)
* [Project Introduction](#Project-Introduction)
* [First model](#First-Model)
* [Photos of our Team](#Photos-of-our-Team)
* [Vehicle Photos](#Vehicle-Photos)
* [List of components used](#List-of-components-used)
* [List of components tested but discarded](#List-of-components-tested-but-discarded)
* [Hardware design](#Hardware-Design)
* [Software design](#Software-Design)
	* [Brief summary of our evolution](#Brief-summary-of-our-evolution)
* [GPIOZERO schematic](#GPIOZERO-schematic)
* [electrical components for detection and motion ](#Electrical-components-for-detection-and-motion)
* [processing components](#Processing-Components)
* [power components](#Power-Components)
* [refrigeration system](#Refrigeration-System)
* [Electronic connection diagram](#Electronic-connection-diagram)
* [How we put together the robot](#How-we-put-together-the-robot)
	* [first phase](#First-phase)
* [creation of the tracks](#Creation-of-the-tracks)
* [Techbot robot video ](#Techbot-robot-video)
# Repository Contents
## Our repository contains the folllowing team data:
|File|Description|
|------|------|
| [`T-photos`](https://github.com/Leonardo3322/TITANIUM/tree/main/T-photos) | Includes team photos |
| [`V-photos`](https://github.com/Leonardo3322/TITANIUM/tree/main/V-photos) | Includes Vehicle photos |
| [`Videos`](https://github.com/Leonardo3322/TITANIUM/tree/main/Videos) | |
| [`Schemes`](https://github.com/Leonardo3322/TITANIUM/tree/main/Schemes) | Schematic diagram (PNG) of the electronic connections from the Raspberry to the components|
| [`SRC`](https://github.com/Leonardo3322/TITANIUM/tree/main/SRC) | All the folders with the tests and practices that the team has done throughout the development of the robot along with a brief history of how we evolved and changed the codes along the way |
| [`Models`](https://github.com/Leonardo3322/TITANIUM/tree/main/Models) | This folder is empty because our robot does not need 3D printing or virtual modeling |
| [`Others`](https://github.com/Leonardo3322/TITANIUM/tree/main/Other) | It contains a list of components we've used, components we've tested and discarded because they didn't work as needed, and components that were implemented in the final version of the robot. It also includes two folders, one containing all the photos and the other containing all the recorded videos |
# Project Introduction
# First Model

# Photos of our Team
| **TITANIUM TEAM** | Guillermo Pacheco and Leonardo Da Silva |
| ![Titanium_team](https://github.com/Leonardo3322/TITANIUM/blob/main/T-photos/Titanium%20Team.jpg)|
# Vehicle Photos
# List of component used
| **Name** | **Description** | **Image** |
|----------|-----------------|-----------|
| **3D Printed Bases** | Es una base en la cual se mantienen las direccionales, sensores y los propios soportes del nivel superior (nivel de abajo), en la parte de arriba se mantienen ciertos cables, la rasberry, entre otros. | ![Base](https://github.com/Leonardo3322/TITANIUM/blob/main/Other/IMG_20260526_143939_edit_1394414993818421.jpg) |
| **Raspberry Pi5**|The motherboard - the robot's brain. Features: 8GB RAM, 4GB ROM, dual 4K GPU support, PCI Express interface. Ports: 2x HDMI, 4x USB (2x USB2.0 + 2x USB3.0), Gigabit Ethernet, 27 programmable pins (2x 3V, 2x 5V, 8x GND), USB-C power, microSD slot. Power: 5V-3A (min) to 5V-5A (max)|![Raspberry_Pi5](https://github.com/Leonardo3322/TITANIUM/blob/main/Other/raspberry-pi-5-03.jpg)|
| **Hexagonal Pillar Screw Kit**|Used to create structural pillars enabling two levels: Lower (motors/directional components) and upper (wiring, Raspberry Pi5, battery, breadboard, sensors)|![Hexagonal_Pillar_Screw_Kit](https://github.com/Leonardo3322/TITANIUM/blob/main/Other/Hexagonal_screw_kit_for_pillars.jpg)|
# List of component but discarded
| **Name** | **Description** | **Why it was discarded** | **Image** |
|----------|-----------------|--------------------------|-----------|
|**Diferencial**|It allows that when the motor rotates, a wheel goes in the same direction or goes in the opposite direction.|It was discarded because it was too rigid and too large for the robot.| ![Differential](https://github.com/Leonardo3322/TITANIUM/blob/main/Other/Differential.jpg)|
# Hardware Design
| **Name** | **Description** | **Image** |
|----------|-----------------|-----------|
| **3D Printed Bases** | It is a base that holds the directional components, sensors, and the supports for the upper level (lower level) themselves. On the top part, certain cables, the Raspberry Pi, and other things, are kept.| ![Base](https://github.com/Leonardo3322/TITANIUM/blob/main/Other/IMG_20260526_143939_edit_1394414993818421.jpg) |
| **Raspberry Pi5**|The motherboard - the robot's brain. Features: 8GB RAM, 4GB ROM, dual 4K GPU support, PCI Express interface. Ports: 2x HDMI, 4x USB (2x USB2.0 + 2x USB3.0), Gigabit Ethernet, 27 programmable pins (2x 3V, 2x 5V, 8x GND), USB-C power, microSD slot. Power: 5V-3A (min) to 5V-5A (max)|![Raspberry_Pi5](https://github.com/Leonardo3322/TITANIUM/blob/main/Other/raspberry-pi-5-03.jpg)|
| **Hexagonal Pillar Screw Kit**|Used to create structural pillars enabling two levels: Lower (motors/directional components) and upper (wiring, Raspberry Pi5, battery, breadboard, sensors)|![Hexagonal_Pillar_Screw_Kit](https://github.com/Leonardo3322/TITANIUM/blob/main/Other/Hexagonal_screw_kit_for_pillars.jpg)|
| **Camera** | It is the fundamental part of the robot that allows it to distinguish distance and colors, which it detects in conjunction with other sensors. | ![Camera](https://github.com/Leonardo3322/TITANIUM/blob/main/Other/Camera.jpg)|
| **Ultrasound sensor** | This sensor was used to detect walls to achieve a more fluid and safe movement, preventing collisions and jamming. | ![Ultrasound_sensor](https://github.com/Leonardo3322/TITANIUM/blob/main/Other/ultrasound_sensor.jpg)|
| **Motor Module** | The module acts as an electronic bridge between a low-power controller (such as a microcontroller or Arduino) and an electric motor. It amplifies the control signals to provide the current and voltage necessary to operate the motor safely and precisely. | ![motor_module](https://github.com/Leonardo3322/TITANIUM/blob/main/Other/motor_module.jpg)|
| **Protoboard and Dupont Cables**| Is a reusable prototyping board used to build and test temporary electronic circuits without soldering. And the dupont cables serve the primary function of interconnecting electronic components without soldering. | ![Protoboard_and_Dupont_cables](https://github.com/Leonardo3322/TITANIUM/blob/main/Other/ProtoBoard_and_Dupont_cables.jpeg)
# Software Design
## Brief Summary of our evolution
## GPIOZERO Library
## GPIOZERO Schematic
## Time Library
# Detection System
# Electrical components for detection and motion
# Procesing Components
| **Name** | **Function** | **Image** |
| -------- | ------------ | --------- |
| Raspberry Pi 5 | The Raspberry is the brain of the entire robot, allowing the programming to be saved and also executed, which allowed us to implement different commands. Without this control board, nothing would be possible; the robot simply wouldn't know what to do | ![Raspberry_Pi5](https://github.com/Leonardo3322/TITANIUM/blob/main/Other/raspberry-pi-5-03.jpg)|
# Power Components
# Refrigeration System
# Electronic Conection Diagram
# How we put together the robot
## First fase
In this first phase, the goal was to use 3D bases to mount all the sensors, the Raspberry Pi 5, the power bank, and the remaining components onto it, and to provide stability to the robot. However, the option of using pre-made acrylic bases is still being considered.
# Creation of the tracks
# Techbot robot
## Video of the first titanium test
