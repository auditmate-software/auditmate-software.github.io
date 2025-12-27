# AuditMate System Audit Tool

AuditMate is a lightweight, automated system auditing tool designed for Linux environments. It collects system information, monitors changes, and helps administrators maintain secure and updated systems. This page documents the tool's features, usage, and setup instructions.

---

## Features

### 1. System Scan
- Collects core system information:
  - Hostname
  - Operating System
  - Kernel version
  - Uptime
- Lists all users and identifies administrators
- Detects running services, installed packages, and open ports
- Checks firewall status and pending system updates

### 2. Baseline Management
- Saves the system state to a JSON file (`baseline.json`)
- Compares the current state to the saved baseline
- Outputs any detected changes in a human-readable format
- Critical warnings trigger a non-zero exit code for automated scripts

### 3. Warning System
- Detects important security or configuration issues:
  - Multiple admin accounts
  - Open SSH port 22
  - Inactive or disabled firewall
  - Pending system updates
- Warnings are categorized as critical or non-critical

### 4. Paid Features
- Export system report to JSON format
- Requires activation using a license key
- License management ensures access to premium features

### 5. License Management
- Activate license via:  
  ```bash
  ./auditmate license activate mylicense.json
