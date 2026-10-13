# Troubleshooting Guide: Network and Internet Connectivity

## Scenario
A user reports no internet access, slow connectivity, or an application that cannot reach a network resource.

## 1. Ask focused questions
- Is the issue no connection, slow performance, intermittent drops, or one application only?
- Is Wi-Fi connected? Does the device show an IP address?
- Are other devices or users affected?
- Does the issue happen on one network or all networks?
- Is a VPN required? Did the issue start after moving locations or changing networks?
- What error appears, and when did it begin?

## 2. Check physical and wireless connectivity
1. Confirm Wi-Fi is enabled and the correct authorized network is selected.
2. Check airplane mode and signal strength.
3. For Ethernet, check cable seating, dock, link lights, and switch port only if authorized.
4. Test another known-good cable or approved network where available.
5. Do not reset network equipment or change shared router settings without authorization.

## 3. Check IP configuration
Open Command Prompt:
```bat
ipconfig /all
```
Review the active adapter, IPv4 address, subnet mask, default gateway, DHCP status, and DNS servers.

Interpret carefully:
- An address beginning `169.254` often indicates the device did not obtain an IPv4 address from DHCP.
- A missing default gateway may prevent access outside the local subnet.
- An unexpected adapter may be disconnected or virtual; identify the active adapter before drawing conclusions.

## 4. Test in a sequence
Use approved destinations and remember some networks block ping.

```bat
ping <default-gateway-IP>
nslookup <approved-hostname>
ping <approved-hostname>
tracert <approved-hostname>
```

Suggested interpretation:
- Gateway test fails: check local Wi-Fi/Ethernet, adapter, address, subnet, and gateway.
- Gateway works but name lookup fails: investigate DNS configuration or DNS service.
- Name resolves but application fails: check the application, proxy/VPN, firewall policy, service availability, and required port with the authorized team.
- Intermittent results: compare times, signal strength, packet loss, and whether other devices are affected.

A failed ping alone does not prove a host is down; ICMP may be blocked.

## 5. Low-risk actions
- Disconnect/reconnect to the approved Wi-Fi network if appropriate.
- Re-seat the Ethernet cable or test a known-good cable.
- Disable/enable an adapter only when safe and authorized.
- Restart the device if appropriate and after saving work.
- Use network reset or release/renew commands only when justified, authorized, and after understanding the impact. Avoid changing DNS, proxy, VPN, or firewall settings without approval.

## 6. Verify
- Confirm valid IP configuration.
- Retest the original destination or application.
- Check whether the problem persists over a reasonable observation period.
- Document the adapter, tests, results, likely cause, fix, and any escalation.

## Results
- Symptom and scope: `[value]`
- `ipconfig /all` findings (sanitized): `[value]`
- Gateway/DNS/application test results: `[value]`
- Cause: `[confirmed / suspected / unknown]`
- Fix and verification: `[value]`
