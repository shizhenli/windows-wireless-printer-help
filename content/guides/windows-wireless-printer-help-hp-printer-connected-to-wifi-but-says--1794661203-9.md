---
title: "HP Printer Connected to Wi-Fi but Says Offline on Windows 11: Fix the Queue State"
description: "HP printer connected to Wi-Fi but says offline on Windows 11? Diagnose the queue state and restore the expected offline marking with this focused fix."
seo_title: "HP Printer Connected to Wi-Fi but Says Offline: Windows 11 Queue Fix"
seo_description: "HP printer connected to Wi-Fi but says offline on Windows 11? Diagnose the queue state and restore the expected offline marking with this focused fix."
keywords:
  - "hp printer connected to wifi but says offline"
date: 2026-11-17T09:38:48+08:00
publishDate: 2026-11-17T09:38:48+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

**hp printer connected to wifi but says offline**. You are on a Windows 11 PC with a wireless HP printer that is powered on and joined to Wi-Fi, yet the queue still shows it as offline.

## Check the queue state before touching the printer

Open Settings > Bluetooth & devices > Printers & scanners, select your HP printer, and choose Open print queue. In the queue window, click Printer in the menu bar. If Use Printer Offline has a checkmark, click it once to clear it. This is the most common reason Windows marks the printer offline while it is powered on. If the checkmark is absent, leave the menu alone and move to the next check.

## Verify the port and the printer's network state

In the same queue window, open Printer > Properties > Ports. Confirm the checked port matches your printer's current IP address or hostname. If it points to an old address, the queue cannot reach the device and Windows marks it offline. Next, print the printer's network configuration page from its control panel and compare the IP address with the port entry. If they differ, update the port to the current address.

## Run a verification test

Print a one-page test document from Notepad. Watch the queue: if the job moves from Pending to Printing, the offline status is cleared. If it stays Pending, the port or driver still needs attention.

## Rollback note

If clearing Use Printer Offline or changing the port makes printing worse, return to Printer > Properties > Ports and restore the previous port selection. You can also re-check Use Printer Offline to return to the original state before continuing diagnosis.

If the queue still reports the printer offline after these checks, the issue may be the driver or the printer's sleep behavior. For a controlled next step,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).
