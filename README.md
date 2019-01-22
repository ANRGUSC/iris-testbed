# iris-testbed
Intelligent Robotic Internet of Things TeStbed (IRIS) - Links and Documentation

Autonomous Networks Research Group (ANRG)

University of Southern California

Welcome to the main IRIS repository where you can find the code, documentation, 
and pcb designs related to the open source IRIS testbed. There are many modular 
parts of the IRIS testbed that may be useful for researchers, and, because the 
maintainers are currently low on bandwidth, we ask strongly encourage the 
community to please submit a Github issue to request further documentation or 
help on how to recreate any to all parts  of the IRIS testbed.

## Repositories:

[IRIS-RIOT](https://github.com/ANRGUSC/iris-riot) - A fork of RIOT-OS with all 
RIOT related IRIS testbed application code.

[IRIS-mbed-os-3pi](https://github.com/ANRGUSC/iris-mbed-os-3pi) - IRIS testbed
application code built on mbed OS for the mbed LPC1768 platform and code for
the Pololu 3pi base (atmega328p MCU).

One very useful piece to the community is the IRISbot's MCU to MCU communication 
via HDLC over UART. We have implemented cross-comaptible libraries for both 
RIOT-OS and mbed OS for sending HDLC packets in a multi-threaded environment.
For the RIOT-OS implementation:

[RIOT-OS HDLC Implementation](https://github.com/ANRGUSC/iris-riot/tree/develop/sys/net/link_layer/hdlc)

[RIOT-OS HDLC Tests](https://github.com/ANRGUSC/iris-riot/tree/develop/examples/iris_testbed/tests/hdlc_txvr)

For the mbed OS implementation:

[mbed OS HDLC Implementation](https://github.com/ANRGUSC/iris-mbed-os-3pi/blob/develop/hdlc.cpp)

[mbed OS HDLC Tests](https://github.com/ANRGUSC/iris-mbed-os-3pi/tree/develop/app_files/hdlc_test)


## PCB Designs

Please see the `pcb_designs` folder to find the .brd and .sch files (Eagle) of 
the various PCB designs for the IRISbots. Since the publishing of our original
paper, we have upgraded the triple sensor board to a quadruple sensor board 
because we found using three sensors for omnidirectional localization resulted
in sporadic blindspots. The layouts have also been simplified to reduce the 
number of needed jumper cables.

## Video Links

[IRIS Trilateration](https://www.youtube.com/watch?v=-iA_I1HjI5E)

[IRIS Chain Test](https://www.youtube.com/watch?v=XQomuFSqbBQ)

## IROS 2018 Presentation Slides:

https://docs.google.com/presentation/d/1Dmg364Kt8fulA3RI1eVobmNLkZHoMGymSkHf-HZB2n8/edit?usp=sharing

## References:

Jason A Tran, Pradipta Ghosh, Yutong Gu, Richard Kim, Daniel D’Souza, Nora 
Ayanian, Bhaskar Krishnamachari, 
"[Intelligent Robotic IoT System (IRIS) Testbed](https://anrg.usc.edu/www/wp-content/uploads/2018/09/Intelligent_Robotic_Iot_System_Testbed__IRIS_-4.pdf)",
in IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 
Oct, 2018.
