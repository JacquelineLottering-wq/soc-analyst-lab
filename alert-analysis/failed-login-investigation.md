# Alert Investigation: Multiple Failed Login Attempts

# Alert Summary
An alert was generated due to multiple failed login attempts on a user account, followed by a successful login within a short time window.

This activity may indicate a brute-force or credential-stuffing attempt.

---

#Timeline of Events
- Multiple failed login attempts detected
- Successful login shortly after failures
- Login originated from the same source IP

---

# Investigation Steps
- Reviewed authentication logs in the SIEM
- Filtered events by username and source IP
- Checked timestamp correlation between failed and successful attempts
- Assessed whether the behaviour matched normal user activity

---

# Analysis & Findings
The pattern of repeated failed logins followed by a successful authentication suggests potential unauthorized access.

However, no further suspicious activity was detected after the successful login.

---

# Severity Assessment
**Severity:** Medium  
**Reason:** Possible credential compromise, but limited post-login activity.

---

# Conclusion
This alert requires monitoring but does not immediately confirm a security incident.

Recommended actions include:
- Monitoring the account for further suspicious activity
- Advising a password reset
- Enabling multi-factor authentication (if not already enabled)

---

# Analyst Notes
This investigation demonstrates common SOC alert triage and analysis steps used to identify authentication-based threats.

