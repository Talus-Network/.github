# Talus Labs Security Policy

This document describes the Talus Labs Security team's process for handling security issues.

## Reporting Security Issues

__IMPORTANT:__ _Please DO NOT open public issues for security related matters, or discuss it in public forum or on social media._

### Email

All security issues should be reported via email to [security-reports@taluslabs.xyz](mailto:security-reports@taluslabs.xyz). Email is delivered to the Talus Labs security team.

Include the following details in the report:

- Your name;
- Your affiliation (if applicable);
- Technical description of the issue, including steps to reproduce;
- Explanation of who may be able to exploit this vulnerability and what the impact or implications may be;
- Whether this vulnerability is public or known to third parties. Please provide details where applicable;

_Please notify the Talus Labs security team at the email above of existing public issues that may be of critical security importance._ Please ensure to include the issue ID along with a short description / explanation of the security relevance.

### GitHub Private Vulnerability Reporting

Under the repository "Security" tab / Security Advisories you will find "Report a vulnerability". Please complete the provided form with as much details as possible.

For more information on GitHub private vulnerability reporting [see this](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing/privately-reporting-a-security-vulnerability).

_Best practices for writing repository security advisories_ can be found [here](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing/best-practices-for-writing-repository-security-advisories).

Security researchers can also use the REST API to privately report security vulnerabilities. For more information, see "[Privately report a security vulnerability](https://docs.github.com/en/rest/security-advisories/repository-advisories#privately-report-a-security-vulnerability)" in the REST API documentation.

### Encrypted Communication

If you wish to encrypt your vulnerability report, please use our PGP public key:

- **Download**: [https://talus.network/security-pgp-key.txt](https://talus.network/security-pgp-key.txt)
- **Key Server**: [keys.openpgp.org](https://keys.openpgp.org)
- **Fingerprint**: `103391C9AE4BE87A85E3EFAE2D4462A29BAB94AE`

Always verify the fingerprint before using the key.

## Handling Security Issues

The Talus Labs security team will:

1. Acknowledge receipt within 72 hours;
2. Verify and confirm the issue;
3. Determine affected versions and scope of impact;
4. Conduct audits to find any potential similar and related issues;
5. Prepare fixes for relevant in-production releases;
6. Endeavor to communicate and coordinate with relevant ecosystem stakeholders, including the Nexus communities, at the appropriate times;

Please assist the Talus Labs security team by following these guidelines:

- Allow a reasonable amount of time for the team to respond to and address the issue;
- Avoid exploiting any issues or vulnerabilities that you may become aware of;
- Demonstrate good faith by not disrupting the Talus Labs / Nexus networks, data, services or communities;

_Every effort will be made to handle and address security issues as quickly and efficiently as possible._

## Safe Harbor

Talus Labs is committed to working with security researchers and the broader security community. We believe that responsible security research benefits everyone and helps keep our users safe.

**Legal Safe Harbor**: When conducting vulnerability research in accordance with this policy, we consider such research to be:

- **Authorized** in accordance with applicable computer fraud and abuse laws, and we will not initiate or recommend legal action against you for accidental, good-faith violations of this policy;
- **Exempt** from restrictions in our Terms of Service/Use that would interfere with conducting security research, and we waive those restrictions on a limited basis for work done under this policy;
- **Lawful** and helpful to the overall security of the Internet when conducted in good faith and in compliance with applicable laws.

**Research Guidelines**: To qualify for safe harbor protection, security research must be conducted in good faith, which means:

- You make a good faith effort to avoid privacy violations, destruction of data, and interruption or degradation of Talus Labs services and the Nexus network;
- You do not access, modify, or delete data belonging to others;
- You do not perform attacks that could harm the reliability/integrity of our services or data;
- You do not use social engineering techniques against our employees, contractors, or community members;
- You provide us with reasonable time to address the issue before any disclosure;
- You do not violate any law or breach any agreement in the course of your research.

**Scope**: This safe harbor applies to security research conducted on:
- Talus Labs operated infrastructure and services
- Open source Nexus software and related repositories
- Public-facing websites and applications operated by Talus Labs

If you have questions about whether your research is consistent with this policy, please contact us at [security-reports@taluslabs.xyz](mailto:security-reports@taluslabs.xyz) before proceeding.
