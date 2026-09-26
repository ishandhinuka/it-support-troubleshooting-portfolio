# TKT-002 — Website would not load while Wi-Fi was off

**Date:** 2026-09-26  
**Type:** Simulated personal lab  
**Platform:** macOS, Google Chrome  
**Priority and reason:** Low — a controlled test on my own Mac  
**Status:** Resolved

## Symptom and impact
A website would not load in Chrome while Wi-Fi was turned off on my Mac. I expected it to load once the Mac was connected to Wi-Fi. This affected only my test device.

## Investigation
| Step | Observation | What it suggests |
| --- | --- | --- |
| 1. Checked Wi-Fi | Wi-Fi was off. | The Mac had no Wi-Fi connection. |
| 2. Ran `ping -c 4 example.com` after reconnecting | Four packets were sent and received with 0% packet loss. | The Mac could reach example.com after Wi-Fi was restored.|
| 3. Ran `nslookup example.com` after reconnecting | Four packets were sent and received with 0% packet loss. | The Mac could reach example.com after Wi-Fi was restored.|

## Action taken
I turned Wi-Fi back on and reconnected to my network. After reconnecting, I ran `ping -c 4 example.com` and `nslookup example.com` to check connectivity and DNS.

## Verification
I reloaded the website in Chrome, and it opened successfully.

## Evidence
None.

## What I learned
I learned to check whether Wi-Fi is connected before investigating a website issue. I also practised using `ping` and `nslookup` to check connectivity and DNS separately.
