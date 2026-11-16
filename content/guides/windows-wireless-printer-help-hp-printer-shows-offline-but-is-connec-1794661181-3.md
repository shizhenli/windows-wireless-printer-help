---
title: "HP Printer Shows Offline but Is Connected to Wi-Fi: Fix the Windows 11 Offline Status"
description: "Fix the Windows 11 offline status when your HP printer is powered on and connected to Wi-Fi. Step-by-step checks, verification, and rollback."
seo_title: "HP Printer Offline but Connected to Wi-Fi: Windows 11 Fix"
seo_description: "Fix the Windows 11 offline status when your HP printer is powered on and connected to Wi-Fi. Step-by-step checks, verification, and rollback."
keywords:
  - "hp printer shows offline but is connected to wifi"
date: 2026-11-16T08:12:13+08:00
publishDate: 2026-11-16T08:12:13+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

## Troubleshooting

You see the queue report your printer offline even though it is powered on and joined to Wi-Fi, and Windows 11 has not completed a controlled diagnosis. Start by confirming the printer's own network state: on the printer control panel, print a network configuration page and check that the IP address is present and the link is active. If the page shows no IP address, the printer is not truly on Wi-Fi; reconnect it before touching Windows. Next, on the PC, open Settings > Bluetooth & devices > Printers & scanners, select the HP printer, and open Print queue. If the queue shows "Offline" with pending jobs, clear those jobs first, because a stuck job can hold the offline flag. Then open Printer properties > Ports and confirm the selected port matches the printer's current IP address. If it points to an old address or a WSD entry, change it to the correct Standard TCP/IP port. This is the point where an **hp printer shows offline but is connected to wifi** condition usually resolves, because Windows is now looking at the right address. Verification test: print a one-page test page from Printer properties > General > Print Test Page. If it prints and the queue status returns to Ready, the fix holds. Rollback note: if the test page fails, return the port to its previous selection and restart the Print Spooler service so you do not leave the queue in a worse state. If the offline flag persists after these checks, stop resetting and

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult) so the queue state can be diagnosed properly.
