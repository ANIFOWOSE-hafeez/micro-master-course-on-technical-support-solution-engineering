# File Systems and Folders

> Learn how computers organize data because every support engineer, automation engineer, and solution engineer works with files daily.

Understanding file systems is critical for:
- troubleshooting
- scripting
- automation
- cloud systems
- deployments
- logs
- backups
- security
- documentation

Most technical work eventually involves:
- locating files
- managing directories
- editing configurations
- analyzing logs
- setting permissions
- troubleshooting missing or corrupted data

This lesson explains file systems in a practical startup-focused way.

---

# Learning Goals

By the end of this lesson, learners should understand:

- what a file system is
- how folders/directories work
- how operating systems organize data
- file paths
- absolute vs relative paths
- file extensions
- permissions basics
- startup operational directory structures
- logs and configuration files
- practical file management
- common file-related support issues

---

# What Is a File System?

A file system is the method an operating system uses to:
- organize data
- store files
- retrieve files
- manage directories
- control permissions

Without file systems:
- files would be impossible to organize
- applications could not store data properly
- operating systems would become chaotic

---

# Real Startup Example

A startup support platform may store:

| Type | Example |
|---|---|
| Logs | `/var/log/app.log` |
| Config files | `/etc/nginx/nginx.conf` |
| User uploads | `/uploads/` |
| Backups | `/backup/` |
| Application code | `/app/` |

Understanding where data lives is essential.

---

# What Is a File?

A file is a container for data.

Examples:
- documents
- images
- videos
- scripts
- logs
- configuration files
- databases

---

# Common File Types

| File Type | Example |
|---|---|
| Text | `.txt` |
| Markdown | `.md` |
| Python | `.py` |
| JavaScript | `.js` |
| JSON | `.json` |
| CSV | `.csv` |
| Logs | `.log` |
| Images | `.png`, `.jpg` |

---

# What Is a Folder (Directory)?

A folder organizes files.

Directories can contain:
- files
- subfolders
- other directories

---

# Real Startup Structure Example

```bash
support-platform/
├── app/
├── logs/
├── backups/
├── docs/
├── tests/
└── config/
```

This structure helps teams:
- organize code
- separate environments
- debug systems
- collaborate professionally

---

# File Paths

A file path describes where a file exists.

---

# Example

```bash
/home/support/logs/error.log
```

This means:
- `home` → directory
- `support` → subdirectory
- `logs` → subdirectory
- `error.log` → file

---

# Absolute vs Relative Paths

This is extremely important in engineering work.

---

# Absolute Path

Starts from the root of the system.

Example:
```bash
/home/startup/app/config.json
```

Always points to the same location.

---

# Relative Path

Starts from the current directory.

Example:
```bash
./config.json
```

Depends on where you currently are.

---

# Real Startup Engineering Relevance

Automation scripts often fail because:
- wrong file paths are used
- environments differ
- deployment paths change

Understanding paths prevents major problems.

---

# Root Directory

The top-level directory.

---

# Linux/macOS Root

```bash
/
```

---

# Windows Root

```powershell
C:\
```

---

# Common Linux Directories

| Directory | Purpose |
|---|---|
| `/home` | User files |
| `/etc` | Configuration files |
| `/var/log` | Logs |
| `/tmp` | Temporary files |
| `/bin` | System commands |
| `/opt` | Optional software |

---

# Why Engineers Must Know These

Production troubleshooting often requires:
- checking logs
- editing configs
- finding application files

---

# Real Startup Example

A support API crashes.

An engineer investigates:
```bash
/var/log/api/error.log
```

Without understanding file systems:
troubleshooting becomes difficult.

---

# Windows File Structure

Windows commonly uses:
```powershell
C:\Users\
C:\Program Files\
C:\Windows\
```

---

# File Extensions

File extensions describe file types.

Examples:
```bash
report.pdf
server.log
app.py
```

---

# Why Extensions Matter

Support engineers use extensions to:
- identify files quickly
- troubleshoot applications
- understand configurations
- automate workflows

---

# Important Startup File Types

---

# Log Files

Example:
```bash
application.log
```

Contain:
- errors
- warnings
- debugging information

---

# Configuration Files

Examples:
```bash
config.json
settings.yaml
.env
```

Used to control:
- application behavior
- credentials
- environments
- APIs

---

# Environment Files

Example:
```bash
.env
```

May contain:
```env
API_KEY=xxxx
DATABASE_URL=xxxx
```

---

# Important Security Rule

Never expose:
- API keys
- passwords
- secrets
- tokens

on GitHub.

---

# Hidden Files

Some files are hidden.

Linux/macOS hidden files usually begin with:
```bash
.
```

Examples:
```bash
.env
.gitignore
```

---

# Viewing Hidden Files

Linux/macOS:
```bash
ls -la
```

Windows:
Enable:
> View → Hidden Items

---

# File Permissions

Permissions control:
- who can read files
- who can edit files
- who can execute files

