# Active-Directory-2.0

## Overview
Active Directory 2.0 is a hands-on enterprise lab that combines Windows Active Directory, Splunk Enterprise, and Splunk SOAR to simulate a real-world Security Operations Center (SOC) workflow. The project demonstrates how security events generated from Active Directory can be monitored, investigated, and automatically responded to using playbooks.

## Project Objectives
- Deploy a Windows Active Directory environment.
- Collect Windows security logs in Splunk.
- Detect successful unauthorized login activity.
- Trigger an automated SOAR playbook.
- Notify the SOC analyst for approval before taking action.
- Automatically disable compromised Active Directory accounts after analyst approval.

## Environment
- Windows Server (Domain Controller)
- Active Directory Domain Services (AD DS)
- Windows Client
- Splunk Enterprise
- Splunk SOAR
- Slack
- Email Notifications

## Workflow
1. Windows security events are forwarded from the Domain Controller and Windows client to Splunk.
2. Splunk detects a successful unauthorized login.
3. An alert triggers a Splunk SOAR playbook.
4. The playbook sends an email and Slack notification to the SOC analyst.
5. The analyst decides whether the account should be disabled.
6. If approved, Splunk SOAR automatically disables the Active Directory user account.
7. If denied, no action is taken.

## Skills Demonstrated
- Active Directory Administration
- Windows Event Log Analysis
- Splunk Enterprise
- Splunk SOAR Automation
- Incident Response
- Security Alert Triage
- Active Directory User Management
- SOC Playbook Development
- Security Operations Workflow

## Future Improvements
- Public IP reputation enrichment
- VirusTotal integration
- Microsoft Sentinel integration
- Microsoft Defender XDR integration
- MITRE ATT&CK mapping
- Automated case management
