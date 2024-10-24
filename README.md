python-EOL-checker

A lightweight Bash tool that identifies dependencies on End-of-Life (EOL) Python versions across your system. This tool scans for outdated Python binaries, files referencing them, running processes, and virtual environments using them.

Usage:

Clone the Repository:

git clone https://github.com/grimmtar/python-EOL-checker.git

cd python-EOL-checker

Make the Script Executable:

chmod +x python-EOL-checker

Run the Script:

sudo ./python-EOL-checker

What the Tool Does:

-- Lists any EOL Python binaries found on your system.

-- File References: Scans system files for explicit references to outdated Python binaries.

-- Running Processes: Identifies currently running processes using EOL Python.

-- Virtual Environments: Finds virtual environments using old Python versions.

Requirements:

Bash (default on most Linux systems)
Root access (required to search system-wide directories and running processes)

Troubleshooting:

If a section shows "None found," it means the scan found no relevant results in that category.

Make sure you run the script with sudo to allow access to all system directories.

License:

This tool is licensed under the MIT License.

Created by grimmtar.