---

# Linux Permission Example

```bash
-rwxr-xr--
```

---

# Permission Meaning

| Symbol | Meaning |
|---|---|
| r | Read |
| w | Write |
| x | Execute |

---

# Why Permissions Matter

Incorrect permissions can:
- break applications
- expose sensitive data
- prevent services from running

---

# Real Startup Incident Example

A deployed API suddenly fails.

Cause:
```bash
Permission denied
```

The application cannot access:
```bash
config.json
```

---

# Changing Permissions

Linux:
```bash
chmod
```

Example:
```bash
chmod 755 script.sh
```

---

# Ownership

Files belong to:
- users
- groups

---

# Example

```bash
hafeez developers app.py
```

---

# Startup Relevance

Cloud servers often run services under special users:
- nginx
- postgres
- docker

Understanding ownership helps troubleshoot:
- deployment failures
- access issues
- permission errors

---

# File Operations

Support engineers constantly:
- create files
- move files
- copy files
- delete files
- rename files

---

# Linux Commands

Create file:
```bash
touch notes.txt
```

Create folder:
```bash
mkdir logs
```

Copy file:
```bash
cp app.log backup.log
```

Move file:
```bash
mv old.txt new.txt
```

Delete file:
```bash
rm file.txt
```

Delete folder:
```bash
rm -rf folder/
```

---

# Windows Commands

Create folder:
```powershell
mkdir logs
```

List files:
```powershell
dir
```

Copy:
```powershell
copy old.txt new.txt
```

Move:
```powershell
move old.txt archive\
```

Delete:
```powershell
del old.txt
```

---

# Navigating Directories

---

# Linux/macOS

Current directory:
```bash
pwd
```

List files:
```bash
ls
```

Change directory:
```bash
cd logs
```

Go up one level:
```bash
cd ..
```

---

# Windows

Current directory:
```powershell
cd
```

List files:
```powershell
dir
```

Change directory:
```powershell
cd logs
```

---

# Logs

Logs are one of the most important file types in production systems.

---

# Real Startup Example

A support engineer receives:
> "Customers cannot login."

Investigation begins in:
```bash
/var/log/
```

Possible findings:
- authentication failures
- database errors
- timeout issues
- permission problems

---

# Common Log Locations

Linux:
```bash
/var/log/
```

Application logs:
```bash
/app/logs/
```

---

# Viewing Logs

Linux:
```bash
cat app.log
```

Live logs:
```bash
tail -f app.log
```

---

# Backup Fundamentals

Good systems always protect important files.

---

# Backup Importance

Without backups:
- ransomware can destroy systems
- accidental deletions become catastrophic
- startups may lose operational data

---

# Common Backup Types

| Type | Meaning |
|---|---|
| Full | Entire system |
| Incremental | Only changes |
| Differential | Changes since full backup |

---

# Real Startup Engineering Practice

Production systems commonly back up:
- databases
- configuration files
- logs
- uploads
- application code

---

# Compression

Large files are often compressed.

Examples:
```bash
.zip
.tar.gz
```

---

# Why Compression Matters

Useful for:
- backups
- deployments
- file transfers
- cloud uploads

---

# Common Beginner Mistakes

| Mistake | Better Approach |
|---|---|
| Deleting wrong files | Verify path carefully |
| Hardcoding paths | Use variables/configs |
| Ignoring permissions | Check ownership/access |
| Uploading secrets to GitHub | Use `.gitignore` |
| Disorganized folders | Use structured directories |

---

# Startup Engineering Best Practices

Good engineers:
- organize files cleanly
- separate configs from code
- use environment variables
- document structures clearly
- back up important data
- avoid exposing secrets

---

# Real Skills Built Here

This lesson develops:
- operational awareness
- troubleshooting confidence
- systems organization
- security awareness
- production debugging habits

These become critical in:
- DevOps
- cloud engineering
- support engineering
- automation
- infrastructure work

---

# Mini Exercise

## Task 1

Create this structure manually:

```bash
startup-support-system/
├── logs/
├── backups/
├── docs/
├── scripts/
└── config/
```

---

## Task 2

Create:
```bash
app.log
```

inside:
```bash
logs/
```

---

## Task 3

Create:
```bash
README.md
```

inside:
```bash
docs/
```

---

## Task 4

Practice:
- copying files
- renaming files
- moving files
- deleting files

---

# Real Startup Simulation

Imagine:
- logs are filling storage
- configs are missing
- permissions are broken
- backups failed overnight

A support engineer must navigate the file system confidently.

---

# Key Takeaways

- File systems organize all computer data
- Support engineers constantly work with files and directories
- Logs and configuration files are critical
- Permissions heavily affect applications
- Good directory structure improves operations
- Backup awareness is essential

---

# Next Lesson

Continue to:

```bash
hardware-basics.md
```

The next lesson explains:
- hardware components
- startup device environments
- laptops
- peripherals
- device troubleshooting
- real-world hardware support workflows
