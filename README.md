## DESCRIPTION
=================

This is a vagrant box for hadoop 0.23.1

## Installation

### Configure share folder

Create a directory on your local machine
```bash
$ mkdir hadoop-share
```
Change the '''config.vm.share_folder''' to be the full path of the folder above (change the third parameter from '/Users/ywen/hadoop-share')

### Run the installation script

```bash
$ git clone git@github.com:demandchain/vagrant-hadoop.git
$ cd vagrant-hadoop
$ git submoudle init
$ git submodule update
$ cd vagrant-hadoop
$ bundle install
$ vagrant box add base http://files.vagrantup.com/lucid32.box
$ vagrant up
```
