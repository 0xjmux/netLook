# netLook
A bash script to find device names on a network. 

It uses arp-scan to locate all devices on the network, even hidden ones, and then pings them for a response. That ping then adds the device to the computer's arp table, which is promptly listed out in the terminal. 

USEAGE:
In order to get it to work, clone it and add the netLook file to your /usr/local/bin directory. THen use chmod to make it executable (chmod +x netLook). Now it is accessible from any directory. 

netLook [WIRELESS INTERFACE]

This will return a list of all devices on the local network, along with their hostnames, IPs and Mac addresses. 

This is one of my first bash scripts, so it isn't all that optimized. If you know a way to optimize it, feel free to commit. 
