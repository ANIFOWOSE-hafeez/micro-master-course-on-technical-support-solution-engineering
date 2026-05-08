# Internet Protocols

> Understand how data actually moves across the internet — because every modern support system, SaaS platform, API, and cloud tool depends on it.

If file systems explain how data is stored locally,  
internet protocols explain how data moves globally.

For a support engineer or solution engineer, this is critical because most real incidents involve:
- “no internet”
- “API not responding”
- “login not working”
- “SaaS service down”
- “slow application”
- “VPN issues”
- “DNS failures”

All of these are internet protocol problems at different layers.

---

# Learning Goals

By the end of this lesson, learners should understand:

- what the internet actually is (technically)
- how devices communicate over networks
- what IP addresses are
- what DNS does
- what HTTP/HTTPS means
- how browsers communicate with servers
- what APIs are at network level
- how data travels in packets
- basic troubleshooting of internet issues

---

# What Is the Internet?

The internet is a global system of connected computers that:
- send data
- receive data
- store data
- route data

It is not “magic Wi-Fi”.

It is a structured communication system built on rules called **protocols**.

---

# Real Startup Example

A user opens a startup SaaS app like:

- Slack
- Zendesk
- Notion
- internal dashboards
- APIs

What happens?

Their computer:
1. connects to a network
2. finds the server address
3. sends a request
4. receives a response
5. displays data

All of this happens in milliseconds using protocols.

---

# What Is a Protocol?

A protocol is a set of rules that defines:
- how devices communicate
- how data is formatted
- how errors are handled
- how connections are established

Think of it like:
> a shared language between computers

---

# IP Address (Internet Protocol Address)

An IP address is a unique identifier for a device on a network.

Example:
```bash
192.168.1.10
```

---

# Why IP Addresses Matter

Without IP addresses:
- computers cannot find each other
- websites cannot be reached
- APIs cannot be called
- cloud systems cannot function

---

# Real Startup Example

When a support engineer says:

> “The server is down”

They often start by checking:
- IP address availability
- network connectivity
- routing issues

---

# Types of IP Addresses

| Type | Meaning |
|---|---|
| Public IP | Visible on the internet |
| Private IP | Internal network only |

---

# Example

Public IP:
```bash
104.21.34.12
```

Private IP:
```bash
192.168.0.15
```

---

# DNS (Domain Name System)

DNS is like the internet phonebook.

It converts:
```bash
google.com
```

into:
```bash
142.250.190.14
```

---

# Why DNS Exists

Humans remember names:
- google.com
- github.com

Computers need numbers:
- IP addresses

DNS bridges that gap.

---

# Real Startup Incident

User says:

> “The website is not loading”

Possible DNS issue:
- domain not resolving
- wrong DNS server
- expired DNS record

---

# DNS Troubleshooting Commands

Windows:
```powershell
nslookup google.com
```

Linux/macOS:
```bash
dig google.com
```

or
```bash
nslookup google.com
```

---

# HTTP and HTTPS

These are the most important web protocols.

---

# HTTP

HyperText Transfer Protocol

Used for:
- web communication
- API requests
- data transfer

But:
- not secure

---

# HTTPS

Secure version of HTTP

Adds:
- encryption
- security
- authentication

Used in:
- all modern SaaS systems
- login pages
- payment systems

---

# Real Startup Example

When a user logs into a SaaS app:

1. browser sends HTTPS request
2. server validates credentials
3. response is encrypted
4. session is created

---

# HTTP Request Structure

A request contains:
- method
- headers
- body
- endpoint

Example:
```http
GET /api/users
```

---

# HTTP Methods

| Method | Meaning |
|---|---|
| GET | Retrieve data |
| POST | Create data |
| PUT | Update data |
| DELETE | Remove data |

---

# Real Startup API Example

Ticket system:

```http
POST /api/tickets
```

```json
{
  "subject": "VPN not working",
  "priority": "auto"
}
```

This is exactly what support systems use internally.

---

# Ports

A port is a communication endpoint.

Think of it like:
> a door into a computer

