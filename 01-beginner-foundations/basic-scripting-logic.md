# Basic Scripting Logic

> Learn how engineers think in automation workflows before writing advanced code.

This lesson is one of the most important foundations in the entire Micro-Master program.

Before becoming good at:
- Python
- PowerShell
- Bash
- automation
- APIs
- AI workflows
- DevOps

learners must first understand:
# scripting logic

Many beginners fail because they try to memorize programming syntax without understanding how engineers think.

This lesson focuses on:
- logical thinking
- automation mindset
- workflow thinking
- support engineering scenarios
- startup operational examples

---

# Learning Goals

By the end of this lesson, learners should understand:

- what scripting is
- why scripting matters in startups
- automation thinking
- variables
- conditions
- loops
- functions
- input/output
- logic flow
- debugging basics
- support automation mindset

---

# What Is a Script?

A script is:
> a set of instructions executed automatically by a computer.

Scripts help engineers:
- reduce manual work
- automate repetitive tasks
- improve consistency
- reduce operational errors
- scale workflows

---

# Real Startup Example

Imagine a startup onboarding process.

Without automation:
- create user account manually
- assign permissions manually
- send welcome email manually
- add Slack access manually
- add Google Workspace manually

This wastes time.

---

# With Scripting

A single script can:
- create the account
- assign permissions
- send notifications
- generate passwords
- create tickets automatically

This is why startups love automation.

---

# Why Scripting Matters in Technical Support

Modern support engineers are expected to automate repetitive tasks.

Examples:
- password resets
- user onboarding
- backup verification
- log cleanup
- endpoint checks
- alerting systems
- ticket routing

---

# Scripting vs Programming

| Scripting | Programming |
|---|---|
| Usually task-focused | Often larger systems |
| Automation-heavy | Application-heavy |
| Faster to write | More architecture |
| Operations-oriented | Software-engineering-oriented |

---

# Important Mindset

Good scripting is not about:
- writing fancy code

Good scripting is about:
- solving operational problems efficiently

---

# Thinking Like an Automation Engineer

Before writing scripts, ask:

## What problem repeats often?
## What steps are manual?
## What wastes time?
## What causes human error?
## What can be automated safely?

---

# Real Startup Support Example

A support team receives:
- 50 password reset requests daily

Manual process:
- verify user
- reset password
- notify employee

Automation opportunity:
- self-service password reset portal

---

# Core Building Blocks of Scripting

Every script is built from simple logic blocks.

---

# 1. Input

Scripts receive information.

Examples:
- usernames
- file names
- API responses
- user requests

---

# Example

```text
Enter your username:
```

---

# Real Startup Example

An onboarding script asks:
```text
Enter employee email:
```

---

# 2. Variables

Variables store data.

Think of variables as:
> labeled containers for information

---

# Example

```python
username = "hafeez"
```

---

# Real Startup Example

```python
ticket_priority = "high"
```

---

# Why Variables Matter

Support systems constantly store:
- usernames
- IP addresses
- ticket IDs
- timestamps
- server names
- error messages

---

# 3. Conditions (Decision Making)

Scripts often make decisions.

---

# Example Logic

```text
IF ticket priority is high
THEN escalate immediately
```

---

# Real Startup Example

```text
IF CPU usage > 90%
THEN send alert
```

---

# Condition Flow Example

```text
IF user account is locked
→ unlock account

ELSE
→ show "account already active"
```

---

# Why Conditions Matter

Most support automation relies heavily on conditions.

Examples:
- alert triggers
- monitoring systems
- authentication workflows
- onboarding logic
- escalation systems

---

# 4. Loops

Loops repeat tasks automatically.

---

# Example

Instead of manually checking:
- 100 laptops

a script loops through:
- all devices automatically

---

# Real Startup Example

A monitoring script checks:
- CPU
- RAM
- disk space

every 5 minutes.

---

# Loop Logic Example

```text
FOR every server
→ check uptime
→ record result
→ send alerts if offline
```

---

# Why Loops Matter

Loops are heavily used in:
- monitoring
- inventory scanning
- backups
- bulk operations
- automation systems

---

# 5. Functions

Functions are reusable blocks of logic.

---

# Example

Instead of rewriting:
```text
send_email()
```

multiple times,
a function allows reuse.

---

# Real Startup Example

A support automation platform may use:

```text
create_ticket()
send_alert()
reset_password()
log_event()
```

---

# Why Functions Matter

Functions improve:
- organization
- reusability
- debugging
- scalability

---

# 6. Output

Scripts produce results.

Examples:
- alerts
- logs
- reports
- dashboards
- notifications

---

# Real Startup Example

A monitoring script outputs:
```text
Server api-01 is offline
```

---

