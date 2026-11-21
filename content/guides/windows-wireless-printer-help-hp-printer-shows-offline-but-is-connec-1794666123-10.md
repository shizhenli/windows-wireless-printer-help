---
title: "HP Printer Shows Offline but Is Connected to Wi-Fi: Fix Windows 11 Offline Status"
description: "Your HP printer shows offline in Windows 11 even though it's on Wi-Fi. Follow these technician steps to diagnose the queue and restore printing."
seo_title: "HP Printer Offline on Windows 11? Fix It While Connected to Wi-Fi"
seo_description: "Your HP printer shows offline in Windows 11 even though it's on Wi-Fi. Follow these technician steps to diagnose the queue and restore printing."
keywords:
  - "hp printer shows offline but is connected to wifi"
date: 2026-11-21T17:03:14+08:00
publishDate: 2026-11-21T17:03:14+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

You're on Windows 11, your HP printer is powered on and connected to Wi-Fi, but the queue still shows it as offline.

## Check the Printer's Actual Network State
First, confirm the printer is truly on the network. On the printer's control panel, print a network configuration page. Look for the IP address and connection status. If the IP is 0.0.0.0 or the status says disconnected, the printer dropped Wi-Fi—reconnect it via the wireless setup wizard. If the IP is valid (e.g., 192.168.1.50), note it and move on.

## Verify Windows Sees the Same IP
On your PC, open Settings > Bluetooth & devices > Printers & scanners. Select your HP printer, then Printer properties > Ports. The checked port should match the printer's IP. If it points to a WSD port or a different IP, that mismatch is why **hp printer shows offline but is connected to wifi**. Click Add Port > Standard TCP/IP Port, enter the printer's current IP, and apply. This forces Windows to talk to the right address.

## Clear the Stale Queue
Open Services (services.msc), stop Print Spooler, delete the files in C:\Windows\System32\spool\PRINTERS, then restart Print Spooler. This removes any stuck job that keeps the offline flag active.

## Verification Test
Print a Windows test page from Printer properties > General > Print Test Page. If it prints, the offline status clears. If it still fails, check the printer's IP again—it may have changed after a router reboot.

## Rollback Note
If the new TCP/IP port doesn't work, return to Ports and re-check the original port. You can also remove and re-add the printer, but note the old queue settings first.

Still stuck?

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).
