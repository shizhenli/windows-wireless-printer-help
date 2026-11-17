---
title: "HP Printer Offline but Connected to Wi-Fi: Reset the Windows 11 Offline Flag"
description: "Your HP printer shows offline in Windows 11 even though it's on Wi-Fi. Follow these steps to reset the offline flag and restore printing."
seo_title: "HP Printer Offline but Connected to Wi-Fi: Windows 11 Fix"
seo_description: "Your HP printer shows offline in Windows 11 even though it's on Wi-Fi. Follow these steps to reset the offline flag and restore printing."
keywords:
  - "hp printer offline but is connected to wifi"
date: 2026-11-17T11:12:17+08:00
publishDate: 2026-11-17T11:12:17+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

You're on Windows 11, your HP printer is powered on and connected to Wi-Fi, yet the queue shows it offline—and you're stuck at the step where Windows marks the printer offline before any controlled diagnosis.

## Check the Printer's Actual Network State

On the printer's control panel, print a network configuration page. Confirm the status says Connected and note the IP address. On your PC, open Settings > Bluetooth & devices > Printers & scanners, select your HP printer, and click Open print queue. In the queue window, click Printer and ensure Use Printer Offline is unchecked. If it was checked, unchecking it is the first real fix—this is often why an **hp printer offline but is connected to wifi** appears stuck.

## Restart the Print Spooler and Reconnect

Press Windows + R, type services.msc, and press Enter. Find Print Spooler, right-click it, and choose Restart. Wait 30 seconds. Back in the printer queue, click Printer > Connect (or Add Printer) and select your HP printer by its IP address if it appears. If the queue still shows offline, remove the printer from Settings > Bluetooth & devices > Printers & scanners, then add it again using Add device. This clears the stale offline flag without touching your Wi-Fi.

## Verification Test

Open Notepad, type a test line, and press Ctrl + P. Select your HP printer and print. The job should leave the queue within 10 seconds and the printer should produce the page. If the queue still says offline, the port is misconfigured—check the port under Printer > Properties > Ports and ensure the standard TCP/IP port matches the printer's IP.

## Rollback Note

If re-adding the printer fails, use System Restore to return to a point before the change, or reinstall the HP driver from the official site. For guided help,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).
