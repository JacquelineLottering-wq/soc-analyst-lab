# Alert Investigation: Repeated Blocked External Connection Attempts

## Alert Summary
The firewall generated multiple alerts indicating repeated blocked outbound connection attempts from an internal workstation to a known malicious external IP address. The pattern suggests possible command-and-control (C2) communication or unauthorized external connectivity attempts.

## Timeline of Events
- Firewall detected outbound connection attempts to blocked IP
- Multiple attempts observed within short interval
- Traffic originated from internal user workstation
- Destination IP matched threat intelligence blacklist

## Investigation Steps
- Reviewed firewall traffic logs
- Verified destination IP reputation
- Checked endpoint associated with source IP
- Correlated activity with endpoint security alerts
- Reviewed recent user activity and processes

## Analysis & Findings
The destination IP is associated with known malicious infrastructure.  
The repeated connection attempts indicate automated or persistent outbound communication behaviour rather than normal user activity.  

No confirmed malware alert was triggered on the endpoint at the time of analysis, but the behaviour is consistent with potential beaconing or unauthorized external communication attempts.

## Severity Assessment
Severity: Medium–High  
Reason: Repeated communication attempts to known malicious external host.

## Conclusion
The activity indicates suspicious outbound communication behaviour requiring further endpoint inspection to rule out compromise.

Recommended actions include:
- Endpoint security scan
- Network monitoring for continued attempts
- Blocking destination at perimeter controls
- Reviewing running processes on host

## Analyst Note
Outbound connections to known malicious infrastructure are a common early indicator of compromise. Early containment reduces risk of persistence or data exfiltration.