---

# Common Ports

| Service | Port |
|---|---|
| HTTP | 80 |
| HTTPS | 443 |
| SSH | 22 |
| DNS | 53 |

---

# Real Startup Example

A server might:
- run API on port 443
- run database on port 5432
- run SSH on port 22

---

# Packets

Data is not sent all at once.

It is broken into small units called:
> packets

---

# Packet Flow

1. data is split
2. packets are sent
3. packets travel different routes
4. packets are reassembled

---

# Why Packets Matter

Support engineers troubleshoot:
- packet loss
- latency
- network congestion

---

# Latency

Latency = delay in communication.

---

# Real Startup Example

A user says:

> “The app is slow”

Possible cause:
- high latency
- poor routing
- overloaded server
- VPN delay

---

# Bandwidth

Bandwidth = how much data can be sent at once.

---

# Example

| Low bandwidth | High bandwidth |
|---|---|
| slow downloads | fast downloads |
| buffering video | smooth streaming |

---

# VPN (Virtual Private Network)

VPN creates a secure tunnel between:
- user device
- company network

---

# Startup Use Case

Employees use VPN to:
- access internal dashboards
- connect to databases
- work remotely securely

---

# Common VPN Issues

| Problem | Cause |
|---|---|
| Cannot connect | authentication failure |
| Slow connection | routing overhead |
| No access to apps | misconfigured VPN |

---

# Firewalls

A firewall controls:
- what traffic is allowed
- what traffic is blocked

---

# Real Startup Example

Firewall may block:
- unauthorized IPs
- suspicious traffic
- unknown ports

---

# Why Firewalls Matter

They protect:
- company data
- internal systems
- APIs
- production servers

---

# Client-Server Model

Most internet systems use this model.

---

# Client

The user device:
- browser
- mobile app
- desktop app

---

# Server

The system that:
- processes requests
- stores data
- returns responses

---

# Real Startup Flow

1. user opens app
2. client sends request
3. server processes it
4. server responds
5. client displays result

---

# API Communication (Important)

APIs are just structured internet communication.

Example:
```http
GET /users
```

Returns:
```json
[
  {"name": "User1"},
  {"name": "User2"}
]
```

---

# Real Startup Support Scenario

> “The dashboard is not loading data”

Possible causes:
- API failure
- DNS issue
- authentication error
- server down
- network timeout

---

# Troubleshooting Internet Issues

Support engineers follow steps:

---

## Step 1: Check connectivity

```bash
ping google.com
```

---

## Step 2: Check DNS

```bash
nslookup google.com
```

---

## Step 3: Check IP

```bash
ipconfig
```

---

## Step 4: Check route

```bash
tracert google.com
```

---

# Common Startup Network Problems

| Problem | Cause |
|---|---|
| No internet | Wi-Fi/router issue |
| API failure | server down |
| Slow app | latency |
| Login failure | DNS/auth issue |

---

# Real Startup Incident Example

A SaaS startup experiences:

> “Users cannot log in”

Investigation shows:
- DNS misconfiguration
- authentication service unreachable
- API gateway failure

---

# Mental Model for Engineers

Always think in layers:

## 1. Device
## 2. Network
## 3. DNS
## 4. Server
## 5. Application
## 6. API
## 7. Database

---

# Real Skills Built Here

This lesson builds:
- network thinking
- troubleshooting discipline
- API understanding
- system awareness
- production reasoning

---

# Mini Exercise

## Scenario

A user says:

> “Slack is not loading but my Wi-Fi is working.”

---

## Your Task

Check:
- DNS
- API reachability
- VPN status
- server status
- latency

---

# Key Takeaways

- Internet is a system of connected computers
- IP addresses identify devices
- DNS translates names to IPs
- HTTP/HTTPS powers web communication
- Packets carry data across networks
- APIs are structured internet communication
- Support engineers troubleshoot across layers

---

# Next Lesson

Continue to:

```bash
command-line-basics.md
```

The next lesson introduces:
- terminal usage
- system control via commands
- startup engineering workflows
- automation foundations
