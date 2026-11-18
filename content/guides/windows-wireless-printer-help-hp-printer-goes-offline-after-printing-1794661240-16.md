---
title: "HP Printer Goes Offline After Printing: Fix Windows 11 Offline Status"
description: "HP printer goes offline after printing on Windows 11? Follow these steps to diagnose the queue state and restore the offline status."
seo_title: "HP Printer Goes Offline After Printing on Windows 11? Fix It"
seo_description: "HP printer goes offline after printing on Windows 11? Follow these steps to diagnose the queue state and restore the offline status."
keywords:
  - "hp printer goes offline after printing"
date: 2026-11-18T11:30:37+08:00
publishDate: 2026-11-18T11:30:37+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

You finish a print job, and Windows 11 immediately marks your wireless HP printer offline even though it is still powered on.

## Confirm the queue state

Open Settings > Bluetooth & devices > Printers & scanners, select your HP printer, and choose Open print queue. If the status reads Offline while the printer is on, note whether any jobs are stuck. A single stalled job can hold the queue offline. Cancel all jobs, then restart the Print Spooler service: press Windows + R, type services.msc, find Print Spooler, and click Restart. Reopen the queue. If the status returns to Ready, the queue was the cause.

## Check the port and power state

In Printers & scanners, open Printer properties > Ports. Confirm the checked port matches your printer's current connection, typically a WSD or standard TCP/IP port. If the port is wrong, select the correct one and apply. Next, check the printer's sleep or auto-off setting; some HP models drop their network link after a job. Set sleep to a longer interval if available.

## Verification test

Print a one-page test from Notepad. Watch the queue status during and after the job. If it stays Ready and the page prints, the fix holds. If it flips back to Offline, the **hp printer goes offline after printing** pattern points to the port or power setting, not the driver.

## Rollback note

If changes make printing worse, return the port selection and sleep setting to their previous values, then restart the Print Spooler again. For a guided diagnosis,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).
