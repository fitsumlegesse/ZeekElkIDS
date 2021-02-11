# Installing Zeek on Ubuntu 20.04 Desktop
###### On this documentation, I will show you how to install zeek, formarly known as bro and configure it to work with ELK stack 
# Dependency
Before downloading and installing zeek, we must download and install all the dependencys 
> sudo su
###### Enter the super user password and press enter 
###### Once you enter the correct super user password check what your IP address is by typing and write it down for later user
>ifconfig
###### The following result will be displayed 
![Image of Yaktocat](https://github.com/fitsumlegesse/ZeekElkIDS/Img/Screenshot from 2021-02-10 22-19-19.png)
###### Update the entire system before starting any instalation 
>apt-get update
###### Once the updating process is complete, upgrade the system
> apt-get upgrade
###### Once the system is done upgrading, we will install all the dependecys by typing the following command
> sudo apt-get install cmake make gcc g++ flex bison libpcap-dev libssl-dev python-dev swig zlib1g-dev -y
###### Once we have all the dependecy installed, we will grab the repository for zeek
> wget -nv https://download.opensuse.org/repositories/security:zeek/xUbuntu_20.04/Release.key -O Release.key
###### Check that the repository is grabbed by typing ls. If it is installed you should see Release.key when you type ls
>ls 
###### Once you see Release.key, enter the following command to add the key
> apt-key add -<Release.key
###### After you add the key, you will get a response "OK". Once you get Okay, update the system again
> apt-get update
###### Once the updating process is complete, download the repository containing zeek 
> sudo sh -c "echo 'deb http://download.opensuse.org/repositories/security:/zeek/xUbuntu_20.04/ /' > /etc/apt/sources.list.d/security:zeek.list"
###### Once the repository is completed, update the system by typing 
> apt-get update 
###### Once the updating is completed, install zeek by typing the following command 
> apt-get install zeek-lts 
###### Once the installations is complete, check if Zeek is installed on the system by typing the following command
> ls
###### If you followed the instruction properly, you should have a  directory named zeek 






