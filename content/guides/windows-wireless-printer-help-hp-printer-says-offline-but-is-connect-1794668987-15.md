---
title: "HP Printer Says Offline but Is Connected to Wi-Fi: Diagnose the Windows 11 Offline Status"
description: "Your HP printer shows offline in Windows 11 even though it's on Wi-Fi. Follow these targeted checks to diagnose the queue state and restore printing."
seo_title: "HP Printer Offline on Windows 11? Fix It While Connected to Wi-Fi"
seo_description: "Your HP printer shows offline in Windows 11 even though it's on Wi-Fi. Follow these targeted checks to diagnose the queue state and restore printing."
keywords:
  - "hp printer says offline but is connected to wifi"
date: 2026-11-26T08:11:00+08:00
publishDate: 2026-11-26T08:11:00+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

**hp printer says offline but is connected to wifi**. You're on Windows 11, your HP printer is powered on and connected to Wi-Fi, yet the print queue shows it as offline. Let's diagnose why Windows marks the printer offline before you reset anything.

## Check the Printer's Actual Network Status

First, confirm the printer is truly on the same network as your PC. On the printer's control panel, print a network configuration page. Look for the IP address and compare its subnet to your PC's. On Windows 11, open Settings > Network & internet > Wi-Fi and check the IPv4 address. If the subnets differ (e.g., 192.168.1.x vs. 192.168.2.x), the printer is on a different network segment, which causes the offline status. Reconnect the printer to the correct SSID.

## Verify the Windows Queue and Port

Open Settings > Bluetooth & devices > Printers & scanners. Select your HP printer and click Open print queue. If it says offline, click Printer > Use Printer Offline to toggle it off. Then go to Printer > Properties > Ports. Ensure the checked port matches the printer's current IP address. If it shows a WSD port or an old IP, create a new Standard TCP/IP port with the correct IP. This directly addresses why windows marks the printer offline.

## Restart the Print Spooler

Press Win+R, type services.msc, and find Print Spooler. Right-click and restart it. This clears stale queue states that can falsely flag the printer as offline.

## Verification Test

Print a test page from the printer's properties. If it prints, the offline status is resolved. If not, check the queue again—if it still shows offline, the port or network segment is still mismatched.

## Rollback Note

If changes worsen the issue, use System Restore to revert to a previous point before adjusting ports or spooler settings.

Still stuck?

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult) for a guided diagnosis.
