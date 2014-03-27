LaTeX text for my master thesis report
===============================================================

### About this report
This git repository includes my report(s) from my master thesis work
done during the spring of 2014 about the "Virtual Network Protocol".

### Keywords
Space plug-and-play Avionics, Space plug-and-play Architecture, Ada,
Safety-critical systems, Internet of Things, Unmanned Vehicles

### How to generate PDF using virtualbox and Vagrant
For this project Virtualbox and Vagrant is used for easier management of LaTeX
code compilation. Virtualbox is used to run a virtual machine (VM) and Vagrant
is the tool used to manage the virtual machines configuration.

##### Ubuntu 12.04
To install latest Virtualbox and Vagrant on Ubuntu 12.04 do the following:

**Add virtualbox repository and install Virtualbox 4.3 with apt-get**
```
$ sudo sh -c 'echo "deb http://download.virtualbox.org/virtualbox/debian precise contrib" >> /etc/apt/sources.list'
$ wget -q http://download.virtualbox.org/virtualbox/debian/oracle_vbox.asc -O- | sudo apt-key add -
$ sudo apt-get update
$ sudo apt-get install virtualbox-4.3
```

**Download and install Vagrant**
```
http://www.vagrantup.com/downloads.html
$ sudo dpkg -i <downloaded_deb_file>
```

##### Start the VM and generate PDF from the LaTeX code
```
$ git clone https://github.com/christofferholmstedt/dva501-master-thesis-report 
$ cd dva501-master-thesis-report
$ vagrant up (wait for the VM to install and boot up)
$ vagrant ssh
$ cd host/report
$ make
```

The report is generated and available as "main.pdf" both on your host machine
and in your VM.
