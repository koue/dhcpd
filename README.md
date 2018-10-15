# FreeBSD port of OpenBSD dhcpd

dhcpd implements the Dynamic Host Configuration Protocol (DHCP) and the
Internet Bootstrap Protocol (BOOTP). DHCP allows hosts on a TCP/IP network
to request and be assigned IP addresses, and also to discover information
about the network to which they are attached. BOOTP provides similar
functionality, with certain restrictions.

The DHCP protocol allows a host which is unknown to the network administrator
to be automatically assigned a new IP address out of a pool of IP addresses
for its network. In order for this to work, the network administrator allocates
address pools in each subnet and enters them into the dhcpd.conf(5) file.

http://cvsweb.openbsd.org/cgi-bin/cvsweb/src/usr.sbin/dhcpd/

## Installation

### Requirements
* libressl/openssl

`cd src/usr.sbin/dhcpd/ && make && make install`

## Usage

`dhcpd -c etc/examples/dhcpd.conf`

## Status

master | develop
-------|--------
[![Build Status](https://cipier.net/status/koue/dhcpd/master)](https://cipier.net/status/koue/dhcpd/master) | [![Build Status](https://cipier.net/status/koue/dhcpd/develop)](https://cipier.net/status/koue/dhcpd/develop)
