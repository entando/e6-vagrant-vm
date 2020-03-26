# How to

## Prerequisites

- VirtualBox > 6 https://www.virtualbox.org/wiki/Downloads
- Any of Linux, Windows > 8.1 (Professional), Mac OSX
- Vagrant https://www.vagrantup.com/downloads.html

## Create the Box

In the root of this project run `vagrant up` and wait until the process ends. The first time it will take longer so you can take a coffee and relax. 

**During the startup phase vagrant will ask you to choose the network interface to use for the bridging.** This way all the network configuration will be done automatically and you'll access to openshift web console from your pc.

## Login to the VM

Execute `vagrant ssh` and you'll be connected in ssh to the newly created VM.

## Start Openshift installation

Execute `./start-oc.sh` and yes... if you want you can take another coffee. This script will also :
- assigns the cluster-role rights to the **developer** user 
- install the Entando CRD
- create a project called **my-app**

