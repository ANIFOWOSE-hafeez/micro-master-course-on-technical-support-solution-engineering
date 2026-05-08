# Operating Systems Basics

> Learn how operating systems work because every support engineer, solution engineer, and startup technical professional interacts with them daily.

Operating systems are one of the most important foundations in technical work.

Every:
- laptop
- cloud server
- SaaS platform
- monitoring tool
- automation script
- database
- support system

runs on an operating system.

Understanding operating systems helps learners:
- troubleshoot intelligently
- automate confidently
- navigate systems professionally
- support users effectively
- understand cloud infrastructure faster

---

# Learning Goals

By the end of this lesson, learners should understand:

- what an operating system is
- why operating systems exist
- how operating systems manage hardware
- processes and applications
- users and permissions
- files and storage
- startup system environments
- Windows vs Linux vs macOS
- system performance basics
- operating system troubleshooting

---

# What Is an Operating System?

An operating system (OS) is the software layer between:
- hardware
and
- applications/users

The operating system controls:
- CPU access
- memory
- files
- storage
- networking
- permissions
- applications
- devices

Without an operating system:
- applications cannot run properly
- hardware cannot be managed efficiently
- users cannot interact easily with computers

---

# Simple Real-World Startup Example

An employee opens:
- Slack
- Zoom
- Chrome

The operating system:
- allocates memory
- schedules CPU usage
- manages internet connections
- handles notifications
- controls permissions
- manages storage access

---

# Main Responsibilities of an Operating System

| Responsibility | Example |
|---|---|
| Process management | Running applications |
| Memory management | Allocating RAM |
| File management | Saving documents |
| User management | Login accounts |
| Device management | Keyboard/mouse support |
| Security | Permissions |
| Networking | Internet access |

---

# Types of Operating Systems

---

# 1. Windows

## Common Usage

Widely used in:
- companies
- enterprise environments
- business laptops
- IT support environments

---

## Why Support Engineers Use Windows

Many organizations rely heavily on:
- Active Directory
- Microsoft 365
- Windows laptops
- Windows servers

---

## Real Startup Use Cases

- employee laptops
- onboarding systems
- endpoint management
- Office applications
- support tooling

---

# Strengths

| Strength | Explanation |
|---|---|
| User-friendly | Easy for non-technical users |
| Enterprise tools | Strong business ecosystem |
| Compatibility | Supports many applications |

---

# Weaknesses

| Weakness | Explanation |
|---|---|
| Resource-heavy | Can consume more RAM |
| Licensing costs | Enterprise licensing expensive |
| Malware targeting | Common attack target |

---

# 2. Linux

## Common Usage

Widely used in:
- cloud servers
- DevOps
- backend systems
- startup infrastructure
- containers
- APIs

---

# Why Linux Matters So Much

A huge percentage of:
- cloud systems
- production servers
- APIs
- databases
- Docker containers

run on Linux.

---

# Real Startup Examples

Linux powers:
- AWS EC2 instances
- Kubernetes clusters
- PostgreSQL servers
- backend APIs
- monitoring systems

---

# Strengths

| Strength | Explanation |
|---|---|
| Stable | Great for servers |
| Lightweight | Efficient resource usage |
| Powerful CLI | Excellent automation |
| Open source | Flexible |

---

# Weaknesses

| Weakness | Explanation |
|---|---|
| Learning curve | CLI-heavy |
| Some desktop apps missing | Limited commercial software |

---

# 3. macOS

## Common Usage

Popular among:
- developers
- startup founders
- designers
- engineering teams

---

# Why Engineers Like macOS

macOS combines:
- Unix/Linux-style terminal
- polished UI
- strong developer tooling

---

# Startup Engineering Reality

Many startup engineers use:
- MacBooks
- Linux servers
- cloud infrastructure

This combination is extremely common.

---

# What Happens When a Computer Boots?

Booting means starting the computer.

---

# Simplified Boot Process

1. Power turns on
2. BIOS/UEFI starts
3. Hardware is checked
4. Operating system loads
5. User login appears

---

# Why Support Engineers Care

Boot failures are common support issues.

Examples:
- corrupted OS
- damaged bootloader
- failed disk
- hardware failure

---

# Kernel

## What Is the Kernel?

The kernel is the core part of the operating system.

It controls:
- CPU
- memory
- hardware communication
- processes

---

# Simple Analogy

Think of the kernel as:
> the operating system traffic controller

---

# User Space vs Kernel Space

| Area | Purpose |
|---|---|
| Kernel space | Core system operations |
| User space | Applications |

---

# Real Example

Slack runs in:
- user space

Disk drivers run in:
- kernel space

---

# Processes

## What Is a Process?

A process is:
> a running instance of a program

Examples:
- Chrome
- Slack
- Python scripts
- Zoom

---

# Real Startup Example

An employee opens:
- 10 Chrome tabs
- Slack
- Zoom
- Spotify

Each creates processes consuming:
- CPU
- RAM
- networking
- storage access

---

# Why Processes Matter

Support engineers troubleshoot:
- high CPU usage
- frozen apps
- memory leaks
- crashing processes

daily.

---

# Process Monitoring

---

# Windows

Task Manager:
```powershell
Ctrl + Shift + Esc
```

---

# Linux/macOS

View running processes:
```bash
ps aux
```

Live monitoring:
```bash
top
```

Better monitoring:
```bash
htop
```

---

# Memory Management

