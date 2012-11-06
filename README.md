## DESCRIPTION
=================

This is a vagrant box for hadoop 0.23.1

## Installation

### Get the code

```bash
$ git clone git@github.com:demandchain/vagrant-hadoop.git
$ cd vagrant-hadoop
$ git submoudle update --init
```

### Configure share folder

Create a directory on your local machine
```bash
$ mkdir ~/hadoop-share
$ chmod a+w ~/hadoop-share
```
Change the ```config.vm.share_folder``` in Vagrantfile to be the FULL PATH of the folder above (change the third parameter from '/Users/ywen/hadoop-share')
```bash
$ vi Vagrantfile
```

### Run the installation

```bash
$ bundle install
$ vagrant box add base http://files.vagrantup.com/lucid32.box
$ vagrant up
```
