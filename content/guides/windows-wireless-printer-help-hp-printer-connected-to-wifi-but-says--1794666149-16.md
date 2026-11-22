---
title: "HP Printer Connected to Wi-Fi but Says Offline: Clear the Stale Windows 11 Status"
description: "Your HP printer is on Wi-Fi and powered on, but Windows 11 shows it offline. Follow these steps to clear the stale offline status and verify printing."
seo_title: "HP Printer Connected to Wi-Fi but Says Offline: Windows 11 Fix"
seo_description: "Your HP printer is on Wi-Fi and powered on, but Windows 11 shows it offline. Follow these steps to clear the stale offline status and verify printing."
keywords:
  - "hp printer connected to wifi but says offline"
date: 2026-11-22T10:12:46+08:00
publishDate: 2026-11-22T10:12:46+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

Your HP printer is powered on and joined to the same Wi-Fi as your Windows 11 PC, yet the print queue still shows it as offline. This usually means Windows is holding a stale status or the queue is paused, not that the printer has failed. Work through these checks in order.

## Check the Printer's Network Status
On the printer's control panel, open the wireless or network settings and confirm it is connected to your network with a valid IP address. If the IP is missing or shows 0.0.0.0, reconnect the printer to Wi-Fi from its panel, then return to Windows. A valid IP tells you the printer is reachable; a missing one means the connection dropped.

## Clear the Offline Flag in Windows
Open Settings > Bluetooth & devices > Printers & scanners, select your HP printer, and choose Open print queue. In the queue window, click Printer and uncheck Use Printer Offline if it is checked. Then click Printer > Pause Printing to unpause if needed. This clears the manual offline override that Windows sometimes leaves behind.

## Restart the Print Spooler
Press Windows + R, type services.msc, and press Enter. Find Print Spooler, right-click it, and choose Restart. If the queue still shows offline after the service restarts, this is the point where an **hp printer connected to wifi but says offline** status often needs a deeper port check rather than repeated restarts.

## Verification Test
Print a Windows test page from Printers & scanners > your printer > Print test page. If it prints, the offline status is cleared. If it still fails, note the exact error shown in the queue.

## Rollback Note
If you changed the printer's port or IP settings during troubleshooting and printing worsens, return to the previous port configuration before continuing. For guided diagnosis,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).
