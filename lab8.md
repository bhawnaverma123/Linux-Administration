**Lab Experiment 8**

Experiment a:
Write shell scripts to print system information.

Command to be used:
nano lab8a.sh

#!/bin/bash
# System Information Script
echo "===== System Information ====="
echo "Hostname: $(hostname)"
echo "Operating System: $(lsb_release -d | cut -f2-)"
echo "Kernel Version: $(uname -r)"
echo "Uptime: $(uptime -p)"
echo -e "\n===== CPU Information ====="
cat /proc/cpuinfo | grep 'model name' | uniq
echo -e "\n===== Memory Information ====="
free -h
echo -e "\n===== Disk Usage ====="
df -h
echo -e "\n===== Network Information ====="
ip a | grep inet
echo -e "\n===== Running Processes ====="
top -b -n 1 | head -10

chmod +x system_info.sh

./system_info.sh


-----------------------------------------------------------------
Experiment b:
Write shell script to perform basic mathematical calculation.

Command to be used:

-----------------------------------------------------------------
Experiment c:
Use redirection operators to store the output of commands.

Command to be used:
