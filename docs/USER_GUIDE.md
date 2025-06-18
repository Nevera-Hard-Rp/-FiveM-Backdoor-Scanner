# 📚 FiveM Backdoor Scanner - User Guide

## Table of Contents
1. Installation
2. Basic Usage
3. Scan Modes
4. Understanding Results
5. Troubleshooting

## Installation

### Prerequisites
- Ubuntu 20.04+ (or compatible Linux distribution)
- Python 3.7 or higher
- Git
- 100MB free disk space

### Installation Steps

```bash
sudo apt update
sudo apt install python3-full python3-venv python3-pip python3-tk
git clone https://github.com/Nevera-Hard-Rp/-FiveM-Backdoor-Scanner.git
cd -FiveM-Backdoor-Scanner
python3 -m venv scanner_env
source scanner_env/bin/activate
pip install -r requirements.txt
chmod +x fivem_scanner_cli.py
```

## Basic Usage

```bash
cd /path/to/fivem-backdoor-scanner
source scanner_env/bin/activate
./fivem_scanner_cli.py /path/to/resources
./fivem_scanner_cli.py /path/to/resources --detailed
./fivem_scanner_cli.py /path/to/resources --quick
./fivem_scanner_cli.py /path/to/resources -o scan_report.txt -f txt
```