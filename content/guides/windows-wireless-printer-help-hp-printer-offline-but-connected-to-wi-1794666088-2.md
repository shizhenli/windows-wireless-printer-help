---
title: "HP Printer Offline but Connected to Wi-Fi: Diagnose the Windows 11 Offline Status"
description: "Your HP printer shows offline in Windows 11 even though it's on and connected to Wi-Fi. Follow these steps to diagnose the queue state and restore printing."
seo_title: "HP Printer Offline but Connected to Wi-Fi? Fix Windows 11 Offline Status"
seo_description: "Your HP printer shows offline in Windows 11 even though it's on and connected to Wi-Fi. Follow these steps to diagnose the queue state and restore printing."
keywords:
  - "hp printer offline but connected to wifi"
date: 2026-11-21T16:57:11+08:00
publishDate: 2026-11-21T16:57:11+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

Your Windows 11 PC shows your HP printer as offline in the queue, even though the printer is powered on and connected to Wi-Fi. This is a common frustration, but it usually points to a communication issue between Windows and the printer, not a hardware failure. Let's walk through a controlled diagnosis.

## Check the Printer's Network Status

First, confirm the printer is actually on the network. On the printer's control panel, print a network configuration page. Look for the IP address and connection status. If the IP address is blank or shows "Not Connected," the printer has dropped off Wi-Fi. Reconnect it to the correct network. If the IP address is present, note it down—you'll need it later.

## Verify the Windows Queue State

On your PC, go to Settings > Bluetooth & devices > Printers & scanners. Select your HP printer and click Open print queue. If the queue shows "Offline," right-click the printer and ensure "Use Printer Offline" is unchecked. Then, click "See what's printing" and cancel any stuck jobs. A stuck job can force the printer into an offline state.

## Test Communication with the Printer

Open Command Prompt and type `ping [printer IP address]` (replace with the IP you noted). If you get replies, the network path is clear. If you get "Request timed out," the printer isn't reachable—check your router or printer's Wi-Fi settings. Next, go back to Printers & scanners, select your printer, and click "Print a test page." If it prints, the issue is resolved. If not, proceed to the next step.

## Reset the Print Spooler

Press Windows + R, type `services.msc`, and press Enter. Find "Print Spooler," right-click, and select Restart. Wait a moment, then try printing again. This clears temporary communication glitches.

## Rollback Note

If these steps don't resolve the **hp printer offline but connected to wifi** status, avoid deleting the printer until you've noted its IP address and driver version. You can then remove and re-add it using the original IP. For personalized assistance,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).
