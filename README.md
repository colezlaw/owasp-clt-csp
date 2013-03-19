Aboalarm devbox
======

Vagrant Development Box for running Aboalarm


## Requirements

* [VirtualBox](https://www.virtualbox.org/wiki/Downloads) - Free virtualization software 
* [Vagrant](https://www.vagrantup.com) - Tool for working with VirtualBox images


## Setup

* Clone this repository `git clone https://github.com/Aboalarm/devbox.git`
* run `vagrant up` inside the newly created directory
* (the first time you run vagrant it will need to fetch the virtual box image which is ~300mb so depending on your download speed this could take some time)
* Vagrant will now use Puppet to provision the box with the Aboalarm software stack (this could take a few minutes)
* Point aboalarm.dev to XXX (t.b.d.) in your hosts file of your os. 
* Done! You can verify that everything was successful by opening http://aboalarm.dev/stacktest in a browser



### Using Vagrant

Vagrant is [very well documented](http://vagrantup.com/v1/docs/index.html) but here are a few common commands:

* `vagrant up` starts the virtual machine and provisions it
* `vagrant suspend` will essentially put the machine to 'sleep' with `vagrant resume` waking it back up
* `vagrant halt` attempts a graceful shutdown of the machine and will need to be brought back with `vagrant up`
* `vagrant ssh` gives you shell access to the virtual machine


##### Virtual Machine Specifications #####

* OS          - Ubuntu 12.04
* Nginx       - xxx
* PHP         - 5.4.13
* MySQL       - 5.5.28
* Redis       - xxx
* Beanstalkd  - xxx
* supervisord - xxx
* Sphinx      - xxx
* localtunnel - xxx
* Node.js     - xxx
* MongoDB     - xxx