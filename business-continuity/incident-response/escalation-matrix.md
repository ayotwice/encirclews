# Escalation Matrix

## Primary On-Call Rotation

### Level 1 - Service Desk
- **Role**: Initial incident triage and basic troubleshooting
- **Escalation Time**: 30 minutes for P1/P2, 2 hours for P3/P4
- **Contact**: +1-555-HELP (4357)
- **Backup**: Service Desk Supervisor

### Level 2 - Technical Teams

#### Infrastructure Team
- **Primary**: John Smith (Infrastructure Lead)
- **Contact**: +1-555-0101, john.smith@company.com
- **Backup**: Sarah Johnson (+1-555-0102)
- **Specialties**: Servers, networking, cloud infrastructure

#### Application Team
- **Primary**: Mike Chen (Application Lead)
- **Contact**: +1-555-0201, mike.chen@company.com
- **Backup**: Lisa Rodriguez (+1-555-0202)
- **Specialties**: Custom applications, databases, middleware

#### Security Team
- **Primary**: David Wilson (Security Lead)
- **Contact**: +1-555-0301, david.wilson@company.com
- **Backup**: Jennifer Lee (+1-555-0302)
- **Specialties**: Security incidents, compliance, forensics

### Level 3 - Management Escalation

#### IT Operations Manager
- **Name**: <Manager Name>
- **Contact**: +1-555-0401, manager@company.com
- **Escalation Triggers**: 
  - P1 incidents > 2 hours
  - P2 incidents > 4 hours
  - Multiple concurrent incidents

#### IT Director
- **Name**: <Director Name>
- **Contact**: +1-555-0501, director@company.com
- **Escalation Triggers**:
  - P1 incidents > 4 hours
  - Major security incidents
  - Business-critical system failures

#### CTO/CISO
- **Contact**: +1-555-0601, executive@company.com
- **Escalation Triggers**:
  - Extended outages (>8 hours)
  - Data breaches
  - Regulatory compliance issues

## Vendor Escalation Contacts

### Critical Vendors
- **AWS Support**: Enterprise Support, Case Priority: High
- **Microsoft**: Premier Support, +1-800-MICROSOFT
- **Salesforce**: Premier Success, priority escalation
- **Network Provider**: 24/7 NOC, +1-555-NET-OPS

## Escalation Decision Tree

```
Incident Detected
    ↓
Service Desk Assessment
    ↓
P1/P2? → YES → Immediate L2 Escalation
    ↓
    NO
    ↓
Standard L2 Escalation (per SLA)
    ↓
Resolution within SLA? → YES → Close
    ↓
    NO
    ↓
Management Escalation
    ↓
Extended Duration? → YES → Executive Escalation
```

## Communication Escalation

### Stakeholder Notification Matrix

| Incident Severity | Immediate (0-15 min) | 1 Hour | 4 Hours | 8+ Hours |
|-------------------|---------------------|---------|---------|----------|
| P1 | IT Ops Manager, Technical Teams | IT Director, Business Owners | CTO, Executive Team | CEO, Board (if applicable) |
| P2 | Technical Teams | IT Ops Manager | IT Director | CTO |
| P3 | Technical Teams | IT Ops Manager (if unresolved) | - | - |
| P4 | Technical Teams | - | - | - |

## After-Hours Contacts

### Weekend/Holiday Coverage
- **Primary On-Call**: Rotating schedule (see PagerDuty)
- **Backup On-Call**: Secondary rotation
- **Management**: IT Ops Manager (always available for P1)

### Emergency Contact Protocol
1. PagerDuty automatic escalation
2. Phone tree activation for P1 incidents
3. Slack incident channel (#incident-response)
4. Email distribution lists by severity

## Special Escalation Scenarios

### Security Incidents
- Immediate CISO notification
- Legal team involvement (if data breach)
- External forensics team (if required)
- Law enforcement (if criminal activity)

### Compliance Issues
- Compliance officer notification
- Audit team involvement
- Regulatory body notification (if required)
- Legal counsel consultation