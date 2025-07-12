# TOBB ETÜ ELE495 - Capstone Project

# Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Screenshots](#screenshots)
- [Acknowledgements](#acknowledgements)

## Introduction
This project aims to design NLP Autonomous mini vehicle capable of recognizing Turkish spoken natural language commands and translating them into fundamental motion instructions to help people to control a vehicle with no touch. In this way, the vehicle enhance usability and alleviate the user workload in task-oriented applications such as military technologies and the service sector with voice-based controls.

## Features
- Hardware: 
MPU6050 6 Axis Gyro Sensor    https://www.alldatasheet.com/html-pdf/1132807/TDK/MPU-6050/413/6/MPU-6050.html
L298N DC Motor Driver         https://www.alldatasheet.com/datasheet-pdf/pdf/22440/STMICROELECTRONICS/L298N.html
Raspberry Pi Model 4B         chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://datasheets.raspberrypi.com/rpi4/raspberry-pi-4-datasheet.pdf
HC-SR04 Ultrasonic Sensor     https://www.alldatasheet.com/datasheet-pdf/pdf/1132204/ETC2/HCSR04.html
Anker Powerbank 10000mAh      https://www.trendyol.com/anker/powerbank-10k-30w-c-l-siyah-a1680-p-881913944
Lion Battery x2 3.7V 18650    https://www.aspilsan.com/en/cozumler/uretimini-yaptigimiz-sarj-edilebilir-lityum-iyon-pil/inr18650a28/

- Operating System and packages
Raspberry Pi OS

- Applications
Python 3.11.2

- Services 
Google Speech Recognition API
OpenAI
ElevenLabs

## Installation

import RPi.GPIO as GPIO  Its used to activate Raspberry Pi pins to control circuit modules; HC-SR04, MPU6050, L298N
import smbus2 as smbus   Its used to ...
from resemblyzer import VoiceEncoder, preprocess_wav   It is used to recognize voice of group members
import numpy as np                                     It is used in recognition process....
from elevenlabs.client import ElevenLabs               It is used in TTS 
from elevenlabs import save, play                      It is used in TTS to play and save user voice    
import os,                                             It is necessary for file operations
re,                                                    It is used to match motion functions to strings of commands  
subprocess,                                            It is used in settings of user voice record
openai,                                                It is used in STT(Speech to text) procces and interpretting commands
time,                                                  It is used for holding time                                                   
json,                                                  It is used to send information to User Interface(UI) 
socket,                                                It is used to built TCP connection  user interface and vehicle
threading                                              It is used in multi - processing operations  



```bash
# Example commands
git clone https://github.com/username/project-name.git
cd project-name
```

## Usage
Provide instructions and examples on how to use the project. Include code snippets or screenshots where applicable.
1- User Interface is initialized
2- Click "Kaydı Başlat" button to start recording your commands and speak
3- Click "Kaydı Durdur" button to stop recording and wait for the response 
4- Check the User Interface to follow given and executing commands  

## Screenshots
Youtube Link:  https://www.youtube.com/watch?v=83Itll7FwYU  
images were added on a different file named with "suno_images" on repository.


## Acknowledgements

TOOLS & RESOURCES APPLIED
https://www.youtube.com/watch?v=V0CKi89dTcM
https://www.youtube.com/watch?v=wTfSfhjhAU0

THANK-YOU PART
We would like to express my sincere gratitude to everyone who supported our group during the development of this project. We especially thankful to my teammates for their collaboration, to my mentor Murat SEVER for their valuable feedback and guidance, and to the Lecturer Zeki KOCABIYIKOGLU that provided the working environment. This project has become stronger thanks to the shared knowledge and collective effort.

[Contributor 1](https://github.com/aliemirhaneskicioglu)
[Contributor 2](https://github.com/bmertgocer)
[Contributor 3](https://github.com/berkeserileli)
[Contributor 4](https://github.com/alperaltiparmak)
[Contributor 5](https://github.com/agokcel)
[Resource or Tool](https://www.nvidia.com)
