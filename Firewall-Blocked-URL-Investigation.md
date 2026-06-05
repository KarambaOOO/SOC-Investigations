# Access to Blacklisted External URL Blocked by Firewall

## Incident Summary

A firewall alert was generated after an internal host attempted to access a URL listed in the organization's blacklist and threat intelligence feed. The firewall successfully blocked the outbound connection, preventing communication with the destination host.

## Alert Details

* Alert ID: 8816
* Alert Type: Firewall
* Severity: High
* Source IP: 10.20.2.17
* Destination IP: 67.199.248.11
* URL: hxxp://bit.ly/3sHkX3da12340
* Protocol: TCP
* Action: Blocked
<img width="1538" height="658" alt="Снимок экрана 2026-06-05 184527" src="https://github.com/user-attachments/assets/e0669503-852c-4e37-be4a-62b7fcdd5b2f" />

## Investigation Steps

1. Reviewed the firewall alert.
2. Identified the source and destination IP addresses.
3. Verified the URL involved in the connection attempt.
4. Confirmed the URL was blocked according to the firewall policy.
5. Confirmed that the firewall blocked the connection.

## Findings
<img width="1905" height="752" alt="Снимок экрана 2026-06-05 184608" src="https://github.com/user-attachments/assets/63bdc6a2-ed5b-4a76-91a9-2328c7cf6809" />
<img width="1872" height="922" alt="Снимок экрана 2026-06-05 184654" src="https://github.com/user-attachments/assets/dd006c1c-170b-477e-bca7-c66e23e316f7" />

The investigation confirmed an attempt to access a URL that was present in the organization's blacklist and threat intelligence feed.

No evidence of:

* Credential theft
* Malware execution
* Data exfiltration
* Successful communication with the destination host

was identified.

## Classification

**True Positive**

## Impact Assessment

The security control operated as intended and blocked the connection attempt. No compromise or data loss was observed.

## Recommended Actions

* Identify the user associated with source IP 10.20.2.17.
* Review how the user obtained the malicious URL.
* Verify whether additional users attempted to access the same resource.
* Continue monitoring for similar events.
* Reinforce user awareness regarding suspicious links and URL shorteners.

## Lessons Learned

Preventive security controls successfully stopped access to a malicious resource before any impact to the environment occurred.
