# TKT-002 — Website unavailable while Wi-Fi was off

Date:26 September 2026  
Type:Simulated personal lab  
Platform:macOS; Google Chrome  
Status:Resolved

## Symptom
A website did not load in Chrome while Wi-Fi was turned off on my Mac.

## Investigation
I checked the Wi-Fi setting and confirmed it was off. After reconnecting, I ran `ping -c 4 example.com` and `nslookup example.com`.

**Ping result:** [Write what you saw]  
**DNS lookup result:** [Write what you saw]

## Action taken
I turned Wi-Fi back on and reconnected to my network.

## Verification
I reloaded the website in Chrome, and it opened successfully.

## What I learned
I learned to check the Wi-Fi connection first, then use `ping` and `nslookup` to investigate connectivity and DNS.
