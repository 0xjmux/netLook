!/bin/bash
if [ ! -d "/sys/class/net/$1" ]; then echo Interface does not exist. Please enter a valid interface. && exit; fi
echo -e "\e[5;32mPinging addresses, please wait \e[0m"
arp-scan -I $1 -l | awk '{print $1}' | sed -e '1,2d' | sed -e '$ d' | sed -e '$ d' | sed -e '$ d' | while read -r line; do ping $line -c 2; done >/dev/null
arp -a 

