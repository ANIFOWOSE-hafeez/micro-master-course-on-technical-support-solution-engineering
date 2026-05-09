# Command Line Basics

> Learn the command line because modern support engineers, solution engineers, cloud engineers, and startup technical teams rely on it daily.

The command line is one of the most important technical skills in engineering.

Many beginners avoid it because it looks intimidating.

In reality:
- the command line is faster
- more powerful
- easier to automate
- essential for cloud and startup environments

Modern technical teams use the command line for:
- troubleshooting
- deployments
- automation
- monitoring
- cloud management
- server administration
- DevOps workflows
- debugging production systems

This lesson teaches command line fundamentals using real startup engineering examples.

---

# Learning Goals

By the end of this lesson, learners should understand:

- what the command line is
- why engineers use it
- terminal vs shell
- navigating directories
- managing files
- viewing logs
- running scripts
- inspecting systems
- startup engineering workflows
- Linux vs Windows CLI basics
- common support troubleshooting commands

---

# What Is the Command Line?

The command line allows users to interact with a computer using text commands instead of graphical interfaces.

Instead of:
- clicking buttons
- opening menus
- dragging files

you type commands directly.

---

# Real Startup Example

A startup backend server crashes at 2 AM.

There is:
- no graphical desktop
- no mouse
- no visual interface

The engineer connects remotely using SSH and investigates entirely from the terminal.

This is extremely common in:
- cloud systems
- Linux servers
- production environments

---

# Why Engineers Use the Command Line

| Reason | Explanation |
|---|---|
| Faster workflows | Commands are quicker than clicking |
| Automation | Scripts can repeat tasks |
| Remote management | Servers often have no GUI |
| Better troubleshooting | Deep system visibility |
| Production environments | Cloud systems rely heavily on CLI |

---

# Real Startup Tasks Done in CLI

Support and solution engineers use the command line to:
- inspect logs
- restart services
- monitor servers
- deploy applications
- debug APIs
- automate workflows
- manage cloud systems
- test networking
- check system health

---

# Terminal vs Shell

This confuses many beginners.

---

# Terminal

The terminal is:
> the application window where commands are typed.

Examples:
- Windows Terminal
- PowerShell
- iTerm2
- GNOME Terminal

---

# Shell

The shell is:
> the command interpreter.

Examples:
- Bash
- Zsh
- PowerShell
- Fish

The shell processes commands.

---

# Common Startup Environment

Most startups use:
- macOS terminals
- Linux shells
- cloud Linux servers

This makes command line skills extremely valuable.

---

# Opening the Command Line

---

# Windows

## Command Prompt

Open:
```powershell
cmd
```

---

## PowerShell

Open:
```powershell
powershell
```

---

## Windows Terminal

Modern recommended terminal for Windows.

---

# macOS

Open:
```bash
Terminal
```

---

# Linux

Open:
```bash
Terminal
```

---

# First Important Concept: Current Directory

The terminal always operates from a location called:
> the current working directory

---

# View Current Directory

Linux/macOS:
```bash
pwd
```

Example output:
```bash
/home/hafeez/projects
```

---

# Windows PowerShell

```powershell
pwd
```

Example:
```powershell
Path
----
C:\Users\Hafeez
```

---

# Listing Files

---

# Linux/macOS

```bash
ls
```

Detailed view:
```bash
ls -la
```

---

# Windows

```powershell
dir
```

---

# Real Startup Example

An engineer investigates:
```bash
/app/logs/
```

to check:
- application logs
- deployment artifacts
- configuration files

---

# Changing Directories

---

# Linux/macOS

```bash
cd folder-name
```

Example:
```bash
cd logs
```

Go back:
```bash
cd ..
```

---

# Windows

```powershell
cd logs
```

---

# Important Navigation Symbols

| Symbol | Meaning |
|---|---|
| `.` | Current directory |
| `..` | Parent directory |
| `~` | Home directory |

---

# Example

Go home:
```bash
cd ~
```

---

# Creating Directories

Linux/macOS:
```bash
mkdir logs
```

Windows:
```powershell
mkdir logs
```

---

# Creating Files

Linux/macOS:
```bash
touch app.log
```

Windows:
```powershell
New-Item app.log
```

---

# Viewing File Contents

Linux/macOS:
```bash
cat app.log
```

Windows:
```powershell
type app.log
```

---

# Real Startup Usage

Support engineers constantly inspect:
- logs
- configs
- deployment files
- monitoring outputs

from the command line.

---

# Copying Files

Linux/macOS:
```bash
cp app.log backup.log
```

Windows:
```powershell
copy app.log backup.log
```

---

# Moving/Renaming Files

Linux/macOS:
```bash
mv old.txt new.txt
```

Windows:
```powershell
move old.txt new.txt
```

---

# Deleting Files

Linux/macOS:
```bash
rm app.log
```

Windows:
```powershell
del app.log
```

---

# Important Warning

This command:
```bash
rm -rf
```

can permanently destroy files.

Production engineers use it carefully.

---

# Viewing Running Processes

---

# Linux/macOS

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

