---
title: "HP Printer Offline on Wi-Fi: Fix Windows 11 Status Before You Reset"
description: "Windows 11 shows your HP printer offline even though it's connected to Wi-Fi. Follow these targeted checks to confirm the queue state and restore the correct status."
seo_title: "HP Printer Offline on Wi-Fi: Fix Windows 11 Status Before You Reset"
seo_description: "Windows 11 shows your HP printer offline even though it's connected to Wi-Fi. Follow these targeted checks to confirm the queue state and restore the correct status."
keywords:
  - "hp printer offline but connected to wifi mac"
date: 2026-11-17T10:12:18+08:00
publishDate: 2026-11-17T10:12:18+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

You're on Windows 11, your HP printer is powered on and connected to Wi-Fi, but the queue still marks it offline. That mismatch is the specific failure we'll fix here.

## Confirm the queue is the only problem
Open Settings > Bluetooth & devices > Printers & scanners, select your HP printer, and choose Open print queue. If the status says Offline while the printer's Wi-Fi light is solid, the PC is holding a stale connection state. Do not remove the printer yet.

## Check the port and spooler state
In the same printer entry, click Printer properties > Ports. Note which port is checked. A WSD port can report offline after the printer sleeps or changes IP. If the port is WSD, switch to a Standard TCP/IP port using the printer's current IP address from its control panel. Then open Services (services.msc), restart Print Spooler, and reopen the queue. If the status changes to Ready, the port was the cause.

## Verify with a test page
Print a Windows test page from Printer properties > General. If it prints, the offline flag is cleared. If the queue still shows offline, power-cycle the printer and router together, wait two minutes, and retry.

## Rollback note
If switching ports causes no output, return to the original port and restart the spooler again. This restores your previous setup before further changes.

If the queue still marks the printer offline after these checks, the remaining cause is usually a driver-level mismatch. For a controlled diagnosis,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult). This **hp printer offline but connected to wifi mac** scenario is resolved once the queue reports Ready and the test page prints.
