# Sentinel Pulse

Offline Windows desktop monitor for unusual network and process activity on the machine it is installed on.

## Problem

A lightweight local signal was needed: is this PC busier or noisier than its own normal, without sending that activity to a cloud service or opening a listen port.

## What I built

- Always-on-top widget with sparklines for network intensity and process churn
- Compact bar and system-tray modes
- Green, yellow, and red status with hysteresis so it does not flicker
- First-run baseline learned on that host
- On-device scoring from the baseline plus simple heuristics
- Optional local response: end a process, add a firewall outbound rule, remember a block
- Self-contained .NET 8 build so end users do not install a runtime
- Update check only when the user asks, over outbound HTTPS, then the session closes

It is not antivirus.

## Stack

C#, .NET 8, WPF, Windows.

## Status

Private desktop tool. This page does not include detection rules or data paths.
