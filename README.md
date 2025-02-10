# 🔍 Process Memory & CPU Watcher
## 📝 Description
A lightweight bash script that provides real-time monitoring of memory (PSS) and CPU usage for specific processes. It features automatic process detection from active windows and continuous updates. 🔄

## ✨ Features
🖥️ Real-time memory and CPU monitoring
🎯 Automatic active window process detection
📊 Memory usage in appropriate units (Ki, Mi, Gi)
💻 CPU usage percentage display
🔄 Auto-refresh every second
🎨 Clean, columnar output format

## 🚀 Usage

```bash
# Monitor active window
./pss_xprop
```
## ⚙️ Prerequisites

Linux system
xprop utility
smem utility
sudo privileges

## 🛠️ Configuration
Customize monitored applications in the appcust array:
```bash
appcust=("chrome" "discord" "python" "i3" "gvfs" "systemd" "at-spi" "vim")
```

📂 Cache Location : ~/.cache/pss_usage/

## ⚠️ Notes
Requires sudo password for smem
Memory percentage based on 8GB total RAM (configurable)
Auto-detects common applications via window title
