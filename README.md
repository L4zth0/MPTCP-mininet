# MPTCP-mininet
MPTCP simulation using Mininet in basic network topology

check if MP-TCP is enabled in the host computer
      sysctl -a | grep mptcp.enabled

Containernet is a fork of Mininet that allows to use Docker containers as Mininet hosts as well as Mininet-WiFi stations. 
This enables interesting functionalities to built networking/cloud testbeds. The integration is done by subclassing the original Host/Station classes.

Run containernet 
      sudo docker run -v /Home/Documents/configuration:/mnt --name containernet -it --rm --privileged --pid='host' -v /var/run/docker.sock:/var/run/docker.sock containernet/containernet /bin/bash

Copy the network configuration on the currently running 

      sudo docker cp /home/jorge/Documents/configuration/prueba.py containernet:/mnt/prueba.py
