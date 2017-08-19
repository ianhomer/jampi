---
layout: tool
title: Raspberry Pi Getting Started
---

# Network and Users

Change password for *pi* user from the default password *raspberry*

    passwd

Documentation is based on the following :

The Raspberry Pi IP address has been configured in the local /etc/hosts 
file, e.g

    192.168.1.126   my.pi

A user called *pi* has been configured.

Locally SSH keys have been set up for the *pi* user such you can log in to
*my.pi* with

    ssh pip@my.pi
    
# Update system
    
As per https://learn.pimoroni.com/tutorial/raspberry-pi/keeping-your-raspberry-pi-updated
    
    sudo apt-get update
    sudo apt-get upgrade
    sudo reboot
    
# Install Unicorn HAT

See https://github.com/pimoroni/unicorn-hat and
https://learn.pimoroni.com/tutorial/unicorn-hat/getting-started-with-unicorn-hat

Installation boils down to running :

    curl -sS https://get.pimoroni.com/unicornhat | bash

Or manually with

    git clone https://github.com/pimoroni/unicorn-hat.git
    cd unicorn-hat/library/UnicornHat
    cd ../../examples/

Then you can run examples with :
    
    cd ~/Pimoroni/unicornhat/examples/
    sudo python ./simple.py
    
