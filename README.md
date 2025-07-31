
linux_task3

🐧 Linux Task – Network Diagnostics Assignment

This repository contains my GUVI Linux assignment focused on basic network troubleshooting and system diagnostics. All tasks were executed using the WSL Ubuntu terminal and outputs logged to files.


---

✅ Tasks Performed

1. 🧠 DNS Resolution (nslookup)

Resolved the domain guvi.in to its IP addresses using the nslookup command:

nslookup guvi.in > guvi_info.txt
batcat guvi.in_info.txt > guvi.in.txt

nslookup: Queries DNS to fetch IP info.

batcat: Used for formatting output with borders and line numbers.


Captured both IPv4 and IPv6 entries. Final readable version stored in guvi.in.txt.


---

2. 📶 Ping to Check Reachability

Used ping to test if the domain was reachable and log packet statistics:

ping guvi.in -c 3

-c 3: Limits ping to 3 packets.

Response times and packet loss stats confirm connectivity.



---

3. 🔐 Port Availability via Telnet

Checked if port 9000 on guvi.com was open:

telnet guvi.com 9000

Connection opened and stagnated with no resolution.

Also tested port 80 for baseline reference.



---

4. 📊 CPU & Memory Usage Snapshot

Used htop cmd for better a graphical representation.
  
Collected system performance data using top:

top -b -n 1 > server_cpumemory.txt

-b: Batch mode

-n 1: Single snapshot

Logged resource usage like CPU %, memory allocation, and running processes.


Used batcat for structured output:

batcat server_cpumemory.txt


---

🧰 Tech Stack

WSL Ubuntu (Windows Subsystem for Linux)

Bash Shell

Git & GitHub



---

📚 References

LinuxCommand.org – CLI fundamentals

KodeKloud Linux Labs – Terminal practice

Ray Yao - Linux CLI (cover all essential Linux commands) Beginners guide



---

📸 Screenshots

IP resolution from nslookup

Ping response log

Telnet attempt and connection status

CPU/memory output from top

All commands executed in practice directory to isolate changes



---

📎 Submission

Submitted for GUVI DevOps Linux Assignment (Task 3).
All required files and screenshots have been organized and pushed to GitHub as per submission guide.


---

🧠 Reflections

This task reinforced real-world troubleshooting habits:

Always start with DNS resolution before connectivity or port checks.

Resource monitoring can be logged cleanly with simple flags.

batcat continues to be my preferred tool for structured CLI output.







