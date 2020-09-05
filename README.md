# Simulation-of-Fast-Ethernet

This project is to simulate the Fast Ethernet. The goal of the project is to practice basic socket AP programming
through a client/server application.

• Fast Ethernet is simulated by multiple processes on multiple machines and each station in the Ethernet is
simulated by a process.

• The switch of the fast Ethernet is also simulated by a process. These processes can run on different workstations
in the Linux lab.


Program files:
==============
CommunicationBusProcess.c
StationProcess.c

Simulation input files for Station Process:
==========================================
station_process1.txt
station_process2.txt
station_process3.txt
station_process4.txt
station_process5.txt
station_process6.txt
station_process7.txt
station_process8.txt
station_process9.txt
station_process10.txt

Output log file of CommunicationBusProcess:
==========================================
Communication_Bus_Output.txt

Output log file of StationProcess:
==================================
Station_Process_Output.txt


Steps involved in compiling and Running the Project:
===================================================

STEP1:
=====
Path of the folder where I have done the Project in my UNIX account.
"/home/Students/j_k201/public_html/unpv13e/Networks_Project"

STEP2:
=====
Compile the CommunicationBusProcess.c program:
"gcc -std=c99 -o  CommunicationBusProcess CommunicationBusProcess.c"

STEP3:
=====
Complie the StationProcess.c program:
"gcc -std=c99 -o  StationProcess StationProcess.c -lm"

STEP4:
=====
Execute the CommunicationBusProcess.c program:
"./CommunicationBusProcess <ANY PORT NUMBER> &" 

STEP5:
=====
Execute the StationProcess program for different stations simultaneously:
"./StationProcess 127.0.0.1 <PORT NO> <STATION NUMBER> & ./StationProcess 127.0.0.1 <PORT NO> <STATION NUMBER> & ./StationProcess 127.0.0.1 <PORT NO> <STATION NUMBER>"
