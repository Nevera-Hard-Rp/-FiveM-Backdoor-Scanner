# 📚 FiveM Backdoor Scanner - User Guide

## 📑 Table of Contents
1. [📥 Installation](#installation)
2. [🧪 Basic Usage](#basic-usage)
3. [🔍 Scan Modes](#scan-modes)
4. [📈 Understanding Results](#understanding-results)
5. [🛠️ Troubleshooting](#troubleshooting)

---

## 📥 Installation

### ✅ Prerequisites
- Ubuntu 20.04+ (or compatible Linux distribution)
- Python 3.7 or higher
- Git
- 100MB free disk space

### 🛠️ Detailed Installation Steps

```bash
# 1. Update system packages
sudo apt update
sudo apt install python3-full python3-venv python3-pip python3-tk

# 2. Clone the repository
git clone https://github.com/yourusername/fivem-backdoor-scanner.git
cd fivem-backdoor-scanner

# 3. Create a virtual environment
python3 -m venv scanner_env

# 4. Activate the virtual environment
source scanner_env/bin/activate

# 5. Install dependencies
pip install -r requirements.txt

# 6. Make the CLI executable
chmod +x fivem_scanner_cli.py
🧪 Basic Usage
🔃 Entering the Scanner Environment
bash
Copy
Edit
# Navigate to the scanner directory
cd /path/to/fivem-backdoor-scanner

# Activate virtual environment
source scanner_env/bin/activate

# Prompt will change to:
(scanner_env) user@hostname:~/fivem-backdoor-scanner$
🔍 Scan Modes
⚙️ Standard Scan
bash
Copy
Edit
./fivem_scanner_cli.py /path/to/fivem/resources
🧠 Detailed Scan (shows code snippets)
bash
Copy
Edit
./fivem_scanner_cli.py /path/to/fivem/resources --detailed
🚀 Quick Scan (high-risk areas only)
bash
Copy
Edit
./fivem_scanner_cli.py /path/to/fivem/resources --quick
💾 Saving Results
📄 Save as TXT
bash
Copy
Edit
./fivem_scanner_cli.py /path/to/resources -o scan_report.txt -f txt
🧾 Save as JSON
bash
Copy
Edit
./fivem_scanner_cli.py /path/to/resources -o scan_report.json -f json
⏱️ Save with Timestamp
bash
Copy
Edit
./fivem_scanner_cli.py /path/to/resources -o scan_$(date +%Y%m%d_%H%M%S).txt -f txt
📈 Understanding Results
During a scan, the CLI outputs results in real time:

yaml
Copy
Edit
[*] Scanning: /home/fivem/resources
[*] Files scanned: 150 | Threats found: 3

🚨 CRITICAL THREAT FOUND:
📁 Resource: suspicious_resource
📄 File: server/main.lua
📍 Line: 45
🎯 Severity: 10/10
💬 Hex encoded backdoor detected

[✓] Scan complete in 2.45 seconds
🛠️ Troubleshooting
Issue	Solution
Permission denied	Run with sudo or check file permissions
ModuleNotFoundError	Activate virtual environment before running
Too slow scan	Use --quick mode or exclude large folders
No threats detected	Ensure correct path is provided to the script
Output empty	Use --detailed or check file extensions

✅ Tip: For scheduled scans, add to crontab:

bash
Copy
Edit
0 3 * * * cd /home/fivem-scanner && ./scanner_env/bin/python fivem_scanner_cli.py /home/fivem/resource
