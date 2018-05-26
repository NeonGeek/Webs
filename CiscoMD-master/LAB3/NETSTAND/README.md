- [1](#1)
- [3](#3)

# 1

- `no`
- `<enter>`
- `conf t`
- `int vlan1`
- `ip address 190.168.1.1 255.255.255.0`
- `exit`
- `ip route 193.168.1.0 255.255.255.0 190.168.1.3`

# 3

- `no`
- `<enter>`
- `conf t`
- `int vlan1`
- `ip address 190.168.1.3 255.255.255.0`
- `exit`
- `int fa1/3`
- `no switchport`
- `ip address 193.168.1.1 255.255.255.0`
