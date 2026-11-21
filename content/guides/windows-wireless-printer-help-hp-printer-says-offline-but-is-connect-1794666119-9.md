---
title: "HP Printer Says Offline but Is Connected to Wi-Fi: Fix Windows 11 Offline Status"
description: "Fix the Windows 11 offline status when your HP printer is powered on and connected to Wi-Fi. Follow these checks to get the queue working again."
seo_title: "HP Printer Offline but Connected to Wi-Fi: Windows 11 Fix"
seo_description: "Fix the Windows 11 offline status when your HP printer is powered on and connected to Wi-Fi. Follow these checks to get the queue working again."
keywords:
  - "hp printer says offline but is connected to wifi"
date: 2026-11-21T17:03:14+08:00
publishDate: 2026-11-21T17:03:14+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

Your Windows 11 PC shows the HP printer as offline even though the printer is powered on and connected to Wi-Fi, and you're stuck at the offline status before any controlled diagnosis. Let's walk through this step by step.

## Check the Printer's Network Connection

On the printer's control panel, print a network configuration page. Look for the IP address and connection status. If the IP address is missing or shows 0.0.0.0, the printer has dropped off Wi-Fi even though the light may be on. Reconnect it to the same network your PC uses. If the IP address is present, note it down and move to the next check.

## Verify the Port in Windows 11

Open Settings > Bluetooth & devices > Printers & scanners, select your HP printer, and choose Printer properties. Click the Ports tab. The checked port should match the printer's current IP address. If it points to a WSD port or an old IP, change it to the correct Standard TCP/IP port. This is often why an **hp printer says offline but is connected to wifi** — Windows is still looking at the wrong address.

## Clear the Stuck Queue

Open the print queue and cancel any pending jobs. Then restart the Print Spooler service: press Windows + R, type services.msc, find Print Spooler, and restart it. This clears the offline flag Windows has cached.

## Verification Test

Print a test page from Printer properties. If it prints, the offline status is resolved. If it still shows offline, power-cycle the printer and PC, then repeat the port check.

## Rollback Note

If changing the port breaks printing, return to the previous port setting and restart the spooler. For guided help,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).
