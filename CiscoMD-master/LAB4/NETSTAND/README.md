- [1](#1)
- [2](#2)
- [3](#3)

# 1

- `no`
- `<enter>`
- `conf t`
- `ip access-list extended 100`
- `deny icmp any any`
- `permit tcp any any eq ftp`
- `exit`
- `int vlan 1`
- `ip address 192.168.1.1 255.255.255.0`

# 2

- `no`
- `<enter>`
- `conf t`
- `ip access-list extended 100`
- `permit tcp host 192.168.1.1 host 192.168.1.3 eq telnet`
- `permit tcp host 192.168.1.1 host 192.168.1.3 eq 22` // aka ssh
- `exit`
- `int vlan 1`
- `ip address 192.168.1.2 255.255.255.0`
- `ip access-group 100 in`

# 3

- `no`
- `<enter>`
- `conf t`
- `int vlan 1`
- `ip address 192.168.1.3 255.255.255.0`
