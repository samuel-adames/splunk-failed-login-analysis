# Unauthorized AWS API Calls (AccessDenied)

# Splunk Failed Login Analysis

## Objective
Detect and analyze failed authentication attempts using Splunk,
simulating a SOC analyst investigation based on AWS CloudTrail logs.

## Dataset
AWS CloudTrail logs in JSON format were ingested into Splunk.
Most events were indexed into the default `main` index, which contains
over 2.4 million events.

## Tools Used
- Splunk Enterprise (Free Trial)
- AWS CloudTrail sample logs
- GitHub (documentation and version control)

## Detection Logic
Failed authentication attempts were identified by filtering
CloudTrail events with the error code `AccessDenied`.

## Evidence
![Failed Login Detection](screenshots/failed-login-basic.png)

## Findings
- Multiple AccessDenied events detected
- Requests originated from specific IP addresses
- Events related to AWS API calls without sufficient permissions

## Conclusion
This project demonstrates basic SOC detection skills using Splunk,
including log ingestion, query development, and security analysis.
