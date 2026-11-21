---
title: "HP Printer Connected to Wi-Fi but Offline: Fix the Windows 11 Offline Status"
description: "Your HP printer shows offline in Windows 11 even though it's powered on and connected to Wi-Fi. Follow these steps to diagnose and restore the online status."
seo_title: "HP Printer Connected to Wi-Fi but Offline? Windows 11 Fix"
seo_description: "Your HP printer shows offline in Windows 11 even though it's powered on and connected to Wi-Fi. Follow these steps to diagnose and restore the online status."
keywords:
  - "hp printer connected to wifi but offline"
date: 2026-11-21T17:00:15+08:00
publishDate: 2026-11-21T17:00:15+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

You're on Windows 11, your HP printer is powered on and linked to Wi-Fi, yet the print queue stubbornly shows it as offline. This guide walks you through a controlled diagnosis to get Windows to recognize the printer as online again.

## Check the Printer's Actual Network Status

First, confirm the printer is truly on the same network as your PC. On the printer's control panel, print a network configuration page (usually under Settings > Network > Print Network Configuration). Look for the IP address and network name (SSID). On your PC, open Settings > Network & Internet > Wi-Fi and compare the SSID. If they differ, reconnect the printer to the correct network. If the IP address starts with 169.254, the printer didn't get a valid DHCP lease—restart your router and printer, then recheck.

## Verify the Windows Queue and Port

Open Settings > Bluetooth & devices > Printers & scanners. Select your HP printer and click Open print queue. If it says offline, click Printer > Use Printer Online (if available). Then go to Printer > Properties > Ports. Ensure the checked port matches the printer's current IP address (Standard TCP/IP port). If the IP changed, click Add Port > Standard TCP/IP Port and enter the new IP. This resolves many cases of an **hp printer connected to wifi but offline** due to a stale port.

## Restart the Print Spooler

Press Windows + R, type services.msc, and press Enter. Find Print Spooler, right-click, and choose Restart. This clears stuck jobs that can force an offline state.

## Verification Test

Print a test page from the printer's properties (right-click printer > Printer properties > Print Test Page). If it prints, the status should change to online. If not, check the queue for errors.

## Rollback Note

If changes don't help, revert the port to its previous setting or use System Restore to undo recent driver updates. For personalized help,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).
