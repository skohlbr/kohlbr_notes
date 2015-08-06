= Install =

sudo bmaptool copy --bmap 2015-04-06-ubuntu-trusty.bmap 2015-04-06-ubuntu-trusty.img /dev/mmcblk0

sync

= On Pi =

passwd

sudo apt-get install linux-firmware htop openssh-server iftop wireless-tools screen chrony git

As described in https://wiki.ubuntu.com/ARM/RaspberryPi

sudo fdisk /dev/mmcblk0

(d, 2)
(n, p, 2, enter, enter)
reboot

sudo resize2fs /dev/mmcblk0p2

sudo apt-get install dphys-swapfile


= Install ROS =

Fix locale issue:
sudo locale-gen en_US en_US.UTF-8 hu_HU hu_HU.UTF-8 de_DE.UTF-8
sudo dpkg-reconfigure locales


sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list'

wget https://raw.githubusercontent.com/ros/rosdistro/master/ros.key -O - | sudo apt-key add -

sudo apt-get update

sudo apt-get install ros-indigo-ros-base

sudo apt-get install python-rosdep
sudo rosdep init
rosdep update

= Setup dev environment =

git config --global credential.helper 'cache --timeout=3600'