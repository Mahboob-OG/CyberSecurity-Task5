# 🛠️ Wireshark Setup and Capture Guide

## 📥 Installation Steps
1. Download Wireshark from [wireshark.org](https://www.wireshark.org/)
2. Run the installer with default settings
3. Install WinPcap/Npcap when prompted (required for packet capture)
4. Launch Wireshark after installation

## 🔍 Capture Process

### Step 1: Select Network Interface
- Open Wireshark
- Identify your active network interface (Wi-Fi or Ethernet)
- Look for the interface with fluctuating packet counts
- Double-click to start capturing on that interface

### Step 2: Generate Traffic
While capturing, generate network traffic by:
- Opening a web browser and visiting websites
- Running ping commands in Command Prompt:
  ```cmd
  ping google.com
  ping 8.8.8.8
