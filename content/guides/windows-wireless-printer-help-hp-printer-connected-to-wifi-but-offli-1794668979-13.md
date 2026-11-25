---
title: "HP Printer Connected to Wi-Fi but Offline on Windows 11: Fix the Offline Status"
description: "Your HP printer shows offline in Windows 11 even though it's powered on and connected to Wi-Fi. Follow these steps to diagnose and restore the online status."
seo_title: "HP Printer Connected to Wi-Fi but Offline on Windows 11? Fix It"
seo_description: "Your HP printer shows offline in Windows 11 even though it's powered on and connected to Wi-Fi. Follow these steps to diagnose and restore the online status."
keywords:
  - "hp printer connected to wifi but offline"
date: 2026-11-25T11:12:38+08:00
publishDate: 2026-11-25T11:12:38+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

You see your HP printer marked offline in Windows 11, even though it's powered on and connected to Wi-Fi. Let's walk through a controlled diagnosis to get it back online.

## Check the Printer's Network Connection

First, confirm the printer is actually on the same network as your PC. On the printer's control panel, print a network configuration page (usually under Settings > Network > Print Network Configuration). Look for the IP address and network name (SSID). On your PC, open Settings > Network & Internet > Wi-Fi and verify the SSID matches. If they differ, reconnect the printer to the correct network. If the IP address starts with 169.254, the printer didn't get a valid address—restart your router and printer.

## Verify the Queue and Port

Open Settings > Bluetooth & devices > Printers & scanners. Select your HP printer and click Open print queue. If it shows offline, click Printer > Use Printer Online (if available). Then go to Printer > Properties > Ports. Ensure the port with the printer's current IP address is checked. If the IP changed, click Add Port > Standard TCP/IP Port and enter the new IP. This is a common fix for an **hp printer connected to wifi but offline**.

## Restart the Print Spooler

Press Windows + R, type services.msc, and press Enter. Find Print Spooler, right-click, and select Restart. This clears stuck jobs that can cause the offline status.

## Verification Test

Print a test page from the printer's properties. If it prints, the status should change to online. If not, check the queue for errors.

## Rollback Note

If changes don't help, note your original port settings and revert them. For further diagnosis,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).
