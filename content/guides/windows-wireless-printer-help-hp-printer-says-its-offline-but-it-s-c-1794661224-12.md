---
title: "HP Printer Offline on Wi-Fi? Check the Windows 11 Queue State First"
description: "Your HP printer says it's offline but connected to Wi-Fi. Diagnose the Windows 11 queue state before resetting anything, then verify printing works."
seo_title: "HP Printer Offline but Connected to Wi-Fi: Windows 11 Queue Fix"
seo_description: "Your HP printer says it's offline but connected to Wi-Fi. Diagnose the Windows 11 queue state before resetting anything, then verify printing works."
keywords:
  - "hp printer says its offline but it's connected to wifi"
date: 2026-11-17T12:12:18+08:00
publishDate: 2026-11-17T12:12:18+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

Your HP printer is powered on and joined to Wi-Fi, yet Windows 11 shows it offline in the queue. Before you reset the printer or reinstall drivers, confirm whether Windows is holding a stale queue state.

## Check the queue state first

Open Settings > Bluetooth & devices > Printers & scanners, select your HP printer, then choose Open print queue. If the queue window shows the printer as offline while jobs are listed, note whether jobs are stuck in "Paused" or "Error." That tells you Windows is not refreshing the device status, not that the printer lost Wi-Fi.

## Clear the stale queue

In the queue window, click Printer and clear any check next to "Use Printer Offline." Then cancel all pending jobs. If jobs will not cancel, stop the Print Spooler service in Services, delete the files in C:\Windows\System32\spool\PRINTERS, and restart the service. This is a safe rollback point: if printing worsens, restarting the spooler restores the previous state.

## Reconnect the port

Return to Printers & scanners, open the printer's properties, and check the Ports tab. The selected port should match your printer's Wi-Fi connection, typically a WSD or TCP/IP port. If the port shows a stale address, run Add Printer again and let Windows rediscover the device. This is the step that resolves most cases where the **hp printer says its offline but it's connected to wifi**.

## Verification test

Print a one-page test from Notepad. If the queue status changes to "Printing" and the page emerges, the offline flag is cleared. If it still shows offline, the printer's Wi-Fi address may have changed; confirm the IP in the printer's network settings matches the port.

If the queue still refuses to clear,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult) before making deeper changes.
