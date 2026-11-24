---
title: "Wireless Printer Not Found on Windows 11: Fix Discovery Before You Reset"
description: "Windows 11 can't find your wireless printer on the same network? Follow these targeted checks to restore discovery without resetting everything."
seo_title: "Wireless Printer Not Found on Windows 11? Fix Discovery"
seo_description: "Windows 11 can't find your wireless printer on the same network? Follow these targeted checks to restore discovery without resetting everything."
keywords:
  - "wireless printer not found"
date: 2026-11-24T08:12:38+08:00
publishDate: 2026-11-24T08:12:38+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

Your Windows 11 PC and wireless printer are on the same network, but Windows cannot discover the printer, leaving you stuck at the **wireless printer not found** stage.

## Confirm the Printer Is on the Same Network and Reachable

On the printer's control panel, print a network configuration page. Look for the IP address and subnet mask. On your PC, open Settings > Network & internet > Wi-Fi and check the IP address and subnet mask. The first three octets of both IP addresses must match (for example, 192.168.1.x). If they differ, the printer is on a different network or band; reconnect it to the same SSID your PC uses.

Next, open Command Prompt and run `ping <printer IP>`. A reply with time values means the printer is reachable. "Destination host unreachable" or timeouts mean the network path is blocked; check that the printer is not connected to a guest network and that client isolation is disabled on your router.

## Verify Discovery Settings and Services

Open Settings > Bluetooth & devices > Printers & scanners. Select Add device > Add manually. Choose "Add a printer using an IP address or hostname" and enter the printer's IP address. If Windows adds it successfully, discovery is the only broken piece, not the driver or port.

Also confirm these services are running: Function Discovery Provider Host, Function Discovery Resource Publication, and SSDP Discovery. Set each to Automatic and start it. Then return to Printers & scanners and let the scan complete.

## Verification Test

Print a test page from the newly added printer. If it prints, open the original discovery scan once more; the printer should now appear. If it does not, remove the manually added printer and restart the Print Spooler service, then rescan.

## Rollback Note

If these changes do not help, remove any printer entries you added during this process and restore the services you modified to their previous startup type. For guided diagnosis,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).
