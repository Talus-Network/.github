# Talus Labs Security Policy

This document describes the Talus Labs security team's process for handling security issues across all Talus repositories and services.

## Reporting Security Issues

**IMPORTANT:** Please DO NOT open public issues for security-related matters or discuss them in public forums or on social media.

### Primary Reporting Methods

#### Email (Recommended)
Report security issues to: **[security-reports@taluslabs.xyz](mailto:security-reports@taluslabs.xyz)**

Include these details in your report:
- **Your information**: Name and affiliation (if applicable)
- **Technical description**: Detailed issue explanation with reproduction steps
- **Impact assessment**: Who can exploit this and what the implications may be
- **Visibility status**: Whether this vulnerability is public or known to third parties
- **Supporting evidence**: Relevant logs, screenshots, or proof-of-concept (if safe to share)

#### GitHub Private Vulnerability Reporting
For repository-specific issues, use GitHub's private vulnerability reporting:
1. Navigate to the repository's "Security" tab
2. Click "Report a vulnerability" under Security Advisories
3. Complete the form with detailed information

See [GitHub's documentation](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing/privately-reporting-a-security-vulnerability) for more information.

### Encrypted Communication

For sensitive reports, use our PGP public key:
- **Download**: [https://talus.network/security-pgp-key.txt](https://talus.network/security-pgp-key.txt)
- **Key Server**: [keys.openpgp.org](https://keys.openpgp.org)
- **Fingerprint**: `103391C9AE4BE87A85E3EFAE2D4462A29BAB94AE`

**Always verify the fingerprint before using the key.**

## Our Response Process

The Talus Labs security team will:

1. **Acknowledge receipt** within 72 hours
2. **Verify and assess** the reported vulnerability
3. **Determine scope** including affected versions and impact assessment
4. **Audit for similar issues** to prevent related vulnerabilities
5. **Develop fixes** for all affected production releases
6. **Coordinate disclosure** with ecosystem stakeholders when appropriate
7. **Deploy fixes** following our emergency release procedures
8. **Publish advisories** once fixes are deployed and users can update

### Timeline Expectations
- **Initial response**: Within 72 hours
- **Severity assessment**: Within 5 business days
- **Fix development**: Varies by complexity, communicated during assessment
- **Public disclosure**: After fixes are available and reasonable time for adoption

## Incident Response Integration

Security issues may trigger our [Incident Management Plan](https://www.notion.so/taluslabs/Incident-Management-Plan-25e7a61d1baa80498736f5ece8e58ece), particularly for:
- Active exploits affecting user funds or data
- Platform-wide vulnerabilities
- Critical infrastructure compromises

In such cases, response times may be accelerated and additional coordination procedures activated.

## Researcher Guidelines

Please help us handle security issues effectively by:

### Responsible Disclosure
- **Allow reasonable time** for our team to respond and address issues
- **Coordinate disclosure timing** to ensure users can protect themselves
- **Provide clear communication** throughout the process

### Research Ethics
- **Avoid exploitation** of discovered vulnerabilities
- **Demonstrate good faith** by not disrupting services, data, or communities
- **Respect privacy** and avoid accessing user data
- **Follow applicable laws** in your research activities

## Safe Harbor Policy

Talus Labs is committed to working constructively with security researchers and the broader security community.

### Legal Protection
When conducting vulnerability research according to this policy, we consider such research to be:

- **Authorized** under applicable computer fraud and abuse laws
- **Exempt** from Terms of Service restrictions that would interfere with security research
- **Lawful and beneficial** when conducted in good faith and compliance with applicable laws

### Research Scope
This safe harbor applies to security research on:
- **Talus Labs infrastructure** and operated services
- **Nexus platform** and related open source software
- **Public-facing applications** and websites operated by Talus Labs
- **Smart contracts** deployed by Talus Labs

### Good Faith Requirements
To qualify for safe harbor protection, research must:
- **Avoid privacy violations** and data access/modification
- **Prevent service disruption** or data destruction
- **Exclude social engineering** against employees or community members
- **Provide reasonable disclosure time** before any public disclosure
- **Comply with applicable laws** and agreements

## Scope and Exclusions

### In Scope
- **Platform vulnerabilities**: Nexus protocol and infrastructure
- **Smart contract issues**: Logic flaws, economic exploits, access control
- **Infrastructure security**: API endpoints, authentication, data handling
- **Dependency vulnerabilities**: Third-party library issues affecting our services
- **Configuration issues**: Misconfigurations leading to security exposure

### Out of Scope
- **Social engineering** attacks on staff or users
- **Physical security** of office locations
- **Distributed denial of service (DDoS)** attacks
- **Spam or content-based** attacks
- **Issues in third-party** services not controlled by Talus Labs

## Recognition and Rewards

From time to time we may operate formal bug bounty programs. We may publish these on our web site, social media or other formal communication channels.

We recognize valuable security research through:
- **Public acknowledgment** in security advisories (with your permission)
- **Direct communication** with our security team
- **Community recognition** when appropriate
- **Swag and merchandise** for significant contributions

## Questions and Support

For questions about this security policy or the reporting process:
- **Email**: [security-reports@taluslabs.xyz](mailto:security-reports@taluslabs.xyz)
- **General security discussions**: Use GitHub Discussions in relevant repositories

---

**Last updated**: 2025-09-22
**Version**: 2.0

*This policy is regularly reviewed and updated to reflect our evolving security practices and community needs.*
