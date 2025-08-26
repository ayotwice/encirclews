# Incident Communication Templates

## Initial Incident Notification

### Internal Notification (Slack/Teams)
```
🚨 INCIDENT ALERT - P[X] 🚨
Incident ID: INC-YYYY-NNNN
Severity: P[X] - [Critical/High/Medium/Low]
Status: Investigating
Affected Systems: [System Names]
Impact: [Brief description of user impact]
Incident Commander: [Name]
Next Update: [Time]
Bridge: [Conference line/link]
```

### Executive Notification (Email)
```
Subject: P[X] Incident - [Brief Description] - INC-YYYY-NNNN

Executive Summary:
We are currently experiencing a P[X] incident affecting [systems/services]. 

Impact: [Description of business impact]
Affected Users: [Number/percentage of users affected]
Start Time: [Timestamp]
Current Status: [Investigating/Identified/Resolving]
ETA for Resolution: [Best estimate or "Under investigation"]

Actions Taken:
- [Action 1]
- [Action 2]

Next Steps:
- [Next step 1]
- [Next step 2]

Incident Commander: [Name, Contact]
Next Update: [Time]
```

## Status Updates

### Hourly Update Template
```
📊 INCIDENT UPDATE - INC-YYYY-NNNN
Time: [Timestamp]
Status: [Investigating/Identified/Resolving/Monitoring]
Progress: [What has been accomplished]
Current Actions: [What is being done now]
Blockers: [Any impediments to resolution]
Next Update: [Time]
ETA: [Updated estimate if available]
```

### Customer-Facing Update (Status Page)
```
[Timestamp] - [Investigating/Identified/Monitoring/Resolved]

We are aware of an issue affecting [service/feature]. Users may experience [specific impact]. We are actively investigating and will provide updates as more information becomes available.

Next update: [Time]
```

## Resolution Notification

### Internal Resolution Notice
```
✅ INCIDENT RESOLVED - INC-YYYY-NNNN
Resolution Time: [Timestamp]
Total Duration: [X hours Y minutes]
Root Cause: [Brief technical explanation]
Resolution: [What was done to fix it]
Monitoring: [Ongoing monitoring plans]
Post-Incident Review: Scheduled for [Date/Time]
```

### Customer Resolution Notice
```
[Timestamp] - Resolved

The issue affecting [service/feature] has been resolved. All services are now operating normally. We apologize for any inconvenience this may have caused.

If you continue to experience issues, please contact support.
```

## Escalation Communication

### Management Escalation
```
Subject: Escalation Required - P[X] Incident - INC-YYYY-NNNN

This incident requires management attention due to:
- [Reason for escalation - duration, impact, complexity]

Current Situation:
- Duration: [X hours]
- Impact: [Business impact description]
- Resources Engaged: [Teams involved]
- Challenges: [What's preventing resolution]

Requested Support:
- [Specific help needed]
- [Additional resources required]
- [Decision points requiring management input]

Incident Commander: [Name, Contact]
```

## Special Incident Types

### Security Incident Notification
```
🔒 SECURITY INCIDENT - CONFIDENTIAL
Incident ID: SEC-YYYY-NNNN
Classification: [Data Breach/Unauthorized Access/Malware/etc.]
Severity: [Critical/High/Medium/Low]
Affected Systems: [Systems involved]
Data at Risk: [Type of data potentially affected]
Containment Status: [Contained/In Progress/Not Contained]
CISO Notified: [Yes/No - Time]
Legal Notified: [Yes/No - Time]
External Reporting Required: [TBD/Yes/No]

DO NOT FORWARD - CONFIDENTIAL
```

### Vendor-Related Incident
```
Subject: Vendor Incident Impact - [Vendor Name] - INC-YYYY-NNNN

We are experiencing service disruption due to an incident at [Vendor Name].

Vendor Status: [Their reported status]
Our Impact: [How it affects our services]
Workaround: [Any temporary solutions in place]
Vendor ETA: [Their estimated resolution time]
Our Actions: [What we're doing to mitigate]

Vendor Incident ID: [Their reference number]
Vendor Contact: [Primary contact managing their incident]
```

## Communication Checklist

### During Incident
- [ ] Initial notification sent within 15 minutes
- [ ] Stakeholders identified and notified per escalation matrix
- [ ] Status page updated (for customer-facing incidents)
- [ ] Regular updates provided per communication schedule
- [ ] Executive briefings scheduled for extended incidents

### Post-Resolution
- [ ] Resolution notification sent to all stakeholders
- [ ] Status page updated with resolution
- [ ] Customer apology/explanation provided if needed
- [ ] Post-incident review scheduled
- [ ] Lessons learned documented