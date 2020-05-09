# DockerProject_MultiTeamCompetitionPlatform
This project is made with the technologies like Docker, RHEL8 and Python3 under which multi teams participate to compete with each other on Intranet and a judging system evaluates the competition.

<h2>OVERVIEW:</h2>
This project deals with the competition platform in which 2 or more teams can participate on their local network and perform their activity or task on the platform known as container. This container is made through DOCKER commands. Once the competition or task gets over, the evaluator or the judge can access to the server of each participant’s container through DNAT.  Since all the containers are independent from each other, participants get the fair chance to compete without any intervention. And the judge from outside can evaluate and declare the best work.
This TUI based platform is easy to use and handy for the participant as well as judge. They can easily interact through this. 

 
Where judging requires authentication before final evaluation while participate option just needs participants to compete.
With the help of basic networking concepts like NAT, Multi-Tenant over the Docker makes this idea of competition platform viable and feasible. Hence the technologies used over this project are:
1.	DOCKER
2.	RED HAT 8
3.	PYTHON 3
4.	NETWORKING
Docker is used to build isolated containers over which a competition will be organised. RedHat 8 is used to implement Linux commands and Python 3 is used to build handy TUI (Terminal User Interface) which is used for interaction with the users whereas Networking is used to connect all the container which helps in evaluation system.


<h2> Project Description</h2>
<h3>PARTICIPANT SECTION:</h3>
To participate, the user have to just give the Team ID and Team Name to compete. As soon the participant enters his details a container for his team is built with its Team Name. In this particular container only he has to perform his tasks.
Hence on entering his details team’s container is made. This way we can make countless no of participants to participate.
 
All the team details are stored inside a python list. This stored data is further used at the time of judging and evaluation. For the safety of the participant’s container data, its data is stored in a volume, which is mounted at the time of container building.
 
The communication between the container and outside world can be made afterwards with the technologies like docker file etc. This will further improve our project accessibility and participant’s convenience and interaction.

<h3>JUDGING SECTION:</h3>
This section deals with the admin section for evaluation and environment management. This section requires authentication before entering. Here the judge can see every participants work and can also delete the existing containers and volumes attached to it.
 
If the password is not correct, the user will be denied entering this section. With the particular container’s IP Address, the evaluation can be made for his work. Once the remarks and marks are allotted, the rankings can be declared.
After the rankings, the platform requires cleaning before the second competition which can be done by deleting all the existing containers and attached volumes.

•	Detaching volumes and containers:
 
•	Team Details:
 
At the end with the help of system IP and active port no., the evaluation can be made by judge. Hence these two things are critically important.


<h3>PROJECT QUALITIES:</h3>
This platform can be used as many times as possible with over hundreds and thousands of participants.
It is very fast, requires even less than a second to configure container’s settings including setting up of volumes.
It is reliable and also backup the data of each container in a volume.
It is secure, as a proper measures for authentication is required from each user, without which he will not be able to operate.
Basic idea behind this is the concept of “isolation” and “multitenancy”.
This platform can be used to perform any kind of competitions like coding, web development, web Apps, etc. 
 
<h3>PROJECT CONSTRAINTS:</h3>
This platform can only be used to perform competitions locally on a local network. Currently the communication from the participant and organiser is not setup. This feature can further be improved by adding up new technologies like docker file etc.

<h3>FAQs:</h3>
1.	Can thousands of participants use this ?
Yes, any no. of participants can participate on this platform.

2.	Can we perform coding competitions ?
Yes, you can perform any kind of competition that does not require graphical interface.

3.	Does it work locally only ?
Yes, currently it works locally only.
