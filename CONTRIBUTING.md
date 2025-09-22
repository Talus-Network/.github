# Contributing to Talus Projects

Thank you for considering contributing to Talus! This document outlines our contribution process and standards across all Talus repositories.

## Getting Started

All contributions follow our systematic development process. Please familiarize yourself with:

- **[Discussion Guidelines](https://github.com/Talus-Network/.github/blob/main/DISCUSSIONS.md)** - How to propose and discuss ideas
- **[Improvement Proposal Process](https://github.com/Talus-Network/.github/blob/main/IP_PROCESS.md)** - Our formal proposal and approval workflow
- **Code of Conduct** - Standards for respectful collaboration

## How Ideas Become Features

### 1. Community Discussion (GitHub Discussions)
Start with a discussion to gauge community interest and gather initial feedback. Use our [Discussion Guidelines](link) to structure your proposal effectively.

### 2. Technical RFC (GitHub Discussions - Ideas)
For ideas with community support, create a technical RFC to explore implementation approaches and feasibility.

### 3. Improvement Proposal (GitHub Issues)
Promising RFCs become formal Improvement Proposals following our [IP template](link). All significant changes require IP approval.

### 4. Implementation (Pull Requests)
Approved IPs become implementation epics with specific development tasks.

## Development Standards

### Code Quality
- **Follow established coding style** for the specific project language
- **Write clear, concise commit messages** using [Conventional Commits](https://www.conventionalcommits.org/)
- **Add comprehensive tests** for new functionality
- **Ensure all tests pass** and code quality checks succeed
- **Update documentation** to reflect changes
- **No unsafe code** in Rust projects without explicit justification

### Commit Message Format
```
type(scope): description

- Use present tense ("add feature" not "added feature")
- Use imperative mood ("fix bug" not "fixes bug")
- Reference issues when applicable
- Provide context for the change
```

### Pull Request Process
1. **Link to Epic/Issue**: All PRs must reference the implementing issue/epic
2. **Descriptive Title**: Clear summary of changes
3. **Detailed Description**: What changed and why
4. **Testing Evidence**: Demonstrate changes work as expected
5. **Documentation Updates**: Include any required documentation changes

## Issue Reporting

### Bugs
Use the bug report template to provide:
- Steps to reproduce
- Expected vs actual behavior
- Environment details
- Relevant logs or screenshots

### Feature Requests
Start with a Discussion rather than immediately creating feature request issues. This allows for community input and ensures alignment with project direction.

### Security Issues
**Never report security issues publicly.** Follow our [Security Policy](SECURITY.md) for responsible disclosure.

## Code Review Standards

### For Contributors
- **Keep PRs focused**: One logical change per PR
- **Respond promptly** to review feedback
- **Test thoroughly** before requesting review
- **Be respectful** of reviewer time and feedback

### Review Process
- Maintainers will review within 48-72 hours for active PRs
- Address all review comments before requesting re-review
- At least one maintainer approval required for merge
- Automated checks must pass before merge

## Community Guidelines

### Communication
- **Be respectful** and constructive in all interactions
- **Assume positive intent** from other contributors
- **Ask questions** when something is unclear
- **Help others** learn and improve

### Collaboration
- **Search existing** discussions and issues before creating new ones
- **Provide context** when referencing external information
- **Update status** on work in progress
- **Celebrate successes** and learn from failures

## Repository-Specific Guidelines

Different repositories may have additional requirements:

- **Rust projects**: Use `rustfmt` and address `clippy` warnings
- **Smart contracts**: Follow Sui Move best practices and security guidelines
- **Documentation**: Use clear, accessible language with examples
- **Frontend**: Follow accessibility standards and responsive design principles

Check individual repository README files for specific requirements.

## License and CLA

### Contributor License Agreement
All contributors must sign our Contributor License Agreement (CLA) before contributions can be merged. The CLA assistant will guide you through this process on your first PR.

### Licensing
- Most repositories use **Business Source License 1.1** by default
- Open source projects use **Apache License 2.0**
- Check individual repository LICENSE files for specific terms

## Getting Help

### Community Support
- **GitHub Discussions**: General questions and community support
- **Discord/Telegram**: Real-time community chat (links in project README)
- **Documentation**: Comprehensive guides at [docs.talus.network](https://docs.talus.network)

### Developer Support
- **Technical Questions**: Start with GitHub Discussions
- **Process Questions**: Reference this guide or ask in discussions
- **Urgent Issues**: Follow our incident response procedures

## Recognition

We value all contributions and recognize contributors through:
- Commit attribution and co-authorship
- Contributor acknowledgments in release notes
- Community recognition in discussions and social media

Thank you for contributing to the Talus ecosystem! Your efforts help build the future of decentralized autonomous systems.

---

**Last updated**: 2025-09-22

*This document is maintained by the Talus team and updated as our processes evolve. For questions or suggestions about these guidelines, please open a discussion.*
