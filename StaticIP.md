## Static IP Address in Ubuntu

/etc/network/interfaces

auto eth0

iface eth0 inet static

address 10.0.0.100

netmask 255.255.255.0

gateway 10.0.0.1
