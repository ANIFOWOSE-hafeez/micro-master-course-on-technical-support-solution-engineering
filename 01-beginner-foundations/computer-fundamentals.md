# Computer Fundamentals

> Learn how computers actually work so troubleshooting, support, automation, and engineering concepts make sense later.

This lesson builds the foundation for everything else in Technical Support and Solution Engineering.

Without understanding computer fundamentals, later topics like:
- troubleshooting
- networking
- cloud
- APIs
- automation
- monitoring
- scripting

will feel confusing and disconnected.

This lesson explains computers in a practical, startup-oriented way using real-world engineering examples.

---

# Learning Goals

By the end of this lesson, learners should understand:

- what a computer actually is
- how software interacts with hardware
- how operating systems work
- how applications run
- how memory and storage differ
- how data moves through a system
- how startup systems rely on computers
- common performance bottlenecks
- beginner troubleshooting logic

---

# What Is a Computer?

A computer is a machine that:
1. receives input
2. processes information
3. stores data
4. produces output

---

# Simple Real-World Example

At a startup company:

A remote employee opens Slack and joins a video meeting.

What happens behind the scenes?

The computer:
- receives mouse and keyboard input
- loads Slack from storage into memory
- uses CPU power to process the application
- uses internet networking hardware
- renders graphics on the screen
- outputs audio through speakers

This is why support engineers must understand:
- hardware
- operating systems
- networking
- applications
- storage
- memory

because problems can happen at any layer.

---

# Main Parts of a Computer

Every computer has several important components.

---

# 1. CPU (Central Processing Unit)

## What It Does

The CPU is the brain of the computer.

It:
- processes instructions
- runs applications
- performs calculations
- executes operating system tasks

---

## Real Startup Example

When a support engineer runs:
```bash
python monitor.py
```

the CPU executes:
- Python instructions
- operating system operations
- memory allocation
- network requests

---

## Common CPU Problems

| Problem | Example |
|---|---|
| High CPU usage | Laptop becomes slow |
| Overheating | System shuts down |
| Too many processes | Applications freeze |
| Malware | CPU spikes abnormally |

---

## Beginner Troubleshooting Example

A user says:

> "My laptop is extremely slow."

A support engineer checks:
- Task Manager (Windows)
- Activity Monitor (Mac)
- top/htop (Linux)

Possible discovery:
```bash
Chrome using 95% CPU
```

---

# 2. RAM (Memory)

## What RAM Does

RAM stores temporary working data while applications are running.

RAM is:
- fast
- temporary
- volatile

When power goes off:
RAM data disappears.

---

# RAM vs Storage

| RAM | Storage |
|---|---|
| Temporary | Permanent |
| Very fast | Slower |
| Used while apps run | Used to save files |
| Clears on shutdown | Persists after reboot |

---

# Real Startup Example

A company employee opens:
- Slack
- Zoom
- Chrome
- VS Code
- Spotify

Each application consumes RAM.

Too many apps:
→ system slows down.

---

# Common RAM Problems

| Problem | Result |
|---|---|
| Low RAM | System lag |
| Memory leak | App crashes |
| Too many browser tabs | Freezing |
| Faulty RAM | Random reboots |

---

# Support Engineering Reality

A huge amount of IT support tickets involve:
- low memory
- browser overload
- too many startup applications

Understanding RAM helps solve problems faster.

---

# 3. Storage

## What Storage Does

Storage permanently saves:
- files
- applications
- operating systems
- databases
- logs

---

# Types of Storage

| Type | Speed | Common Use |
|---|---|---|
| HDD | Slow | Older systems |
| SSD | Fast | Modern laptops |
| NVMe SSD | Very fast | High-performance systems |

---

# Real Startup Example

A support engineer investigates:

> "The application takes forever to start."

Possible cause:
- slow HDD
- disk nearly full
- corrupted files

---

# Common Storage Problems

| Problem | Result |
|---|---|
| Full disk | Updates fail |
| Slow drive | Long boot times |
| Disk corruption | Missing files |
| SSD failure | Data loss |

---

# Beginner Troubleshooting Example

Check disk usage:

Windows:
```powershell
Get-PSDrive
```

Linux/Mac:
```bash
df -h
```

---

# 4. Motherboard

## What It Does

The motherboard connects:
- CPU
- RAM
- storage
- networking
- peripherals

Think of it as the system communication hub.

---

# 5. GPU (Graphics Processing Unit)

## What It Does

The GPU handles:
- graphics
- rendering
- video
- visual workloads

---

# Startup Engineering Relevance

GPUs are important in:
- AI systems
- machine learning
- video rendering
- gaming startups
- data science platforms

---

# 6. Network Interface Card (NIC)

## What It Does

The NIC connects the computer to networks.

Without networking:
- Slack fails
- Zoom disconnects
- cloud systems become unreachable

