# Installing Zeek on Ubuntu 20.04
###### On this documentation, I will show you how to install zeek, formarly known as bro and configure it to work with ELK stack 
# Dependency
Before downloading and installing zeek, we must download and install all the dependencys 
> sudo su
###### Enter the super user password and press enter 
###### Once you enter the correct super user password check what your IP address is by typing and write it down for later user
>ifconfig
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






