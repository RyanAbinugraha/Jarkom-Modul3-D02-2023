# Jarkom-Modul3-D02-2023

Nama Anggota | NRP
------------------- | --------------		
Ryan Abinugraha | 5025211178
Abdurrohim Usaamah Khafizduddin | 5025201255

Config

Aura (DHCP Relay)
```
auto eth0
iface eth0 inet dhcp
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.192.0.0/16

auto eth1
iface eth1 inet static
	address 192.192.1.0
	netmask 255.255.255.0

auto eth2
iface eth2 inet static
	address 192.192.2.0
	netmask 255.255.255.0

auto eth3
iface eth3 inet static
	address 192.192.3.0
	netmask 255.255.255.0

auto eth4
iface eth4 inet static
	address 192.192.4.0
	netmask 255.255.255.0
```
Himmel (DHCP Server)
```
auto eth0
iface eth0 inet static
	address 192.192.1.1
	netmask 255.255.255.0
	gateway 192.192.1.0

```
Heiter (DNS Server)
```
auto eth0
iface eth0 inet static
	address 192.192.1.2
	netmask 255.255.255.0
	gateway 192.192.1.0
```
Denken (Database Server)
```
auto eth0
iface eth0 inet static
	address 192.192.2.1
	netmask 255.255.255.0
	gateway 192.192.2.0
```
Eisen (Load Balancer)
```
auto eth0
iface eth0 inet static
	address 192.192.2.2
	netmask 255.255.255.0
	gateway 192.192.2.0
```
Frieren (Laravel Worker)
```
auto eth0
iface eth0 inet static
	address 192.192.4.3
	netmask 255.255.255.0
	gateway 192.192.4.0

hwaddress ether 9e:d5:2c:df:39:32
```
Flamme (Laravel Worker)
```
auto eth0
iface eth0 inet static
	address 192.192.4.2
	netmask 255.255.255.0
	gateway 192.192.4.0

hwaddress ether da:cc:d9:29:59:e8
```
Fern (Laravel Worker)
```
auto eth0
iface eth0 inet static
	address 192.192.4.1
	netmask 255.255.255.0
	gateway 192.192.4.0

hwaddress ether 8a:31:c6:e6:a2:7b
```
Lawine (PHP Worker)
```
auto eth0
iface eth0 inet static
	address 192.192.3.3
	netmask 255.255.255.0
	gateway 192.192.3.0

hwaddress ether 8e:c1:16:c2:6d:4b
```
Linie (PHP Worker)
```
auto eth0
iface eth0 inet static
	address 192.192.3.2
	netmask 255.255.255.0
	gateway 192.192.3.0

hwaddress ether 7a:e7:1c:d2:ae:44
```
Lugner (PHP Worker)
```
auto eth0
iface eth0 inet static
	address 192.192.3.1
	netmask 255.255.255.0
	gateway 192.192.3.0

hwaddress ether 8a:02:fd:bb:05:be
```
Revolte, Richter, Sein, dan Stark (Client)
```
auto eth0
iface eth0 inet dhcp
```