---

# Real Support Scenario

User complaint:
> "Internet is not working."

Possible causes:
- Wi-Fi disabled
- NIC driver issue
- VPN problem
- router problem
- DNS issue

---

# 7. Power Supply

## What It Does

Provides electrical power to system components.

---

# Symptoms of Power Problems

| Symptom | Possible Cause |
|---|---|
| Random shutdowns | Bad power supply |
| No boot | Power failure |
| Restart loops | Voltage issues |

---

# Software vs Hardware

This distinction is extremely important.

---

# Hardware

Physical components:
- CPU
- RAM
- motherboard
- keyboard
- monitor

---

# Software

Programs and instructions:
- Windows
- Slack
- Chrome
- Python
- Zoom

---

# Startup Support Example

User says:
> "Slack crashes constantly."

Possible issue types:

| Hardware | Software |
|---|---|
| Faulty RAM | Corrupted Slack app |
| Overheating | OS bug |
| Disk failure | Plugin conflict |

Support engineers must determine:
- hardware problem?
or
- software problem?

---

# What Is an Operating System?

The operating system (OS) manages:
- hardware
- applications
- memory
- files
- permissions
- networking

Examples:
- Windows
- Linux
- macOS

---

# Why Operating Systems Matter

Every startup relies heavily on operating systems for:
- laptops
- servers
- cloud systems
- databases
- containers

---

# What Are Applications?

Applications are programs built on top of the operating system.

Examples:
- Slack
- Zoom
- VS Code
- Chrome
- Postman

Applications depend on:
- CPU
- RAM
- storage
- networking
- operating system APIs

---

# Input → Process → Output

This is one of the most important concepts in computing.

---

# Example

A user logs into a support portal.

## Input
- keyboard typing
- mouse click

## Process
- application validates credentials
- server checks database
- authentication occurs

## Output
- dashboard loads

---

# Understanding Performance

Support engineers constantly diagnose:
- slowness
- freezing
- crashing
- network issues

Understanding performance basics helps massively.

---

# Common Performance Bottlenecks

| Bottleneck | Symptoms |
|---|---|
| CPU | High processing delays |
| RAM | Freezing |
| Disk | Slow loading |
| Network | Lag |
| Application | Crashes |

---

# Real Startup Incident Example

A customer support platform becomes slow.

Possible causes:
- overloaded database
- high CPU usage
- memory exhaustion
- cloud scaling issue
- network congestion

Support engineers investigate layer by layer.

---

# How Startup Systems Actually Work

Modern startups rely on:
- laptops
- cloud servers
- APIs
- SaaS tools
- databases
- monitoring systems

All of these are still computers underneath.

Understanding computer fundamentals helps learners:
- troubleshoot better
- understand infrastructure faster
- communicate technically
- automate intelligently

---

# Beginner Support Mindset

A beginner support engineer should always think:

## What changed?
## What layer is failing?
## Is it hardware?
## Is it software?
## Is it networking?
## Is it permissions?
## Is it performance?
## Is it user error?

This mindset becomes extremely valuable later.

---

# Common Beginner Mistakes

| Mistake | Better Approach |
|---|---|
| Guessing randomly | Investigate systematically |
| Restarting endlessly | Check logs first |
| Ignoring resource usage | Check CPU/RAM/disk |
| Blaming users immediately | Reproduce issue carefully |

---

# Real Startup Skills Built Here

This lesson develops:
- systems thinking
- troubleshooting logic
- performance awareness
- operational reasoning

These skills are foundational for:
- Technical Support
- Solution Engineering
- Cloud Engineering
- DevOps
- Site Reliability Engineering

---

# Important Commands to Know

---

# Windows

Open Task Manager:
```powershell
Ctrl + Shift + Esc
```

Check disk usage:
```powershell
Get-PSDrive
```

Check memory:
```powershell
systeminfo
```

---

# Linux / macOS

Check CPU and memory:
```bash
top
```

Better monitoring:
```bash
htop
```

Check disk usage:
```bash
df -h
```

Check memory:
```bash
free -h
```

---

# Mini Exercise

## Scenario

A startup employee complains:

> "My laptop freezes every time I open Zoom and Chrome together."

---

# Practice Investigation

Ask:
- How much RAM exists?
- How many tabs are open?
- Is CPU usage high?
- Is storage full?
- Is the system overheating?

---

# Expected Learning Outcome

The goal is NOT memorization.

The goal is learning how engineers think.

---

# Key Takeaways

- Computers are systems of interacting components
- Hardware and software depend on each other
- Support engineers troubleshoot layer by layer
- Performance problems usually have root causes
- Startup systems still rely on computer fundamentals

---

# Next Lesson

Continue to:

```bash
operating-systems-basics.md
```

The next lesson explains how operating systems manage hardware, applications, users, files, permissions, and processes.
