# ufw_configuration.sh

Objective :-  Set up a basic firewall using UFW (Uncomplicated Firewall) on a Linux system.

STEP-1
       First for configuring UFW we have to install it on our linux system.
       For installing UFW we have to run a command as sudo apt install UFW.


STEP-2
       We will check the status of UFW by running a command sudo ufw status.
       If the status is inactive then we will activate it by running a command sudo ufw enable.
       After activating the status we will check the status information by running a command as sudo ufw status verbose.
       Then we will allow both SSH and HTTP traffic by running  command as sudo ufw allow ssh and sudo ufw allow 80.


STEP-3
       We will update the default policies of incoming and outgoing traffic.
       We will 'deny' incoming traffic by running command as sudo ufw default deny incoming.
       We will 'allow' outgoing traffic by running command as sudo ufw default allow outgoing.


STEP-4
       We will allow SSH traffic.
       For allowing SSH traffic we will run command as sudo ufw allow ssh.
       As i already allowed ssh traffic in step 2 it will show me the output as skipping adding existing rule(v6).


STEP-5 
       We will deny HTTP traffic.
       For denying HTTP traffic we will run command as sudo ufw deny http.
       As earlier in step 2 i allowed http traffic now i am denying http traffic it will show me the output as rule updated(v6).


STEP-6
       We will again activate the uncomplicated firewall(UFW) to be on the safer side.


STEP-7
       Now the last and final step we will check the ufw status.
       For checking the ufw status we will run command as sudo ufw status verbose.
       It will show us what we have allowed from where and what we have denied for where. 
