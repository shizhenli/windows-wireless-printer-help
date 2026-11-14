---
title: "Brother Printer Goes Offline in Sleep Mode: Fix Windows 11 Offline Status"
description: "Your Brother wireless printer shows offline in Windows 11 after sleep mode. Follow these technician steps to diagnose the queue and restore online status."
seo_title: "Brother Printer Offline in Sleep Mode on Windows 11? Fix It"
seo_description: "Your Brother wireless printer shows offline in Windows 11 after sleep mode. Follow these technician steps to diagnose the queue and restore online status."
keywords:
  - "brother printer goes offline in sleep mode"
date: 2026-11-14T20:01:34+08:00
publishDate: 2026-11-14T20:01:34+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

Your Windows 11 PC shows the Brother printer as offline in the queue even though the printer is powered on and was working before it entered sleep mode.

## Check the Printer's Sleep State and Network Light

First, wake the printer by pressing any button on its panel. Look at the Wi-Fi indicator: a steady light means it is connected; a blinking or off light means it dropped off the network during sleep. If the light is not steady, reconnect the printer to Wi-Fi using its control panel before continuing. A steady light confirms the printer is reachable and the issue is likely Windows-side.

## Clear the Stale Offline Flag in Windows

Open Settings > Bluetooth & devices > Printers & scanners. Select your Brother printer and choose Open print queue. If the status reads Offline, click Printer in the menu bar and uncheck Use Printer Offline. This clears the flag Windows set when the printer was unreachable during sleep. Next, check that the correct port is selected under Printer > Properties > Ports; the standard TCP/IP port for your printer's IP address should be checked. If the IP changed after sleep, update the port address.

## Adjust Power Management

In Device Manager, expand Print queues, right-click your Brother model, and open Properties > Power Management. Uncheck Allow the computer to turn off this device to save power. This prevents Windows from suspending the driver, a common cause when the **brother printer goes offline in sleep mode**.

## Verification Test

Print a Windows test page from Printer Properties > General > Print Test Page. The job should leave the queue and print within 30 seconds, and the status should read Ready, not Offline.

## Rollback Note

If printing fails after these changes, re-enable the power management checkbox and restart the Print Spooler service to return to the previous state. For guided diagnosis,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).
