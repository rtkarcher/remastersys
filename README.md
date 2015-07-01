Remastersys
===========

Remastersys Tool for Backup Your Ubuntu System

* Fork from [http://www.remastersys.com](http://www.remastersys.com/)
* Basically a total clone of [Mutse Young's](https://github.com/mutse/remastersys) repository


## How to install

Add the repository to your software sources:

	$ sudo add-apt-repository ppa:quizas/remastersys

If the above command doesn't work, however, you can manually import the key and add the 

	$ sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys EFDF73BF
	$ sudo add-apt-repository ppa:quizas/remastersys
	$ sudo su

### For Ubuntu 14.04 (Trusty):

	# echo 'deb http://ppa.launchpad.net/quizas/remastersys/ubuntu trusty main' >> /etc/apt/sources.list
	# echo 'deb-src http://ppa.launchpad.net/quizas/remastersys/ubuntu trusty main' >> /etc/apt/sources.list
	
### For Ubuntu 12.04 (Precise):
	
	$ sudo apt-get update
	$ sudo apt-get install remastersys remastersys-gtk

   
The key can be found on the [Launchpad page](https://launchpad.net/~quizas/+archive/ubuntu/remastersys) under the section titled *'Technical details about this PPA'*:

	Signing key:
	4096R/EFDF73BF
	
	Fingerprint:
	E03F7C2D7E25575C3AA24E3EEDF18CFBEFDF73BF


## Application Preview

### Actions
![actions](./images/remastersys-gtk-01.png)
### Settings
![settings](./images/remastersys-gtk-02.png)
### Output
![output](./images/remastersys-gtk-03.png)