# SSA
Secure Architecture Coding output

Goup 1:
Abidemi Adelakun,
Elizabeth Cook,
Haseeb Abdulhak,
Nils Linhoff

# Objective:
This assignment is to demonstrate the interactions between a smart server device (server.py) and client device (client.py). 

A prototype server and client have been created which replicates an Amazon echo controller and smart light client devices. The client device controls turning light switches on and off for each room and sends the information to the server which then knows which rooms have lights switched on or off.

# Language Used: 
Python 3.10

# Libraries Used: 
Tabulate 
Pickle
Threading
Socket

# Installation & Run
Install server.py and client.py files
Install all libraries required
-	Open terminal for the server and run using >>> python3 server.py
-	Open a terminal for the client and run using >>> python3 client.py
-	Enter your name into the client terminal 
-	Enter the name of the room that you want to turn the light on or off
-	Choose from:
‘kitchen’
‘bath’
‘bedroom’
‘hall’
-	Enter ‘on’ or ‘off’ 
-	Message will display ‘Your inputs are successfully sent to the server’ showing the action as been completed
-	Check the server terminal for information of each room and whether the light is ‘on’ or ‘off’
-	This process can be repeated for each room 
A video demonstration has also been provided to show this process in action

# Security Features 
Socket programming has been used to create the connection between client and server devices

Messages are transported using TCP in socket programming, SSL/TLS should be added to improve security of the data.

Data that is input into the client protype is validated and only certain data will be accepted. This prevents against SQL injection to the server and buffer overflow

# Testing
Full detail and screenshots of testing completed is available in the Code Testing file provided

User testing has been carried out to ensure all inputs of ‘on’ and ‘off’ for each room work 

Input of anything other than ‘on’ or ‘off’ will return an error message of ‘you input wrong data, light should be On or Off’

Pylint & pycodestyle tests were run against both server.py and client.py files to ensure code followed python code style best practices and changes were made to improve the score 

# Adaptions from the original design
Our design document stated the use of a speaker client device; however it was difficult to replicate a prototype and only offered the option of music on/off. We decided to focus on a smart light so that we could incorporate different room options as well as on/off data.

# References
Real Python (2022). Socket Programming in Python (Guide). Available at: https://realpython.com/python-sockets/ 

