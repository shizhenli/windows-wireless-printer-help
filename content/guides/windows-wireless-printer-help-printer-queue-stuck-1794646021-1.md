---
title: "Printer Queue Stuck on Windows 11: Clear It and Get Printing Again"
description: "Jobs piling up and nothing prints? Follow these steps to clear a stuck print queue on Windows 11 and verify your wireless printer works again."
seo_title: "Printer Queue Stuck? Fix Windows 11 Wireless Printing"
seo_description: "Jobs piling up and nothing prints? Follow these steps to clear a stuck print queue on Windows 11 and verify your wireless printer works again."
keywords:
  - "printer queue stuck"
date: 2026-11-14T20:01:34+08:00
publishDate: 2026-11-14T20:01:34+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

You are on Windows 11 with a wireless printer, and jobs are sitting in the queue while later jobs refuse to print. Let's walk through a controlled diagnosis to clear the **printer queue stuck** state and get your documents moving again.

## Step 1: Check the queue and printer status

Open Settings > Bluetooth & devices > Printers & scanners, select your printer, and choose Open print queue. If you see jobs listed with statuses like "Error" or "Printing" that never progress, the queue is jammed. Note whether the printer shows "Offline" or "Paused." If it says Paused, click Resume. If Offline, power-cycle the printer and wait for it to reconnect to Wi-Fi.

## Step 2: Clear the stuck jobs

In the print queue window, click Printer > Cancel All Documents. If jobs remain, open Services (services.msc), find Print Spooler, right-click, and choose Restart. Then return to the queue and cancel any remaining jobs. This clears the jammed spooler without deleting your printer setup.

## Step 3: Verify with a test print

Print a one-page test document from Notepad. Watch the queue: the job should appear briefly and then disappear as it prints. If the queue empties and the page prints, the issue is resolved. If the job stays stuck, restart the Print Spooler service again and repeat Step 2.

## Rollback note

If clearing the queue causes your printer to disappear, go to Printers & scanners and use Add device to reinstall it. Your original driver settings remain intact.

If the queue still jams after these steps,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult) for a guided diagnosis.
