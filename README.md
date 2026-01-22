# PC Health & Wellness Monitor (PowerShell)

## Overview
A PowerShell-based “PC health and wellness” monitor that collects key system telemetry:
- CPU/GPU temperature (when supported)
- CPU/GPU clock speeds (when supported)
- System uptime (“time alive”)
- A practical bottleneck heuristic using CPU vs GPU utilization

This project is designed for IT infrastructure / troubleshooting workflows: quick checks, repeatable logging, and exportable output (JSON/CSV).

## Technologies Used
- PowerShell 7+ (works in Windows PowerShell 5.1 with minor changes)
- Windows Performance Counters (CPU/GPU utilization)
- CIM/WMI (uptime + baseline hardware info)
- LibreHardwareMonitor (optional, for temperature/clock telemetry)

## Key Features
- One-command snapshot of system health
- Optional loop mode for continuous monitoring
- Exports JSON + CSV logs for troubleshooting
- Bottleneck heuristic: flags likely CPU-bound or GPU-bound conditions
- Graceful fallback if GPU counters or temp sensors aren’t available

## Setup (Quick Start)
### 1) Clone the repo
```bash
git clone https://github.com/<corbinlikescode>/pc-health-welln



