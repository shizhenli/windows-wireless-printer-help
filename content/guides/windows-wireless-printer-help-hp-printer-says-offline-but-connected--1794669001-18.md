---
title: "HP Printer Says Offline but Connected to Wi-Fi: Fix the Windows 11 Offline Status"
description: "Fix the HP printer offline status on Windows 11 when the printer is powered on and connected to Wi-Fi. Step-by-step checks for the print queue, port, and spooler."
seo_title: "HP Printer Offline but Connected to Wi-Fi: Windows 11 Fix"
seo_description: "Fix the HP printer offline status on Windows 11 when the printer is powered on and connected to Wi-Fi. Step-by-step checks for the print queue, port, and spooler."
keywords:
  - "hp printer says offline but connected to wifi"
date: 2026-11-28T22:03:11+08:00
publishDate: 2026-11-28T22:03:11+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

Your Windows 11 PC shows the HP printer as offline even though the printer is powered on and connected to Wi-Fi, and you want to clear that status before trying anything drastic.

## Check the Queue and Port

Open Settings > Bluetooth & devices > Printers & scanners, select your HP printer, and choose Open print queue. If the queue window says Offline, click Printer in the menu bar and make sure Use Printer Offline is unchecked. Next, go back to the printer's properties and open the Ports tab. Confirm the checked port matches your printer's current connection, usually a WSD or TCP/IP entry with the printer's IP address. If the port shows a stale IP, select the correct one or add a new TCP/IP port using the address printed on the printer's network configuration page.

## Restart the Print Spooler

Press Windows + R, type services.msc, and press Enter. Find Print Spooler, right-click it, and choose Restart. This clears a stuck queue state that can make windows marks the printer offline persist. After the service restarts, reopen the queue and check the status line.

## Verification Test

Print a Windows test page from Printer properties > General > Print Test Page. If it prints, the offline flag is cleared. If the queue still shows offline, note the exact error and port name before changing anything else.

## Rollback Note

If you added a new port, you can revert by reselecting the original port in the Ports tab. If the spooler restart causes issues, restart the service again. When the **hp printer says offline but connected to wifi** despite these checks, stop resetting and get a targeted diagnosis:

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).
