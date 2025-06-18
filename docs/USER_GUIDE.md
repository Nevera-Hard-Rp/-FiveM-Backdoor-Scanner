# 📚 FiveM Backdoor Scanner - User Guide

## Table of Contents
1. [Installation](#installation)
2. [Basic Usage](#basic-usage)
3. [Scan Modes](#scan-modes)
4. [Understanding Results](#understanding-results)
5. [Troubleshooting](#troubleshooting)

## Installation

### Prerequisites
- Ubuntu 20.04+ (or compatible Linux distribution)
- Python 3.7 or higher
- Git
- 100MB free disk space

### Detailed Installation Steps

```bash
# 1. Update system
sudo apt update
sudo apt install python3-full python3-venv python3-pip python3-tk

# 2. Clone repository
git clone https://github.com/yourusername/fivem-backdoor-scanner.git
cd fivem-backdoor-scanner

# 3. Create virtual environment
python3 -m venv scanner_env

# 4. Activate virtual environment
source scanner_env/bin/activate

# 5. Install dependencies
pip install requests

# 6. Make scanner executable
chmod +x fivem_scanner_cli.py
