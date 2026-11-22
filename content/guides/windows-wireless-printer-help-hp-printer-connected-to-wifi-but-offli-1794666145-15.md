---
title: "HP Printer Connected to Wi-Fi but Offline on Windows 10: Clear the Offline Flag"
description: "Step-by-step fix for an HP printer that shows offline in Windows 10 despite being powered on and connected to Wi-Fi. Clear the offline flag and verify printing."
seo_title: "HP Printer Connected to Wi-Fi but Offline Windows 10 Fix"
seo_description: "Step-by-step fix for an HP printer that shows offline in Windows 10 despite being powered on and connected to Wi-Fi. Clear the offline flag and verify printing."
keywords:
  - "hp printer connected to wifi but offline windows 10"
date: 2026-11-22T09:12:38+08:00
publishDate: 2026-11-22T09:12:38+08:00
draft: false
categories:
  - "Printing"
category_slug: "printing"
---

## Troubleshooting

You see your HP printer marked offline in the Windows queue even though it is powered on and joined to Wi-Fi. This is the **hp printer connected to wifi but offline windows 10** scenario where Windows has flagged the device offline before a controlled diagnosis. Start by opening Settings > Devices > Printers & scanners, select your HP printer, and click Open queue. In the queue window, check the status line under the printer name. If it says Offline, click Printer in the menu bar and uncheck Use Printer Offline if it is checked. Next, right-click the printer and choose See what's printing, then clear any stuck jobs with Document > Cancel. Now verify the port: right-click the printer > Printer properties > Ports tab. The checked port should be a Standard TCP/IP port matching your printer's IP address, not a WSD port. If it is WSD, note the current port name, then add a Standard TCP/IP port using the printer's IP from its control panel network report, and select it. This is your rollback point: if printing fails after the change, return to the Ports tab and reselect the original port. To verify, print a Windows test page from Printer properties > General > Print Test Page. A successful page confirms the offline flag is cleared. If the queue still shows offline, restart the Print Spooler service: open services.msc, right-click Print Spooler, and choose Restart. If the status returns,

![Windows printer queue and port settings beside a printed test page](/images/service-detail-960.webp "Windows printer queue and port check")

[Ask for help](/#consult).

Repeat the same check after a restart and confirm the result twice.
