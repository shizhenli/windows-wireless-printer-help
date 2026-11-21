---
title: "Printer Queue Stuck on Windows 11: Clear the Jam and Restore Printing"
description: "Jobs stuck in the Windows 11 print queue? Follow these step-by-step checks to clear the jam, verify the fix, and get your wireless printer working again."
seo_title: "Printer Queue Stuck? Fix It on Windows 11 Wireless Printers"
seo_description: "Jobs stuck in the Windows 11 print queue? Follow these step-by-step checks to clear the jam, verify the fix, and get your wireless printer working again."
keywords:
  - "printer queue stuck"
date: 2026-11-21T16:57:11+08:00
publishDate: 2026-11-21T16:57:11+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

You sent a document to your wireless printer, but the job sits in the queue and later jobs won't print either. Here's how to diagnose and clear a **printer queue stuck** state without guessing.

## Check the queue and spooler status

Open Settings > Bluetooth & devices > Printers & scanners, select your printer, and choose Open print queue. If you see jobs listed as "Printing" or "Pending" for more than a minute, the queue is stalled. Next, press Win+R, type services.msc, and find Print Spooler. If its status is not "Running," right-click and start it. If it is running, right-click and restart it. A successful restart returns the service to "Running" within a few seconds.

## Clear the stuck jobs

Back in the print queue window, click Printer > Cancel All Documents. If jobs remain, stop the Print Spooler service again, then open File Explorer and navigate to C:\Windows\System32\spool\PRINTERS. Delete any files inside that folder. Restart the Print Spooler service. This clears the spool files that keep the queue blocked.

## Verify the fix

Print a Windows test page from Printer properties > General > Print Test Page. The page should emerge within 30 seconds and the queue should empty. Then print a short document from Notepad to confirm normal jobs flow.

## Rollback note

If clearing the spool folder causes a printer to disappear, go to Settings > Bluetooth & devices > Printers & scanners and use Add device to reinstall it. Your original driver remains available in Device Manager under Print queues, so you can roll back by updating the driver there if needed.

If the queue still stalls after these steps, the issue may be the wireless connection or driver.

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult) for a guided diagnosis.