The operating system controls:
- RAM allocation
- memory cleanup
- application access

---

# Real Support Scenario

User says:
> "My system freezes constantly."

Possible causes:
- low RAM
- memory leak
- too many applications

---

# Swap Memory / Virtual Memory

When RAM becomes full:
the operating system may use storage temporarily as backup memory.

This is slower than RAM.

---

# Symptoms of Low Memory

| Symptom | Explanation |
|---|---|
| Freezing | RAM exhaustion |
| Slow application switching | Heavy swapping |
| Crashes | Memory limits reached |

---

# File Systems

Operating systems organize data using file systems.

---

# Examples

| OS | Common File System |
|---|---|
| Windows | NTFS |
| Linux | ext4 |
| macOS | APFS |

---

# Why File Systems Matter

Support engineers troubleshoot:
- missing files
- permission issues
- corrupted disks
- storage failures

---

# Users and Permissions

Operating systems manage:
- users
- groups
- permissions

---

# Startup Security Reality

Not every employee should access:
- finance systems
- production servers
- HR databases

Permissions matter heavily.

---

# Types of Accounts

| Account Type | Purpose |
|---|---|
| Standard user | Normal work |
| Administrator | Full access |
| Service account | Automation/system tasks |

---

# Real Startup Example

A support engineer may:
- reset passwords
- unlock accounts
- assign permissions
- disable terminated employee access

---

# Networking in Operating Systems

Operating systems manage:
- Wi-Fi
- Ethernet
- VPN
- DNS
- internet traffic

---

# Common Support Issues

| Issue | Possible Cause |
|---|---|
| No internet | Network adapter issue |
| VPN failure | Authentication problem |
| Slow internet | DNS/network congestion |

---

# Logs

Operating systems generate logs.

Logs help engineers:
- diagnose failures
- investigate incidents
- understand system behavior

---

# Real Startup Importance

Production troubleshooting heavily depends on:
- logs
- monitoring
- alerts

---

# Windows Logs

Open Event Viewer:
```powershell
eventvwr
```

---

# Linux Logs

Common locations:
```bash
/var/log/
```

View logs:
```bash
tail -f /var/log/syslog
```

---

# Services

Services are background applications.

Examples:
- databases
- monitoring agents
- VPN services
- authentication services

---

# Real Startup Example

If the database service crashes:
- customer applications may fail

---

# Managing Services

---

# Windows

```powershell
services.msc
```

---

# Linux

Check services:
```bash
systemctl status nginx
```

Start service:
```bash
sudo systemctl start nginx
```

---

# Software Installation

Operating systems install and manage software.

---

# Windows

Usually:
- `.exe`
- `.msi`

---

# Linux

Package managers:
```bash
apt
yum
dnf
```

Example:
```bash
sudo apt install nginx
```

---

# Startup Environment Reality

Startup environments often require:
- fast deployments
- automation
- package management
- dependency handling

---

# Updates and Patching

Operating systems require updates for:
- security
- stability
- performance

---

# Real Startup Risk

Outdated systems can lead to:
- security breaches
- ransomware
- downtime
- compliance failures

---

# Common Operating System Problems

| Problem | Possible Cause |
|---|---|
| Slow system | High CPU/RAM usage |
| Random reboot | Driver/hardware issue |
| Blue screen | Kernel/driver failure |
| Application crash | Corrupted software |
| Login issue | Permission/authentication problem |

---

# Troubleshooting Mindset

A support engineer should always ask:

## Is the issue:
- hardware?
- software?
- permissions?
- networking?
- storage?
- performance?
- updates?
- drivers?

---

# Real Startup Incident Example

A startup engineer receives:

> "Nobody can access the internal dashboard."

Possible investigations:
- server offline?
- DNS issue?
- authentication service down?
- expired SSL certificate?
- cloud outage?
- application crash?

Operating system understanding becomes critical.

---

# Monitoring System Health

Support engineers constantly monitor:
- CPU usage
- RAM usage
- disk usage
- network activity
- service uptime

---

# Important Beginner Commands

---

# Windows

System info:
```powershell
systeminfo
```

IP information:
```powershell
ipconfig
```

Running tasks:
```powershell
tasklist
```

---

# Linux/macOS

System info:
```bash
uname -a
```

Memory:
```bash
free -h
```

Disk:
```bash
df -h
```

Processes:
```bash
top
```

Networking:
```bash
ip a
```

---

# Real Skills Built Here

This lesson develops:
- operational awareness
- troubleshooting confidence
- systems understanding
- production thinking

These skills become extremely important later in:
- cloud
- automation
- DevOps
- support engineering
- solution architecture

---

# Mini Exercise

## Scenario

An employee reports:
> "Slack opens very slowly and my laptop fan is always loud."

---

# Investigation Practice

Check:
- CPU usage
- RAM usage
- startup applications
- disk space
- background processes

---

# Expected Outcome

The learner should begin thinking:
- systematically
- layer by layer
- operationally

instead of randomly guessing.

---

# Key Takeaways

- Operating systems manage all system resources
- Applications depend heavily on the OS
- Linux dominates cloud/startup infrastructure
- Logs and monitoring are critical
- Permissions and processes matter heavily
- Support engineers troubleshoot methodically

---

# Next Lesson

Continue to:

```bash
file-systems-and-folders.md
```

The next lesson explains:
- directories
- files
- permissions
- storage organization
- startup operational file structures
- real engineering workflowsk
