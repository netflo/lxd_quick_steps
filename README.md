# LXD containers


sudo apt install lxd lxd-client

#storage+net + ... init
sudo lxd init

lxc launch ubuntu:18.04 container1

#execute the shell command to go and stay in it:
lxc exec container1 -- /bin/bash


#To pull a file from the container, use:

lxc file pull container1/etc/hosts .

#To push one, use:

lxc file push hosts container1/tmp/

#To stop the container, simply do:

lxc stop container1

#And to remove it entirely:

lxc delete container1


