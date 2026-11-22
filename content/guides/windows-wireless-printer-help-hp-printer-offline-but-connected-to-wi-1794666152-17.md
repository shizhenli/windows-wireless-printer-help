---
title: "HP Printer Offline on Windows 11: Fix the Status When Wi-Fi Is Connected"
description: "Windows 11 shows your HP printer offline even though it's on Wi-Fi. Follow these checks to diagnose the queue status and restore printing."
seo_title: "HP Printer Offline but Connected to Wi-Fi Mac: Windows 11 Fix"
seo_description: "Windows 11 shows your HP printer offline even though it's on Wi-Fi. Follow these checks to diagnose the queue status and restore printing."
keywords:
  - "hp printer offline but connected to wifi mac"
date: 2026-11-22T11:12:53+08:00
publishDate: 2026-11-22T11:12:53+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

Your Windows 11 PC shows the HP printer as offline even though it's powered on and connected to Wi-Fi, and you're stuck at the step where Windows marks the printer offline. Let's diagnose this without resetting everything.

## Check the Printer's Actual Network Status

On the printer's control panel, print a network configuration page. Look for the IP address and connection status. If it shows a valid IP and "Connected," the printer is on the network. If the IP is 169.254.x.x or blank, the printer lost its Wi-Fi link—reconnect it before continuing.

## Verify the Windows Queue and Port

On your PC, open Settings > Bluetooth & devices > Printers & scanners. Select your HP printer and click Open print queue. If the queue shows "Offline," click Printer > Use Printer Offline to toggle it off. Then check the port: right-click the printer > Printer properties > Ports. Ensure the checked port matches the printer's current IP (a Standard TCP/IP port). If it points to a WSD port, switch to the TCP/IP port. This is a common cause of the **hp printer offline but connected to wifi mac** status.

## Restart the Print Spooler

Press Windows + R, type services.msc, and press Enter. Find Print Spooler, right-click, and choose Restart. This clears stuck jobs that can hold the offline flag.

## Verification Test

Print a test page from Printer properties > General > Print Test Page. If it prints, the status should now show "Ready." If it still shows offline, note the exact error.

## Rollback Note

If changing the port breaks printing, return to the previous port setting and restart the spooler again.

If these steps don't resolve it,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult) for a guided diagnosis.
