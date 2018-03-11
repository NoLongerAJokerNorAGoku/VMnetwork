#The differences among the following VM networks 
+ ###NAT
#####NAT is the acronym of Network Address Translation, which means VMs use the network of its physical host to realize communication. This is the simplest pattern for VMs to get linked in a network because all the TCP/IP settings are generated and provided by a DHCP server and cannot be modified manually.
	- VMs can visit its physical host, however the host cannot visit its VMS.
	- VMs can visit other hosts in the same subnet, however other hosts cannot.
	- VMs cannot communicate with each others.
+ ###Bridge
#####In this mode, the VM equals to an independent host in a LAN and has the equal right to visit any other host in this network. It is thus necessary to set IP address, subnet mask manually for the users. 
	- Since here a VM has the equal position to other hosts, we regard the VM as a depedent host and all the communications in a same subnet are allowed.
+ ###internal
#####The internal pattern is the most special one because it only realize the communication among VMs in the same virtual subnet. In other words, VMs cannot link with its only physical host, nor with other hosts in the same real ubnet.
	- Only the VMs in a same subnet can communicate with each other.
+ ###host-only
#####Host-only pattern is the best choice for those who want to seperate virtual machines form physical ones for different purposes. Generally speaking, the virtual network cannot be combined with the real network in host-only mode while all the VMs can communicate with each other. However, the VM can communicate with its own physical host.
	- VMs cannot communicate with physical hosts because they are supposed not to be in a same subnet.
	- VMs can communicate with each as they are in the same subnet.
