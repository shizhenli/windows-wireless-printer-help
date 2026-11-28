---
title: "HP Printer Connected to Wi-Fi but Offline on Windows 10: Clear the Offline Status"
description: "Your HP printer is on Wi-Fi but Windows 10 shows it offline. Follow these targeted checks to clear the offline status and restore printing."
seo_title: "HP Printer Connected to Wi-Fi but Offline on Windows 10 — Fix It"
seo_description: "Your HP printer is on Wi-Fi but Windows 10 shows it offline. Follow these targeted checks to clear the offline status and restore printing."
keywords:
  - "hp printer connected to wifi but offline windows 10"
date: 2026-11-28T22:30:52+08:00
publishDate: 2026-11-28T22:30:52+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

Your HP printer is powered on and joined to Wi-Fi, yet the Windows 10 queue still lists it as offline, and you want to clear that status without a full reset.  

## Check the Printer's Network State First
On the printer's control panel, open the wireless summary and confirm the IP address and signal strength. If the IP is missing or shows 0.0.0.0, the printer has dropped off the network even though it is powered on. Rejoin the Wi-Fi from the panel, then return to Windows. If the IP is present, note it; you will compare it with the port in the next step.

## Compare the Port with the Printer's IP
Open Settings > Devices > Printers & scanners, select your HP printer, and choose Manage > Printer properties > Ports. If the checked port is a WSD entry or an IP that differs from the printer's current address, the queue is pointing at a stale address. Add a Standard TCP/IP port using the printer's current IP, apply it, and clear the queue. This is the most common cause of an **hp printer connected to wifi but offline windows 10** status.

## Verification Test
Print a Windows test page from Printer properties > General. If it prints, the offline mark should clear within a minute. If the queue still shows offline, open Services, restart Print Spooler, and retry once.

## Rollback Note
If the new TCP/IP port does not print, switch the port back to the previous entry before making further changes, so you keep a known state. For guided diagnosis,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).
