---
title: "HP Printer Says Offline but Connected to Wi-Fi: Fix Windows 11 Offline Status"
description: "HP printer says offline but connected to Wi-Fi on Windows 11? Diagnose the queue state and restore the expected offline status with this step-by-step fix."
seo_title: "HP Printer Offline but Connected to Wi-Fi: Windows 11 Fix"
seo_description: "HP printer says offline but connected to Wi-Fi on Windows 11? Diagnose the queue state and restore the expected offline status with this step-by-step fix."
keywords:
  - "hp printer says offline but connected to wifi"
date: 2026-11-16T10:12:15+08:00
publishDate: 2026-11-16T10:12:15+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

Your HP printer is powered on and shows a solid Wi-Fi light, yet Windows 11 displays it as offline in the queue. This is a common status mismatch, not necessarily a hardware failure. Let's diagnose it in a controlled way before changing anything.

## Check the Queue and Port

Open Settings > Bluetooth & devices > Printers & scanners, select your HP printer, and click Open print queue. If the queue shows "Offline" with zero pending jobs, the status is stale. Next, click Printer > Properties > Ports. Note which port is checked. If it is a WSD port, Windows may have lost the device's network identity. If it is a standard TCP/IP port, confirm the IP address matches the printer's current IP (print a network configuration page from the printer's control panel). A mismatch means the port is pointing to an old address.

## Restart the Print Spooler

Press Win+R, type services.msc, and press Enter. Find Print Spooler, right-click, and choose Restart. This clears the stale offline flag without deleting your driver. If the queue still shows offline, return to Ports and switch to the correct TCP/IP port, then apply.

## Verification Test

Print a Windows test page from Printer > Properties > Print Test Page. If it prints, the offline status is resolved. If the queue still reads offline after a successful test page, the status display is lagging; restart the spooler once more and reopen the queue.

## Rollback Note

If switching ports causes new errors, return to the original port selection and restart the spooler. Your driver and queue remain intact.

If the **hp printer says offline but connected to wifi** persists after these checks, the port or driver association may need deeper review.

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult) before resetting the printer.
