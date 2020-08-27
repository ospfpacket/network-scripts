BGP Failover Lab
=======

Move your organizations internet bound traffic from one BGP circuit to another

## Quick Links

- [Platforms Used in the Lab](https://github.com/ospfpacket/python_ospf_lab#platforms-used-in-the-lab)
- [Assumptions](https://github.com/ospfpacket/python_ospf_lab#assumptions)
- [Installation](https://github.com/ospfpacket/python_ospf_lab#installation)
- [Common Issues](https://github.com/ospfpacket/python_ospf_lab#installation)

## Platforms Used in the Lab

This lab was run against the following IOL image:
- L3-ADVENTERPRISEK9-M-15.4-2T.bin

## Steps to move traffic

1. Run the preferred path script on the internet router that you want your traffic to ingress and egress through.
2. Run the unpreferred path script on the internet router that you want to avoid sending traffic through.

## BGP Assumptions

In a real-world scenario, it is assumed that you have peering configured with your provider and that they will accept attribute changes that you make to the path. In some instances, you will not be able to do this due to provider limitations as they will not honor any changes that you make to the BGP attributes in the updates that you send to them.