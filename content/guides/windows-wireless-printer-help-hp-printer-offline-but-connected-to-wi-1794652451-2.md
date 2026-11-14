---
title: "HP Printer Offline but Connected to Wi-Fi: Fix the Windows 11 Offline Status"
description: "Step-by-step fix when Windows 11 shows your HP printer offline even though it's powered on and connected to Wi-Fi. Clear the offline status and restore printing."
seo_title: "HP Printer Offline but Connected to Wi-Fi? Windows 11 Fix"
seo_description: "Step-by-step fix when Windows 11 shows your HP printer offline even though it's powered on and connected to Wi-Fi. Clear the offline status and restore printing."
keywords:
  - "hp printer offline but connected to wifi"
date: 2026-11-14T20:01:34+08:00
publishDate: 2026-11-14T20:01:34+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

Your Windows 11 PC shows the HP printer as offline in the queue, even though the printer is powered on and connected to Wi-Fi.

## Check the Printer's Network Status

On the printer's control panel, print a network configuration report. Look for the IP address and connection status. If the IP address is missing or shows 0.0.0.0, the printer has dropped off Wi-Fi. Reconnect it to the same network your PC uses. If the IP is present, note it and move to the next step.

## Verify the Port and Offline Setting

On your PC, open Settings > Bluetooth & devices > Printers & scanners. Select your HP printer, then open Print queue > Printer > Use Printer Offline. If it is checked, uncheck it. Next, open Printer > Properties > Ports. Confirm the checked port matches the printer's current IP address. If it points to a stale IP, click Add Port > Standard TCP/IP Port, enter the correct IP, and select it. This is the most common cause of an **hp printer offline but connected to wifi** status.

## Restart the Print Spooler

Press Windows + R, type services.msc, and press Enter. Find Print Spooler, right-click, and choose Restart. Wait for it to stop and start again. This clears stuck jobs that can hold the offline flag.

## Verification Test

Print a Windows test page from Printer > Properties > General > Print Test Page. If it prints, the offline status is cleared. If it still shows offline, restart both the printer and PC, then repeat the port check.

## Rollback Note

If changing the port breaks printing, return to Ports and reselect the previous port. If you removed a port, re-add it with the original IP. Keep a note of the old settings before editing.

If the queue still marks the printer offline after these checks,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult) for a guided diagnosis.
