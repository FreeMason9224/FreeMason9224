# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability, please report it to the repository maintainer at [your-email@example.com]. Include a detailed description of the vulnerability and any steps to reproduce it. The maintainer will respond as soon as possible to address the issue.

## Handling Vulnerabilities

When a vulnerability is reported, the following steps will be taken:

1. Acknowledge the report and communicate with the reporter to gather more information if needed.
2. Assess the severity and impact of the vulnerability.
3. Develop and test a fix for the vulnerability.
4. Release the fix and notify the reporter and affected users.
5. Update the security policy and documentation as needed.

## Secure Storage and Rotation of Secrets

To ensure the security of sensitive information, follow these guidelines:

- Use GitHub Secrets to store sensitive information such as `GPG_PRIVATE_KEY`, `GPG_PASSPHRASE`, and `GPG_KEY_ID`.
- Avoid hardcoding any sensitive information directly in the code or configuration files. Instead, reference the secrets stored in GitHub Secrets.
- Regularly rotate secrets and update them in the repository settings to minimize the risk of exposure.
- Ensure that decrypted secrets are securely cleaned up after use, as demonstrated in the cleanup step of the `.github/workflows/Secure Storage Workflow main.yml` file.
