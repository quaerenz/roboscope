ROBOSCOPE

Our team decided to create a network of autonomous robotic telescopes that monitors the sky autonomously based on real data from NASA (JPL Horizons), thus amateur astronomers around the world can use our system to monitor and make a record of the asteroids that threaten to our planet. We have created hardware for amateur telescopes, we have developed software to control the telescope and to obtain data of hazardous asteroids, and we have created a website/server to bring support to our system. 

Our main goal is to have a network of autonomous robotic telescopes around the world that monitors the sky autonomously looking for potentially hazardous asteroids (PHAs). The main features of the system that we have developed are:

• Hardware: Design and implementation of a cheap robotic mount usually used by amateur telescopes. It has been done with inexpensive materials, an Arduino UNO board and recycled stepper motors; in order to allow other users to replicate it and work with our project providing useful data to NASA and other observation projects looking for PHAs. It is advisable to use a special camera CCD or CMOS attached to the telescope, as we presented in our prototype. The goal of our project is that other users around the world will be able to replicate our hardware and/or improve it.

• Software: We developed an open source standalone application in Java that accesses into a database of asteroids from NASA (JPL's HORIZONS system) using telnet and under certain criteria, we use filters to search into the databse like: perihelion<1.3au, aphelion>0.7au, dimension>100m, and so on. According to the selected asteroids list an observation schedule is planned daily sending instructions to the telescope via USB cable. The program will perform the conversion of respective celestial coordinates from NASA database into the local autonomous telescope system. This application also controls the camera attached to the telescope and based on catches, processes the image pixel by pixel to identify the asteroid and after that send these images with additional information of them to our website/server. Future improvements of our software can be to calculate the MOID parameter.

• Website: Our website allows to all amateur astronomers in the world to sign up in our database and registering their user data and location. Our webpage also gives our tutorials step by step to create the robotic mount of telescope, direct downloads of our software and further information related with our project. In this website we have an FTP server that include images files and other real data of potentially hazardous asteroids provided by users around the world.
