BGP Prefix-List Lab
=======

Use this method to keep your site from becomming a transit in a case where there might be a shortest AS-Path through your network.

Typically, a provider will put this safe guard in place for you, but in order to be doubly sure that some loose canon engineer doesn't want to blow up your system, you can use this method to ensure that you are only advertising networks that belong to you.

## Quick Links

- [Platforms Used in the Lab](https://github.com/ospfpacket/python_ospf_lab#platforms-used-in-the-lab)
- [Assumptions](https://github.com/ospfpacket/python_ospf_lab#assumptions)
- [Installation](https://github.com/ospfpacket/python_ospf_lab#installation)
- [Common Issues](https://github.com/ospfpacket/python_ospf_lab#installation)

## Platforms Used in the Lab

This lab was run against the following IOL images:
- L3-ADVENTERPRISEK9-M-15.4-2T.bin

## Assumptions

- In a real world scenario, if not done with care, prefix-lists can permit or deny more or less than anticipated. The assumption is that you only want to advertise networks that belong to you and you want to let the provider advertise other networks, not you. 