# Simple Automation Flow

```text
Receive Input
→ Process Logic
→ Make Decision
→ Execute Action
→ Produce Output
```

---

# Real Support Automation Example

```text
Ticket arrives
→ Analyze category
→ Detect urgency
→ Assign priority
→ Route to correct team
→ Notify engineer
```

This is the foundation of:
- AI Ticket Router systems
- support automation platforms

---

# Logic Trees

Support engineers constantly use logic trees.

---

# Example

```text
Can user login?

YES
→ Check application access

NO
→ Check password reset
```

---

# Why Logic Trees Matter

Troubleshooting itself is a scripting mindset.

Good engineers:
- narrow possibilities systematically
- eliminate causes logically

---

# Basic Data Types

Scripts work with different kinds of data.

---

# Text (String)

```python
"name"
```

Examples:
- usernames
- emails
- ticket titles

---

# Numbers

```python
5
100
99.5
```

Examples:
- CPU percentages
- disk usage
- response times

---

# Boolean (True/False)

```python
True
False
```

Examples:
- online/offline
- success/failure
- authenticated/not authenticated

---

# Lists

Groups of items.

Example:
```python
["server1", "server2", "server3"]
```

---

# Real Startup Example

List of endpoints:
```python
["api", "database", "auth-service"]
```

---

# Common Automation Scenarios

---

# Password Reset Automation

```text
Receive username
→ verify identity
→ generate password
→ update system
→ notify user
```

---

# Endpoint Monitoring

```text
Loop through devices
→ check status
→ detect failures
→ send alerts
```

---

# Ticket Routing

```text
Read ticket
→ classify issue
→ assign priority
→ route automatically
```

---

# Backup Verification

```text
Check backup logs
→ confirm success
→ alert if failed
```

---

# Beginner Debugging Mindset

Scripts often fail.

This is normal.

---

# Common Causes

| Problem | Example |
|---|---|
| Wrong variable | Misspelled name |
| Logic error | Wrong condition |
| Bad input | Unexpected data |
| Permission issue | Cannot access file |
| API issue | Authentication failure |

---

# Important Rule

Do not panic when scripts fail.

Real engineers debug constantly.

---

# Debugging Process

## Step 1
Reproduce the issue

## Step 2
Read the error carefully

## Step 3
Check variables

## Step 4
Check logic flow

## Step 5
Test smaller sections

---

# Real Startup Engineering Reality

Professional engineers spend massive amounts of time:
- debugging
- troubleshooting
- testing workflows

This is normal.

---

# Pseudocode

Pseudocode means:
> writing logic in human-readable steps before coding.

---

# Example

```text
IF server is offline
THEN send Slack alert
ELSE continue monitoring
```

---

# Why Pseudocode Matters

Strong engineers think before coding.

This prevents:
- messy scripts
- bad architecture
- operational confusion

---

# Beginner Scripting Exercise

---

# Scenario

A startup wants a simple employee onboarding workflow.

---

# Write Pseudocode

```text
Ask for employee name
Ask for department
Create account
Assign permissions
Send welcome message
Log onboarding event
```

---

# Real Startup Insight

This simple workflow later becomes:
- identity management systems
- HR automation
- cloud onboarding platforms

---

# Automation Thinking

The biggest shift learners must make is:

From:
```text
How do I do this manually?
```

To:
```text
How can the system do this automatically?
```

This mindset separates:
- basic support workers
from:
- high-value startup engineers

---

# Common Beginner Mistakes

| Mistake | Better Approach |
|---|---|
| Memorizing syntax only | Focus on logic |
| Writing giant scripts | Break into small functions |
| Ignoring debugging | Investigate carefully |
| Hardcoding values | Use variables |
| Automating unsafe actions | Validate first |

---

# Real Skills Built Here

This lesson develops:
- automation thinking
- logical reasoning
- systems thinking
- troubleshooting mindset
- operational awareness

These become foundational for:
- Python
- APIs
- cloud automation
- AI workflows
- DevOps
- solution engineering

---

# Mini Exercise 1

Write pseudocode for:

```text
Automatic disk space monitoring system
```

---

# Mini Exercise 2

Write pseudocode for:

```text
Simple ticket escalation workflow
```

---

# Mini Exercise 3

Write pseudocode for:

```text
Employee offboarding automation
```

---

# Key Takeaways

- Scripts automate repetitive work
- Logic matters more than syntax initially
- Conditions and loops power automation
- Functions improve organization
- Debugging is normal engineering work
- Automation thinking is a career superpower

---

# Next Lesson

Continue to:

```bash
basic-python.md
```

The next lesson begins practical Python scripting for:
- support automation
- operational tooling
- APIs
- monitoring
- startup engineering workflows
