# Lab 08 – Access Control List (ACL)

## Objective

The objective of this lab is to understand how a Standard Access Control List (ACL) can be configured on a Cisco router to control network traffic.

## Network Topology

The topology consists of:

- 2 PCs
- 2 Cisco 2960 switches
- 1 Cisco 2911 router

PC0 belongs to the `192.168.10.0/24` network, while PC1 belongs to the `192.168.20.0/24` network.

## IP Addressing

| Device | IP Address | Default Gateway |
|---|---|---|
| PC0 | 192.168.10.10 | 192.168.10.1 |
| Router G0/0 | 192.168.10.1 | N/A |
| Router G0/1 | 192.168.20.1 | N/A |
| PC1 | 192.168.20.10 | 192.168.20.1 |

## ACL Configuration

A Standard ACL was created to deny traffic from PC0 while allowing other traffic.

```text
access-list 10 deny host 192.168.10.10
access-list 10 permit any
