# Cyber-Scan

CyberScan is an open source penetration testing tool   

that can analyse packets , decoding , scanning ports,   

pinging and geolocation of an IP including  

(latitude, longitude , region , country ...)  

Installation :  
$ apt update &amp;&amp; apt upgrade  
$ apt install git   
$ apt install python2  
$ apt install python  
$ git clone https://github.com/medbenali/CyberScan.git  
$ cd CyberScan  

usage :  
$ python2 CyberScan.py -v  
$ CyberScan -h  

We can perform ping operations with several protocols using CyberScan  

The fastest way to discover hosts on a local Ethernet network  

is to use ARP:  
$ python2 CyberScan -s 192.168.1.0/24 -p arp  

In case when ICMP echo requests are blocked, we can still use TCP:  
$ CyberScan -s 192.168.1.105 -p tcp -d 80  
192.168.1.105 = target IP.
