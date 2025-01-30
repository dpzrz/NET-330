### Readings

**Chapter 10:**

- 10.20 DHCP

### LAB 2-1: Subnet Design

Assigning ports to certian Vlans is tedious manually. Using cisco command

```
(config)interface range FastEthernet 0/x-y (let's you configure multiple ports at one time)
(config-if-range)switchport access vlan x (defines the vlan for all ports in the range)
```




```
(config)ip routing (turns on routing on multilayer switches)
(config)interface vlan 100 (brings you into vlan interface config mode)
(config-if)ip address 10.25.100.1 255.255.255.0 (set the ip address of 10.25.100.1 for vlan 100 on a routing switch)
NOTE: This only needs to be set on the router-switch acting as the gateway for the vlan
```