# Windows

```powershell
tasklist
```

---

# Real Startup Scenario

An employee says:
> "My laptop is freezing."

Engineer checks:
- CPU usage
- RAM usage
- background processes

using command-line tools.

---

# Monitoring System Resources

---

# Linux

Memory:
```bash
free -h
```

Disk:
```bash
df -h
```

CPU:
```bash
top
```

---

# Windows

System information:
```powershell
systeminfo
```

---

# Networking Commands

Support engineers constantly troubleshoot networking.

---

# Check IP Address

Linux/macOS:
```bash
ip a
```

Older systems:
```bash
ifconfig
```

Windows:
```powershell
ipconfig
```

---

# Test Connectivity

```bash
ping google.com
```

---

# Real Startup Example

An employee cannot access:
- Slack
- internal dashboards
- APIs

Engineer tests:
- internet connectivity
- DNS resolution
- VPN connection

using CLI tools.

---

# DNS Testing

Linux/macOS:
```bash
nslookup google.com
```

Windows:
```powershell
nslookup google.com
```

---

# Viewing Logs

One of the most important support skills.

---

# Linux Logs

```bash
tail -f app.log
```

This streams logs live.

---

# Real Startup Example

Production API crashes.

Engineer watches:
```bash
tail -f /var/log/api.log
```

to identify:
- errors
- failed requests
- crashes

---

# Searching Files

Linux/macOS:
```bash
find . -name "*.log"
```

Search text:
```bash
grep ERROR app.log
```

---

# Why This Matters

Production systems generate massive logs.

Engineers search logs constantly.

---

# Running Programs

Example:
```bash
python app.py
```

Or:
```bash
node server.js
```

---

# Real Startup Workflow

A support automation engineer may run:
```bash
python ticket_router.py
```

to automate help desk workflows.

---

# Environment Variables

Important for:
- APIs
- cloud systems
- authentication
- deployments

---

# View Variables

Linux/macOS:
```bash
env
```

Windows:
```powershell
Get-ChildItem Env:
```

---

# Example

```bash
API_KEY=xxxxx
DATABASE_URL=xxxxx
```

---

# Security Warning

Never expose:
- secrets
- tokens
- API keys

on GitHub.

---

# Command History

Linux/macOS:
```bash
history
```

---

# Why This Matters

Useful for:
- troubleshooting
- repeating workflows
- debugging deployments

---

# Permissions

Linux uses:
```bash
chmod
```

Example:
```bash
chmod +x script.sh
```

Makes script executable.

---

# Real Startup Example

Deployment fails because:
```bash
Permission denied
```

The script lacks execution permissions.

---

# SSH (Secure Shell)

One of the most important engineering tools.

---

# Connect to Server

```bash
ssh user@server-ip
```

---

# Real Startup Usage

Engineers use SSH to:
- access cloud servers
- debug production systems
- inspect logs
- restart services

---

# Common Beginner Mistakes

| Mistake | Better Approach |
|---|---|
| Fear of terminal | Practice daily |
| Typing random commands | Understand commands first |
| Using admin/root carelessly | Minimize elevated access |
| Deleting files recklessly | Double-check paths |
| Ignoring logs | Investigate systematically |

---

# Real Startup Engineering Habits

Good engineers:
- automate repetitive tasks
- use CLI confidently
- inspect logs regularly
- organize workflows cleanly
- document commands
- troubleshoot methodically

---

# Beginner Practice Workflow

Create a practice environment:

```bash
startup-cli-practice/
├── logs/
├── scripts/
├── docs/
└── backups/
```

---

# Practice Tasks

## Task 1

Navigate directories:
```bash
cd
pwd
ls
```

---

## Task 2

Create files:
```bash
touch app.log
touch notes.txt
```

---

## Task 3

Copy files:
```bash
cp notes.txt backup.txt
```

---

## Task 4

Search logs:
```bash
grep ERROR app.log
```

---

## Task 5

Monitor system:
```bash
top
```

---

# Real Startup Simulation

Imagine:
- the production API fails
- customers cannot login
- monitoring alerts fire
- logs show authentication errors

The support engineer investigates entirely from the command line.

This is real engineering work.

---

# Skills Built in This Lesson

This lesson develops:
- technical confidence
- operational awareness
- troubleshooting habits
- Linux familiarity
- startup workflow understanding

These skills become essential later in:
- cloud engineering
- DevOps
- automation
- support engineering
- infrastructure operations

---

# Key Takeaways

- The command line is essential in startup engineering
- Most cloud systems rely heavily on CLI workflows
- Engineers use CLI for troubleshooting and automation
- Logs and monitoring are core operational skills
- Confidence comes through repetition and practice

---

# Mini Project

Create:

```bash
basic-command-line-practice-repo/
```

Include:
- directories
- logs
- scripts
- markdown notes
- command examples

Push it to GitHub.

---

# Next Lesson

Continue to:

```bash
networking-basics.md
```

The next lesson explains:
- networks
- IP addresses
- routers
- DNS
- VPNs
- internet communication
- startup infrastructure networking
