---
title: "Windows 11 Printer Offline When Powered On: Clear the Offline Flag"
description: "Your wireless printer is on, yet Windows 11 marks it offline. Diagnose the queue state, clear the stale offline flag, and verify printing without a full reset."
seo_title: "Windows 11 Printer Offline but Powered On? Fix the Queue Flag"
seo_description: "Your wireless printer is on, yet Windows 11 marks it offline. Diagnose the queue state, clear the stale offline flag, and verify printing without a full reset."
keywords:
  - "windows 11 printer offline"
date: 2026-11-21T16:57:11+08:00
publishDate: 2026-11-21T16:57:11+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

## Troubleshooting

Your Windows 11 PC shows the wireless printer as offline even though the printer is powered on and connected to Wi-Fi. The queue is stuck at the offline status, and you want to clear that flag before doing anything drastic. Start by opening Settings > Bluetooth & devices > Printers & scanners, selecting the printer, and choosing Open print queue. In the queue window, look at the status line under the printer name. If it says Offline, click Printer in the menu bar and confirm Use Printer Offline is unchecked. If it is checked, uncheck it; that single toggle often clears the stale flag. Next, look at the queue itself. If jobs are listed as Error or Paused, cancel them all, then restart the Print Spooler service: press Windows+R, type services.msc, find Print Spooler, right-click, and choose Restart. Return to the queue and check the status again. If it still reads Offline, open the printer's own control panel or web interface and confirm its IP address has not changed; a mismatch between the port and the printer's current address will keep Windows marking it offline. To verify, print a one-page test document from Notepad. If it prints, the flag is cleared. If it still fails, roll back by re-enabling Use Printer Offline so the queue does not spin on failed jobs, then note the exact status text before trying anything else. For a controlled diagnosis of this **windows 11 printer offline** state,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).

Repeat the same check after a restart and confirm the result twice.
