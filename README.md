Remastersys
===========

(This repository is basically a complete clone of [Mutse Young's forked Remastersys PPA/repo](https://github.com/mutse/remastersys), and is being maintained exclusively for the sake of redundancy.)

[Remastersys](http://ubuntuguide.org/wiki/Remastersys) is a free and open source program for [Debian](https://www.debian.org/)-based or -derivative Linux distributions (including [Ubuntu](http://www.ubuntu.com/) and [Linux Mint](http://linuxmint.com/)) that can create custom Live CD/USB images of the following:

* Your operating system files/specific configurations; a total remaster that can be used in creating a custom Live CD/USB of your system setup.
* Your entire operating system and all user data, including all files; a comprehensive backup of your entire system (which can also be burned to a Live CD/USB of sufficient size).


## Why can't I access the project website?

* April 2013 - Supporters announce end of further development for the Remastersys project; development forked to new supporters in advent of a new project, the [Black Lab Image Creator](http://system-imaging.blogspot.com/).
* June 2015 - Original [Remastersys domain](http://www.remastersys.com/) has expired; now owned by Chinese online retailer, "Rema-Stersys."
 
## How to Install

### 1. Add the Repository to Your Sources

 Add the [repository](https://launchpad.net/~quizas/+archive/ubuntu/remastersys) to your software sources list:

	$ sudo add-apt-repository ppa:quizas/remastersys

If the above command doesn't work, however, you can manually import the key and add the repository with this:

	$ sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys EFDF73BF
	
The key can be found on the [repository's Launchpad page](https://launchpad.net/~quizas/+archive/ubuntu/remastersys) under the section titled *'Technical details about this PPA'*:

	Signing key:
	4096R/EFDF73BF
	
	Fingerprint:
	E03F7C2D7E25575C3AA24E3EEDF18CFBEFDF73BF
	

#### For Ubuntu 14.04 (Trusty):

To manually add the repository to your /etc/apt/sources.list:

	$ sudo su
	# echo 'deb http://ppa.launchpad.net/quizas/remastersys/ubuntu trusty main' >> /etc/apt/sources.list
	# echo 'deb-src http://ppa.launchpad.net/quizas/remastersys/ubuntu trusty main' >> /etc/apt/sources.list
	
#### For Ubuntu 12.04 (Precise):

To manually add the repository to your /etc/apt/sources.list:

	$ sudo su
	# echo 'deb http://ppa.launchpad.net/quizas/remastersys/ubuntu trusty main' >> /etc/apt/sources.list
	# echo 'deb-src http://ppa.launchpad.net/quizas/remastersys/ubuntu trusty main' >> /etc/apt/sources.list

### 2. Update apt-get & Install

Once the repository has been added, update apt-get and install:
	
	$ sudo apt-get update
	$ sudo apt-get install remastersys remastersys-gtk


## How to Use

* Using Remastersys via command line is mercifully easy, but the GUI can also be found here:
	* Menu -> System Adminstration -> **Remastersys Backup**
* Command line instructions:
	* [How to create a custom distribution .ISO from your operating system setup](http://ubuntuguide.org/wiki/Remastersys#Create_a_custom_distribution)
	* [How to create a full system backup .ISO](http://ubuntuguide.org/wiki/Remastersys#Create_a_system_backup)


## Application Preview

### Actions
![actions](./images/remastersys-gtk-01.png)
### Settings
![settings](./images/remastersys-gtk-02.png)
### Output
![output](./images/remastersys-gtk-03.png)