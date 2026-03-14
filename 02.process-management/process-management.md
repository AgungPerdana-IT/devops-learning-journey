# Process Management in Linux


## Viewing Process
1. `ps aux` - View all running process
2. `ps -u username` - View processes for a specific user
3. `ps -C processname` - Show a process by name
4. `pgrep processname` - Find a process by name and return its PID
5. `pidof processname` - Find the PID of a runnng program

# Managing Processes
6. `kill PID` - Terminate a process by PID
7. `pkill processname` - Terminate a process by name
8. `kill -9 PID` - Force kill a process
9. `pkill -9 processname` - Kill all instances of a process
10. `kill -STOP PID` - Stop a running porcess
11. `kill -CONT PID` - Resume a stopped process
12. `renice -n 10 -p PID` - Lower priority of a process
13. `renice -n -5 -p PID` - Increase prioity of a process (requires root)

# Background & Foreground Processes
14. `command &` - Run a command in the background
15. `jobs` - List background jobs
16. `fg %jobnumber` - Bring a ob to the foreground
17. `Ctrl + Z` Suspend a running process
18. `bg %jobnumber~ - Resume a suspended process in the background

# Monitoring System Processes
19. `top` - Interactive process viewer
20. `htop` - User-friendly process viewer (requires installation)

# Deamon Process Management
21. `systemctl list-units --type=service` - List all system deamons
22. `systemctl start service-name` - Start a deamon/service
23. `systemctl stop service-name` - Stop a deamon/service
24. `systemctl enable service-name` - Enable a service at startup