# Guide to installing your virtual machine

## -1 prerequisite installation
1) Ensure you have Virtualbox version 6.0.1 installed on your system
2) Ensure you have Vagrant version 2.2.5
3) Ensure you have Virtualbox extension pack version 6.0.1 installed
4) Ensure hyper V is deactivated on your system: Control panel> programs> Programs and Features> Turn Windows features off or on and deselect HyperV if it is selected.
5) Restart computer if HyperV was deselected.
6) Ensure no virtual machine is running on the machine.

## -2 Create Directory 
1) create a directory in git Bash using: mkdir <directoryname> 
2)Place all included files in this directory 
3) Go into this folder using: cd <directoryname>
This is where your virtual machine will be located. Save all files to here.


## -3 Initiate Machine
1) In  Bash run: vagrant up
NOTE:Look for feedback and ensure there are no errors.

## -4 Connect to Virtual Machine
1) run: vagrant ssh
This will connect to the instance of the machine
Feedback should be welcome to ubuntu
NOTE: Bash input line should start with tilde ~$


## -5 Run nginx 
1)to start nginx you should type : sudo systemctl start nginx
NOTE:should come up with a new line in bash command.

## -6 Test= if nginx is working 
1) run: curl http://localhost
NOTE: Should return with the nginx home page 
