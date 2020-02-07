## Quick Start

### 1- Install Linux
#### Ubuntu 16.04

Start with a clean and minimal install of a Linux system. DevStack attempts to support the two latest LTS releases of [Ubuntu](http://releases.ubuntu.com/16.04/), the latest/current Fedora version, 
CentOS/RHEL 7, as well as Debian and OpenSUSE.

### 2- Install OpenStack with Tacker Service (NFV)
#### Version: Ocata

[DevStack](https://github.com/openstack/devstack) is a series of extensible scripts used to quickly bring up a complete OpenStack environment based on the latest versions of everything from git master. It is used interactively as a development environment and as the basis for much of 
the OpenStack project’s functional testing.

Installation and Configuration step by step: [DevStack-Ocata](https://github.com/edigleisonb/Edge-On/blob/master/OpenStack/OpenStack%20installation%20tutorial%20via%20DevStack).


### 3- Install Mininet-WiFi
#### Version: 2.2.2d1
#### Open vSwitch 2.5.5
[Mininet-WiFi](https://github.com/intrig-unicamp/mininet-wifi) is an open source platform to emulate wireless OpenFlow/SDN scenarios allowing high-fidelity experiments that replicate real networking environments. Mininet-WiFi augments the well-known Mininet emulat
or with virtual wireless stations and access points while keeping the original SDN capabilities and the lightweight virtualization software architecture.

We use the example of [sumo-experimental.py](https://github.com/edigleisonb/Edge-On/blob/master/Mininet%20Wi-Fi/sumo-experimental.py), redirecting the connection to an external controller.


### 4- Install Ryu
#### Version: 4.21
#### Open Flow 1.3
[Ryu](https://osrg.github.io/ryu/) is a component-based software defined networking framework. Ryu provides software components with well defined API that make it easy for developers to create new network management and control applications. 
Ryu supports various protocols for managing network devices, such as OpenFlow, Netconf, OF-config, etc. About OpenFlow, Ryu supports fully 1.0, 1.2, 1.3, 1.4, 1.5 and Nicira Extensions. All of the code is freely available under the Apache 2.0 license.

Ryu was the controller used to receive vehicle connections.


### 5- Install Docker Engine - Community
#### Version: 18.06.1-ce

Get Docker Engine - Community for Ubuntu [Docker-ce/Ubuntu](https://docs.docker.com/install/linux/docker-ce/ubuntu/#install-docker-engine---community-1)

### 6- Install Traefik 
#### Version: latest
Traefik is an [open-source](https://github.com/containous/traefik) Edge Router that makes publishing your services a fun and easy experience. It receives requests on behalf of your system
and finds out which components are responsible for handling them.

We used an official image from Traefik ([Docker Hub](https://hub.docker.com/_/traefik)).

Installation and Configuration step by step: [Traefik](https://github.com/edigleisonb/Edge-On/tree/master/Traefik)

### 7- Install BTSync
#### Version: Stable

[BTSync](https://www.resilio.com/) Connecting Massive Data Flows, Scalable and Customized Data Transfer & Synchronization Solutions.

To create our P2P application, we use a minimal Docker image based on [Alpine](https://hub.docker.com/_/alpine) Linux with a complete package index and only 5 MB in size!

Installation and Configuration step by step: [BTSync](https://github.com/edigleisonb/Edge-On/tree/master/Application%20Edge%20-P2P)
