---
title: "HP Printer Connected to Wi-Fi but Offline on Windows 10: Fix the Offline Status"
description: "Fix an HP printer that shows offline in Windows 10 despite being powered on and connected to Wi-Fi. Follow these targeted steps to restore the correct status."
seo_title: "HP Printer Connected to Wi-Fi but Offline Windows 10 Fix"
seo_description: "Fix an HP printer that shows offline in Windows 10 despite being powered on and connected to Wi-Fi. Follow these targeted steps to restore the correct status."
keywords:
  - "hp printer connected to wifi but offline windows 10"
date: 2026-11-17T08:21:36+08:00
publishDate: 2026-11-17T08:21:36+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

Your HP printer is powered on and connected to Wi-Fi, but Windows 10 still marks it offline in the queue. This guide fixes that specific mismatch.

## Check the Printer's Actual Network Status

On the printer's control panel, print a network configuration page. Verify the IP address is present and the status says Connected or Ready. If the IP is missing or shows 0.0.0.0, the printer lost its Wi-Fi link—reconnect it before continuing. If the IP is valid, note it and move to the next check.

## Verify the Windows Port Matches the Printer's IP

Open Settings > Devices > Printers & scanners. Select your HP printer, click Manage, then Printer properties > Ports. Look for a Standard TCP/IP port with the same IP you noted. If the port uses a different IP (common after a router restart), click Add Port > Standard TCP/IP Port, enter the correct IP, and assign it. This alone often resolves the **hp printer connected to wifi but offline windows 10** status.

## Clear the Stuck Queue

Open Services (services.msc), stop Print Spooler. Navigate to C:\Windows\System32\spool\PRINTERS and delete all files. Start Print Spooler again. This removes any job holding the offline flag.

## Verification Test

Print a Windows test page from Printer properties > General > Print Test Page. The queue should show the job as Printing, then disappear. If the status still reads Offline, restart the printer and PC once, then repeat the port check.

## Rollback Note

If you changed the port and printing fails, return to Ports and reselect the original port. Your previous configuration remains listed.

Still stuck?

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult) and we'll diagnose the remaining cause.
