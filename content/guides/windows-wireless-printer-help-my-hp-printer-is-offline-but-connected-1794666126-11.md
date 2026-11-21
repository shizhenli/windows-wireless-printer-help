---
title: "HP Printer Offline on Windows 11: Fix the Offline Status When Wi-Fi Is Connected"
description: "Your HP printer shows offline in Windows 11 even though it's on Wi-Fi. Follow these steps to diagnose the queue and restore printing."
seo_title: "HP Printer Offline but Connected to Wi-Fi on Windows 11? Fix It"
seo_description: "Your HP printer shows offline in Windows 11 even though it's on Wi-Fi. Follow these steps to diagnose the queue and restore printing."
keywords:
  - "my hp printer is offline but connected to wifi"
date: 2026-11-21T17:03:14+08:00
publishDate: 2026-11-21T17:03:14+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

You see your HP printer listed as offline in Windows 11, but the printer is powered on and connected to Wi-Fi. This guide helps you diagnose the queue state before resetting anything.

## Check the Printer's Actual Connection

First, confirm the printer is truly on the network. Print a network configuration page from the printer's control panel (usually under Settings > Network or Wireless). Look for the IP address and connection status. If the page shows a valid IP address and "Connected," the printer is on Wi-Fi. If not, reconnect it to Wi-Fi first.

## Verify the Windows Queue State

On your PC, open Settings > Bluetooth & devices > Printers & scanners. Select your HP printer and click Open print queue. If the queue window shows "Offline" or "Use Printer Offline" is checked, the queue is stuck. Uncheck "Use Printer Offline" if it's checked. Then, in the same window, click Printer > Cancel All Documents to clear any stuck jobs. This often resolves the **my hp printer is offline but connected to wifi** status when the queue is the culprit.

## Restart the Print Spooler

If the queue still shows offline, restart the print spooler service. Press Windows + R, type services.msc, and press Enter. Find Print Spooler, right-click it, and choose Restart. Wait a few seconds, then reopen the print queue. The status should change to "Ready" or "Online."

## Verification Test

Print a test page: right-click your HP printer in Settings and choose Printer properties > Print Test Page. If it prints, the offline status is fixed. If not, note the exact error.

## Rollback Note

If restarting the spooler causes other printers to disappear, restart your PC to restore them. For persistent issues,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult) before making further changes.
