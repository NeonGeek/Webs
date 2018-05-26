- [1](#1)
- [2](#2)
- [3](#3)

# 1

- `no`
- `<enter>`
- `enable`
- `vlan database`
- `vlan 111`
- `exit`
- `configure terminal`
- `int vlan 111`
- `ip address 192.168.1.1 255.255.255.0`
- `exit`
- `int fa1/2`
- `switchport mode access`
- `switchport access vlan 111`
- `exit`

## Secure

- `enable secret qwerty`
- `username root privilege 15 password qwerty`
- `line vty 0 4`
- `transport input ssh`
- `logging synchronous`
- `exec-timeout 60 0`
- `login`
- `transport input telnet`
- `logging synchronous`
- `exec-timeout 60 0`
- `login`
- `exit`

# 2

- `no`
- `<enter>`
- `enable`
- `vlan database`
- `vlan 111`
- `exit`
- `configure terminal`
- `int vlan 111`
- `ip address 192.168.1.2 255.255.255.0`
- `exit`
- `int fa1/2`
- `switchport mode access`
- `switchport access vlan 111`
- `exit`
- `int fa1/1`
- `switchport mode trunk`
- `switchport trunk allowed vlan add 111`
- `exit`

# 3

- `no`
- `<enter>`
- `enable`
- `vlan database`
- `vlan 111`
- `exit`
- `configure terminal`
- `int vlan 111`
- `ip address 192.168.1.3 255.255.255.0`
- `exit`
- `int fa1/1`
- `switchport mode trunk`
- `switchport trunk allowed vlan add 111`
- `exit`
