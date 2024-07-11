---
layout: page
authors: ["Jannetta Steyn"]
teaser: "The Intro to IoT lesson is available in the Carpentries Incubator and uses the new Carpentries Workbench."
title: "IoT for Novices in South Africa"
date: 2022-12-7
time: "09:00:00"
tags: ["Africa", "Carpentries Incubator"]
---
*Originally posted on the [Society of Research Software Engineering](https://society-rse.org/iot-for-novices-in-south-africa/) website, 
this blog post highlights an Introduction to the Internet of Things workshop hosted 
at Stellenbosch University, South Africa.* 

The Internet of Things (IoT) is one of the buzzwords that researchers would like to include in their research and grant applications, 
but few actually understand what it is. So, when I was asked by Kim Martin whether I could run a workshop at Stellenbosch University in 
South Africa to introduce a group of curious researchers to this thing they are hearing so much about I immediately agreed – as usual 
before completely thinking it through. I am not an IoT expert but merely an enthusiast that likes playing around with microcontrollers, 
sensors and computery things such as Raspberry Pis. I am also a research software engineer and I immediately saw an opportunity to introduce 
research software engineering to researchers – not only because the workshop is being presented by an RSE but also to tell them how an RSE 
can benefit their research.

Kim Martin is a Post-doc and an SSI Fellow at Stellenbosch University. Kim’s fellowship involves connecting African researchers with 
UK-based RSEs, to provide the former with targeted RSE consulting in service of writing higher-impact grant applications. I was already 
on my way to Stellenbosch to run a Software Carpentries workshop and to test CarpentriesOffline (see https://carpentriesoffline.org), 
which is the subject of my SSI Fellowship which meant everything was working out well to kill two birds with one stone.

Prof Thinus Booysen, Engineering and Research Chair in Internet of Things at Stellenbosch University, made some ESP32 microcontrollers 
and humidity/temperature sensors available. For a venue Kim approached the Stellenbosch University Makerspace and the National Institute 
for Theoretical and Computational Sciences (NITheCS) offered to provide the catering.

My first task was to develop a Carpentries-style lesson. There was already an IoT lesson in the Carpentries Incubator, but it focused on 
the use of an Arduino to build a weather station and not so much on exactly what IoT is. To really explain what IoT is and how it works 
one really needs a microcontroller that has WiFi functionality. The ESP32s that Prof Booysen made available already have WiFi onboard and 
has the advantage of being almost 3 times cheaper than an Arduino nano 33 IoT – which make it a more viable option in case leaners want to 
continue their IoT adventure after the workshop.

Thus, I developed a lesson that would use ESP32s rather than Arduinos but still using the Arduino IDE. The lesson covers the connection of 
two sensors, the DHT11/22 for temperature and a light dependent resistor (LDR) for light intensity to an ESP32. The code for reading the 
temperature and the light intensity can be copied from the lesson material. Depending on the time available the instructors can explain how 
the code works in more, or less, detail. After covering the basic code, the learners then copy the code for connecting the microcontrollers 
to the WiFi. Connecting devices to a university’s network can be problematic. For instance, at Stellenbosh University all computers that need 
to connect to the Internet must have their MAC addresses added to the network by the IT department – not a feasible option for a temporary 
setup of 20 microcontrollers.

Fortunately, the solution is not too difficult. Since I had a couple of Raspberry Pis ready for the CarpentriesOffline workshop, I could use 
one of them to create an access point. It wasn’t essential for the success of the workshop, but the IT department agreed to add the MAC address 
of one Raspberry Pi. In case this couldn’t happen, I installed an MQTT server on the RaspBerry Pi. Norman Hebler, head of the Makerspace, kindly 
installed the MQTTx client on the Makerspace PCs and students who wanted to use their laptops could install it themselves. MQTTx is free and 
very lightweight.

While the thinking juices were flowing, I also remembered that SocRSE had the Events and Initiatives Grant. I realised that if I could get the 
grant, it would mean that, firstly, while in South Africa I would have the extra bits of kit that we would need for the workshop such as connector 
cables, light sensors and breadboards. Secondly, it would mean that I could run the same workshop when I am back in the UK. I was elated when SocRSE 
informed me that my application was successful. With the grant I purchased ESP32 WROOM 32Ds, a few Arduino Nano 33 IoTs, some Raspberry Pi Pico Ws, 
Sensor Module Kits, Digital sensor temperatures, mini breadboards, loads of jumper cables (experience dictates that you can never have enough of 
those), USB cables, a power strip tower (because you never have enough power sockets) and a case to put it all in.

Our workshop went really well. We had the help of Norman as well as Keegan Hull, a Masters student at Stellenbosch. Our days were rather short, 
running from 10:00 to 16:00 with an hour for lunch and a couple of coffee breaks, we only had 4.5 to 5 hours a day for two days. Not sure whether 
we’ll be able to complete the lesson we only connected the temperature sensors at first and then did the part on connecting to the MQTT server. 
However, in the end there was enough time to add the LDRs too and learners could subscribe to data being published by the MQTT (RPi) server, 
using MQTTX. With a little more time it should be possible to discuss the code in more detail but since the lesson is aimed at researchers with 
no programming experience, explaining the code has to be at a fairly high level.

The Intro to IoT lesson is available in the Carpentries Incubator and uses the new Carpentries Workbench 
(see https://carpentries-incubator.github.io/iot-novice/). The last couple of episodes of the lesson still need to be “padded” with explanatory text. 
Because I was running out of time to get the lesson done before the workshop, I just wanted to make sure the necessary code and images were in place. 
We picked up the odd spelling and grammar errors that also need to be fixed and the lesson could also do with some notes for instructors.

I plan to run at least one of these workshops in the next four months at Newcastle. We also have a Code Community where I would like to give a 
presentation and if I can think of a version of the lesson that one can fit into an hour or two, I might make it a hands-on session. If anyone is 
interested in piloting the workshop at their institution and would like for me, and my kit, to help out, please be in touch. If you would like to 
contribute to the lesson in any way please be in contact, look at the lesson and create and issue or a pull request.

We would like to thank the following people for their help in piloting this workshop at Stellenbosch University:

- Dr. Kim Martin, for organising the workshop and testing the lesson material.
- Prof Thinus Booysen, Engineering and Research Chair in Internet of Things at Stellenbosch University,
- Norman Hebler Head of the Stellenbosch University Makerspace
- National Institute for Theoretical and Computational Sciences (NITheCS)
- Keegan Hull for being a helper at the workshop
- The Society of Research Software Engineering for granting me the funds to obtain the kit I needed to develop the lesson, pilot the workshop at Stellenbosch and hopefully run several more workshops in the future.
