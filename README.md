# LSA

practial 1


Step 1: Installing DHCP Server in Ubuntu
        $ sudo apt install isc-dhcp-server
        
Step 2: Configuring DHCP Server in Ubuntu
        $ sudo vi /etc/dhcp/dhcpd.conf 
        
Step 3: Configure Static IP on DHCP Client Machine
        host centos-node {
	 hardware ethernet 00:f0:m4:6y:89:0g;
	 fixed-address 192.168.10.105;
 }

host fedora-node {
	 hardware ethernet 00:4g:8h:13:8h:3a;
	 fixed-address 192.168.10.106;
 }
 
 Step 4: Configuring DHCP Client Machines
         $ sudo vi /etc/network/interfaces
