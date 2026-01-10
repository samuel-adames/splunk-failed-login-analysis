## Analysis Notes

- Most failed login attempts were caused by insufficient IAM permissions
- Several requests originated from the same IP address
- Events were classified as AWS API calls rather than console logins

Potential risks:
- Misconfigured IAM policies
- Possible credential misuse

Recommended actions:
- Review IAM permissions
- Enable alerts for repeated AccessDenied events
