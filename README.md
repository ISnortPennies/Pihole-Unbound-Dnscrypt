This is my personal pihole setup I run it on a raspberry pi 4b with openwrt as the OS
Installation on OpenWRT:

get prerequisites
opkg update
opkg install kmod-macvlan docker docker-compose dockerd luci-app-dockerman

download files
wget https://github.com/ISnortPennies/Pihole-Unbound-Dnscrypt.git

change folder name
mv Pihole-Unbound-Dnscrypt dns

then start the containers
cd dns
docker-compose up
