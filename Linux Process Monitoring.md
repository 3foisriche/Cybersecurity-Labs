# Linux Process Monitoring and System Security Lab

## Objective
Learn how Linux processes work, monitor system performance, and recognize potentially suspicious activity.

## Lab Environment
- Platform: Hack The Box Academy
- Operating system: Linux
- Topics: Processes, CPU, memory, and system monitoring

## 1. List Running Processes
```bash
ps
ps aux
```
The `ps` command displays process information. `ps aux` provides a more detailed list of running processes.

## 2. Monitor System Activity
```bash
top
```
The `top` command displays live process activity, CPU usage, and memory usage.

## 3. Explore htop
```bash
htop
```
The `htop` command provides an interactive view of system processes when the tool is installed.

## 4. Find a Process
```bash
pgrep -a bash
```
This command searches for processes named `bash` and displays their process IDs and command lines.

## 5. End a Process Safely
```bash
kill <PID>
```
Replace `<PID>` with the process ID of a process you own and are authorized to stop. The default signal requests graceful termination. Do not stop unknown or critical processes.

## 6. Check System Resources
```bash
free -h
uptime
```
`free -h` shows memory usage in a readable format. `uptime` shows how long the system has been running and its load averages.

## Security Importance
Process monitoring helps cybersecurity analysts identify unusual activity, investigate performance issues, and understand which programs are running.

## Learning Goals
- Understand process IDs (PIDs).
- Monitor CPU and memory usage.
- Locate running processes.
- Recognize unexpected processes for further investigation.
- Understand safe process termination.

## Practice Status
This document is a learning guide. Commands and results should be verified during hands-on practice.
