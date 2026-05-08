# Networking Basics

> Understand how computers talk to each other because almost every modern IT support and solution engineering role depends on networks.

If a computer cannot connect to a network, in a startup environment it usually means:

- users cannot log in
- SaaS tools stop working (Slack, Zoom, Notion)
- APIs fail
- cloud services become unreachable
- entire teams become blocked

This is why networking is one of the most important foundations in technical support and solution engineering.

---

# Learning Goals

By the end of this lesson, learners should understand:

- what a network is
- how devices connect
- IP addresses and their meaning
- DNS and why it matters
- routers and switches
- LAN vs WAN
- Wi-Fi vs Ethernet
- basic troubleshooting approach
- common network failures in startups
- how support engineers diagnose network issues

---

# What Is a Network?

A network is a group of connected devices that can communicate with each other.

Examples:
- your laptop connecting to Wi-Fi
- employees accessing company systems
- servers communicating with each other
- mobile apps calling APIs

---

# Real Startup Example

A startup uses:
- Slack (communication)
- Google Drive (files)
- AWS (cloud backend)
- Zendesk (support system)

All of these require networking.

If the network fails:
> the entire startup becomes partially or fully offline

---

# How Network Communication Works

When you open a website or app:

1. Your device sends a request
2. The request travels through a network
3. A server receives the request
4. The server responds
5. Your device displays the result

This happens in milliseconds.

---

# Key Networking Components

---

# 1. IP Address

## What It Is

An IP address is a unique identifier for a device on a network.

Example:
```bash
192.168.1.10
```

---

## Startup Analogy

Think of an IP address like:
> a home address for a computer

Without it:
- data cannot find the device
- communication fails

---

## Types of IP

| Type | Meaning |
|---|---|
| IPv4 | Most common format |
| IPv6 | Newer, larger address system |

---

# 2. DNS (Domain Name System)

## What It Does

DNS translates:
> human-readable names → IP addresses

Example:
```bash
google.com → 142.250.x.x
```

---

## Why DNS Matters

Humans cannot remember IP addresses.

We use:
- google.com
- slack.com
- github.com

DNS makes this possible.

---

## Startup Failure Example

If DNS fails:
- websites stop loading
- APIs fail
- SaaS tools become unreachable

Even if the internet is working.

---

# 3. Router

## What It Does

A router connects your local network to the internet.

It:
- routes traffic
- assigns IP addresses
- manages data flow

---

## Real Startup Example

In an office:
- all laptops connect to a router
- router connects to ISP
- ISP connects to internet

If router fails:
> entire office loses connectivity

---

# 4. Switch

## What It Does

A switch connects devices inside a local network.

Example:
- office computers
- printers
- internal servers

---

# LAN vs WAN

---

# LAN (Local Area Network)

A small network inside a location:
- office
- home
- building

---

# WAN (Wide Area Network)

A large network:
- internet
- cloud systems
- global infrastructure

---

# Startup Example

A startup uses:
- LAN for office devices
- WAN for cloud services

---

# Wi-Fi vs Ethernet

---

# Wi-Fi

- wireless
- flexible
- slower in some cases
- prone to interference

---

# Ethernet

- wired connection
- faster
- more stable
- preferred for servers and production systems

---

# Real Startup Practice

Engineers prefer:
- Ethernet for production systems
- Wi-Fi for general users

---

# Packets

## What Is a Packet?

Data is broken into small pieces called packets.

Each packet contains:
- sender information
- receiver information
- data content
- sequence information

---

# Real Example

Sending a Slack message:
- message is split into packets
- packets travel through network
- packets are reassembled

---

# Latency

## What It Means

Latency is the delay in network communication.

---

## Startup Impact

High latency causes:
- slow APIs
- lag in video calls
- delayed responses
- poor user experience

---

# Bandwidth

## What It Means

Bandwidth is how much data can be transferred at once.

---

## Analogy

- latency = speed
- bandwidth = width of pipe

---

# Common Network Problems in Startups

| Problem | Impact |
|---|---|
| No internet | Complete outage |
| Slow connection | Productivity drop |
| DNS failure | Apps not loading |
| VPN issues | Remote work blocked |
| Packet loss | Broken communication |

---

# How Support Engineers Diagnose Network Issues

---

# Step 1: Check Physical Connection

- Is Wi-Fi on?
- Is cable connected?
- Is router working?

---

# Step 2: Check IP Address

Linux/macOS:
```bash
ip a
```

Windows:
```powershell
ipconfig
```

---

# Step 3: Test Internet Connectivity

```bash
ping google.com
```

If it fails:
- DNS issue
- network issue
- firewall issue

---

# Step 4: Check DNS

```bash
nslookup google.com
```

---

# Step 5: Check Routing

```bash
traceroute google.com
```

Windows:
```powershell
tracert google.com
```

---

# Real Startup Incident Example

## Problem

Employees cannot access SaaS tools.

---

## Investigation

Support engineer checks:

- Wi-Fi status
- router connectivity
- DNS resolution
- ISP status
- VPN configuration

---

## Root Cause

DNS misconfiguration at router level.

---

## Fix

Updated DNS settings:
```bash
8.8.8.8
1.1.1.1
```

---

# Firewalls

## What They Do

Firewalls block or allow network traffic.

---

## Startup Use

Used to:
- protect systems
- restrict access
- secure internal tools

---

# VPN (Virtual Private Network)

## What It Does

VPN creates a secure tunnel between user and company network.

---

## Startup Use Case

Remote employees use VPN to:
- access internal systems
- connect to private servers
- secure communication

---

# Why VPNs Fail

Common issues:
- expired credentials
- blocked ports
- misconfiguration
- unstable connection

---

# Public vs Private IP

| Type | Meaning |
|---|---|
| Public IP | Visible on internet |
| Private IP | Internal network only |

---

# Real Startup Architecture Example

A typical startup system:

```bash
User Laptop → Router → Internet → Cloud Server → Database
```

---

# Why Networking Matters in Solution Engineering

Solution engineers must:
- design system connectivity
- integrate APIs
- ensure uptime
- debug connectivity issues
- support distributed systems

---

# Beginner Mistakes

| Mistake | Better Approach |
|---|---|
| Restarting router blindly | Diagnose step-by-step |
| Ignoring DNS | Always check DNS first |
| Not using ping tools | Always test connectivity |
| Guessing issues | Follow structured troubleshooting |

---

# Real Skills Built Here

This lesson builds:

- diagnostic thinking
- infrastructure awareness
- troubleshooting logic
- production readiness
- startup system understanding

---

# Mini Exercise

## Scenario

A startup employee reports:

> "Slack, Zoom, and Google Drive are not loading."

---

## Your Investigation Steps

1. Check Wi-Fi
2. Check IP address
3. Ping external site
4. Test DNS
5. Check VPN status

---

## Expected Thinking Pattern

Do NOT guess.

Think:
- layer by layer
- systematically
- like a support engineer

---

# Key Takeaways

- Networks connect all modern systems
- DNS is critical for SaaS applications
- IP addresses identify devices
- Routers connect users to the internet
- Support engineers troubleshoot step-by-step
- Most startup outages are network-related

---

# Next Lesson

Continue to:

```bash
internet-protocols.md
```

The next lesson explains:
- how internet communication actually works
- HTTP/HTTPS
- APIs communication basics
- request/response cycles
- real startup backend communication flow
