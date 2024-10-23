python-EOL-checker

A lightweight Bash tool that identifies dependencies on End-of-Life (EOL) Python versions across your system. This tool scans for outdated Python binaries, files referencing them, running processes, and virtual environments using them.

Usage:

Clone the Repository:
bash
Copy code
git clone https://github.com/your-username/python-EOL-checker.git
cd python-EOL-checker
Make the Script Executable:
bash
Copy code
chmod +x python-EOL-checker
Run the Script:
bash
Copy code
sudo ./python-EOL-checker

What the Tool Does

-- Lists any EOL Python binaries found on your system.
-- File References: Scans system files for explicit references to outdated Python binaries.
-- Running Processes: Identifies currently running processes using EOL Python.
-- Virtual Environments: Finds virtual environments using old Python versions.

Example Output:

======================================================
| EOL Python Version Dependency Check Results        |
======================================================
[+] Installed EOL Python Versions:
| Python 2.7.18
| Python 3.5.10

[+] Files Referencing EOL Python Versions:
| /usr/bin/python2.7
| /etc/cron.d/python2-job

[+] Running Processes Using EOL Python Versions:
| root     12345  0.0  0.1 /usr/bin/python2.7

[+] Virtual Environments Using EOL Python Versions:
| /home/user/venv/bin/python2.7
======================================================

Requirements

Bash (default on most Linux systems)
Root access (required to search system-wide directories and running processes)

Troubleshooting:

If a section shows "None found," it means the scan found no relevant results in that category.
Make sure you run the script with sudo to allow access to all system directories.

License

This tool is licensed under the MIT License.

Created by grimmtar.
