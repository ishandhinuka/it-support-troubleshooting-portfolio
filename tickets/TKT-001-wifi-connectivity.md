# TKT-001 — Wi-Fi connected, website does not load

**Status:** illustrative scenario; replace observations after running your own test  
**Priority:** medium in this scenario  
**Environment:** example Windows laptop and home Wi-Fi

## Reported symptom
A user says the laptop shows Wi-Fi connected but a website does not open. Other sites may or may not work; ask before assuming.

## Questions and checks
1. Confirm the exact error, affected sites, start time, and whether another device works on the same network.
2. Check the Wi-Fi connection and IP configuration with `ipconfig /all`. Do not publish addresses or network names.
3. Test the default gateway with `ping <gateway-address>`.
4. Test DNS with `nslookup example.com`, then try another known site in the browser.
5. If permitted, reconnect Wi-Fi and retry. Document any change.

## Example decision path
- No gateway response: inspect local connection, signal, and router; escalate if the network is unavailable to multiple users.
- Gateway responds but DNS fails: investigate DNS configuration or resolver availability; escalate if managed settings need an administrator.
- DNS resolves but one site fails: inspect browser error and site availability; do not assume the entire network is down.

## Resolution and verification
**To complete after your own exercise:** record the exact action taken, command results, a successful page load, and whether the issue recurred. Do not mark as resolved until verified.

## Learning
Connectivity, DNS, and a specific website are separate failure points. Each check narrows the cause.
