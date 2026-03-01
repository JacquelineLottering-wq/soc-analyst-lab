# Phishing Incident Response Procedure

## Purpose
Provide a consistent response approach when phishing activity is suspected or confirmed within the environment.

## Identification
Potential phishing indicators include:
- Unexpected credential or payment requests
- Suspicious sender address or domain
- Urgent or coercive language
- Unknown attachments or links

## Containment Steps
- Remove email from affected mailbox
- Block sender address/domain
- Disable malicious links if possible
- Isolate endpoint if interaction occurred

## Eradication Steps
- Delete all copies of phishing message
- Block identified indicators in security tools
- Remove any downloaded malicious files

## Recovery Steps
- Reset affected user credentials
- Restore normal mailbox access
- Confirm no persistence mechanisms remain

## Post-Incident Actions
- Notify user and provide awareness guidance
- Update email filtering controls if required
- Share indicators with security team

## Analyst Notes
This procedure supports early containment to reduce risk of credential compromise and lateral movement.
