---
title: "HP Printer Offline on Windows 11: Clear the Stale Queue Status"
description: "Your HP printer is powered on and on Wi-Fi, yet Windows 11 shows it offline. Diagnose the queue state, refresh the port, and verify printing without a full reset."
seo_title: "HP Printer Shows Offline but Is Connected to Wi-Fi: Fix Windows 11 Queue"
seo_description: "Your HP printer is powered on and on Wi-Fi, yet Windows 11 shows it offline. Diagnose the queue state, refresh the port, and verify printing without a full reset."
keywords:
  - "hp printer shows offline but is connected to wifi"
date: 2026-11-26T09:10:53+08:00
publishDate: 2026-11-26T09:10:53+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

## Troubleshooting

Your Windows 11 PC shows your HP printer as offline even though the printer is powered on and connected to Wi-Fi. Before resetting anything, check whether Windows is holding a stale queue state. Open Settings > Bluetooth & devices > Printers & scanners, select the HP printer, and choose Open print queue. If the queue window says Offline, note whether any jobs are listed. A queue with stuck jobs can keep the offline flag even when the printer is reachable. Cancel all jobs, then close the queue. Next, return to Printers & scanners and open Printer properties > Ports. Confirm the checked port matches the printer's current connection, usually a WSD or TCP/IP port. If you see multiple entries for the same HP model, select the one that responds, then Apply. This is the point where many users assume the **hp printer shows offline but is connected to wifi** and reset the printer unnecessarily; the queue state is often the real cause. To verify, print a Windows test page from Printer properties > General. If it prints, the offline status was stale and the queue is clear. If it still fails, open the queue again and check whether the status changes to Ready. If not, restart the Print Spooler service once: services.msc > Print Spooler > Restart. As a recovery note, if you changed the port and printing fails, return to Ports and recheck the original port before making further changes. For a controlled diagnosis of your exact queue state,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).

Repeat the same check after a restart and confirm the result twice.
