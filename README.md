# Cybrarians November Challenge — Office Network

## Project Overview
A small office network designed and configured using Cisco Packet Tracer.

The network separates Staff and Guest devices using VLANs, provides automatic IP addressing through DHCP, and uses an ACL to restrict Guest access to Staff devices.

## Network Devices
- 1 Cisco 2911 Router
- 2 Cisco 2960 Switches
- 6 Staff PCs
- 6 Guest PCs
- 1 Staff Server

## IP Addressing

| Network | VLAN | Subnet | Default Gateway |
|---|---|---|---|
| Staff | 10 | 192.168.10.0/24 | 192.168.10.1 |
| Guests | 20 | 192.168.20.0/24 | 192.168.20.1 |
| Staff Server | 10 | 192.168.10.100 | 192.168.10.1 |

## Features Implemented
- VLAN segmentation
- Trunk configuration between switches and router
- Router-on-a-stick inter-VLAN routing
- DHCP configuration
- Static IP configuration for the server
- Extended ACL for Guest network restrictions
- Port security using sticky MAC addresses
- Switch console and remote-line password configuration

## Connectivity Tests

| Test | Result |
|---|---|
| Staff PC to Staff Server | Successful |
| Guest PC to Staff Server | Blocked |
| Staff PC to Guest PC | Successful |
| Guest PC to Guest Gateway | Successful |
| DHCP address assignment | Successful |

## Evidence
Screenshots included in this repository:
- `staff-server-success.jpg`
- `guest-server-blocked.jpg`
- `staff-dhcp.jpg`
- `guest-dhcp.jpg`

## Project File
`Cybrarians_Nov_Challenge.pkt`

## Tool Used
Cisco Packet Tracer

## Disclaimer
This is a simulated networking and cybersecurity learning project developed for the Cybrarians November Challenge.
