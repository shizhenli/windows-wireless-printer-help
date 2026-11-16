---
title: "My HP Printer Is Offline but Connected to Wi-Fi: Fix the Windows 11 Offline Status"
description: "Step-by-step fix when your HP printer shows offline in Windows 11 despite being connected to Wi-Fi. Diagnose the queue, restart the spooler, and verify printing."
seo_title: "HP Printer Offline but Connected to Wi-Fi on Windows 11"
seo_description: "Step-by-step fix when your HP printer shows offline in Windows 11 despite being connected to Wi-Fi. Diagnose the queue, restart the spooler, and verify printing."
keywords:
  - "my hp printer is offline but connected to wifi"
date: 2026-11-16T09:12:12+08:00
publishDate: 2026-11-16T09:12:12+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

You see the printer listed as offline in Windows 11 even though it is powered on and connected to Wi-Fi. This usually means Windows has lost the active session with the printer, not that the printer is broken. Follow these steps to diagnose and restore the online status.

## Check the Printer's Network Status

On the printer's control panel, print a network configuration page. Confirm the IP address is present and the connection status says Connected or Ready. If the IP is missing or shows 0.0.0.0, reconnect the printer to Wi-Fi first. If the IP is present, note it for the next step.

## Verify the Port in Windows

Open Settings > Bluetooth & devices > Printers & scanners. Select your HP printer, then Printer properties > Ports. The checked port should be a Standard TCP/IP port matching the printer's IP. If it points to a WSD port or an old IP, change it to the correct TCP/IP port. Click Apply.

## Restart the Print Spooler

Press Windows + R, type services.msc, and press Enter. Find Print Spooler, right-click, and choose Restart. This clears stuck jobs that can hold the queue offline. If the spooler stops immediately, a corrupted job is likely; clear the queue from C:\Windows\System32\spool\PRINTERS after stopping the service.

## Verification Test

Open Notepad, type a test line, and press Ctrl + P. Select your HP printer and print. The status should change from offline to ready, and the page should print within 30 seconds. If it still shows offline, the port or driver needs attention.

## Rollback Note

If changing the port or restarting the spooler causes new errors, revert the port to its previous setting and restart the spooler again. Your original configuration will be restored.

If **my hp printer is offline but connected to wifi** persists after these checks, the driver may need reinstalling.

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult) for a guided diagnosis.
