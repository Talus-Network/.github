# Improvement Proposal (IP) Process for FDD-Release Framework

## Overview

This process serves as the **Architecture Pipeline** in our FDD-Release framework, providing the formal mechanism for evaluating and approving changes before they enter the Feature Pipeline. It supports **dual-stream input**: internal strategic planning (Notion) and external community contributions (GitHub Discussions), both converging at formal IP creation on GitHub.

## Dual-Stream Architecture

### **Internal Stream (Private)**

**Strategic initiatives** → **Notion RFC** → **GitHub IP**

### **External Stream (Public)**

**Community ideas** → **GitHub Discussion** → **GitHub RFC** → **GitHub IP**

### **Convergence Point**

**All streams** → **GitHub IP Issue** → **Epic Creation**

## Process Phases

### **Phase 1: Input Stream Initiation**

### **Stream A: Internal Strategic Initiation (Notion-based)**

**Location**: Notion

**Participants**: Leadership Team, Product, Strategy

**Purpose**: Internal strategic evaluation and planning

### **1A.1 Strategic RFC Creation**

- **Trigger**: Strategic need identified by Leadership/Product/Business teams
- **Format**: Notion RFC template with strategic context
- **Content**:
    - Problem statement and strategic rationale
    - High-level value proposition
    - Business impact assessment
    - Resource implications (high-level)
- **Outcome**: Go/No-go decision for formal IP creation

### **1A.2 Strategic Review**

- **Reviewers**: Leadership Team (CEO, CTO, CSO, Head of Product)
- **Criteria**:
    - **Strategic Fit**: Alignment with company objectives and roadmap
    - **Business Case**: Clear value proposition and priority relative to other initiatives
    - **Resource Feasibility**: High-level assessment of required investment
- **Outcomes**:
    - ✅ **Approved for IP Creation** → Proceed to Phase 2
    - 🔄 **Needs Refinement** → Return to strategic RFC
    - ❌ **Rejected** → Document rationale, archive

### **Stream B: External Community Initiation (GitHub-based)**

**Location**: GitHub Discussions

**Participants**: Community, Maintainers, Engineering

**Purpose**: Community-driven idea development and technical exploration

### **1B.1 Community Discussion**

- **Trigger**: Community member identifies need/opportunity
- **Location**: GitHub Discussions → General category
- **Format**: Following [Discussion Contributing Guidelines](https://www.notion.so/taluslabs/link)
- **Content**:
    - Problem statement with community context
    - Real-world examples and use cases
    - Open-ended questions for community input
- **Outcome**: Community consensus on problem importance

### **1B.2 Technical RFC (if warranted)**

- **Trigger**: Discussion shows significant community support
- **Location**: GitHub Discussions → Ideas category
- **Format**: Technical RFC with implementation focus
- **Content**:
    - Reference to original community discussion
    - Technical problem statement
    - Proposed technical approach
    - Initial feasibility assessment
- **Outcome**: Technical direction and community validation

### **Phase 2: Convergence & Formal IP Creation (GitHub)**

**Location**: GitHub Issues

**Participants**: All stakeholders

**Purpose**: Single formal evaluation process regardless of origin

### **2.1 Formal IP Issue Creation**

- **Trigger**:
    - Strategic RFC approval (Internal Stream), OR
    - Productive technical RFC discussion (External Stream)
- **Location**: GitHub Issues
- **Template**: IP Issue Template (below)
- **Tags**: `proposal`, `draft` (initially)
- **Content**:
    - **Internal Origin**: Reference to strategic RFC and business context
    - **External Origin**: Reference to community discussion and RFC
    - **Both**: Complete IP evaluation criteria addressed

### **2.2 Technical Review & Evaluation**

- **Reviewers**: CTO, Technical Leads, relevant Engineering teams
- **Criteria** (same for both streams):
    - **Technical Feasibility**: Can we build this with acceptable risk?
    - **Impact Assessment**: What are the technical consequences?
    - **Implementation Complexity**: Resource and timeline estimates
    - **Security & Risk**: Technical risks and mitigation strategies
- **Process**:
    1. Discussion on GitHub issue with structured comments
    2. Add `details` tag if detailed design needed
    3. Provide detailed design (in issue or external doc)
    4. **Comment Resolution Process** (see below)
    5. Add `final` tag only when all comments resolved

### **Phase 3: Final Approval (Cross-functional)**

**Location**: Both Notion (decision) and GitHub (implementation)

**Participants**: Full Leadership Team

**Purpose**: Final go/no-go decision with full context

### **3.1 Comprehensive Review**

- **Input**: Strategic RFC (Notion) + Technical IP (GitHub)
- **Reviewers**: Leadership Team
- **Prerequisites**: **All comments resolved** (GitHub + Notion discussions)
- **Criteria**: All four IP criteria assessed:
    - ✅ **Functional Feasibility**: Value proposition validated
    - ✅ **Strategic Fit**: Alignment confirmed
    - ✅ **Technical Feasibility**: Implementation plan approved
    - ✅ **Impact**: Downstream effects acceptable

### **3.2 Decision & Documentation**

- **Outcomes**:
    - ✅ **Accepted** → Tag as `accepted`, create Epic
    - ❌ **Rejected** → Tag as `rejected`, document rationale
- **Documentation**:
    - Decision recorded in both Notion and GitHub
    - Rationale clearly documented for future reference
    - If accepted, Epic creation triggered

## IP Issue Template

```markdown
# IP-[YYYY-MM-DD]: [Proposal Title]

## Origin & Context
**Source Stream**: [Internal Strategic RFC | External Community Discussion]
**Strategic RFC**: [Link to Notion RFC if internal origin]
**Community Discussion**: [Link to GitHub Discussion if external origin]
**Technical RFC**: [Link to GitHub RFC if applicable]
**Business Driver**: [Problem this solves]
**Strategic Priority**: [High/Medium/Low]

## Proposal Summary
[Brief description of what you're proposing]

## Functional Feasibility
### Core Value Proposition
- [What value does this deliver?]
- [Who benefits and how?]

### Operational Considerations
- [How does this affect operations?]
- [What new processes or capabilities needed?]

### Economic Impact
- [Development cost estimates]
- [Operational cost implications]
- [Revenue/value generation potential]

### Legal Considerations
- [Regulatory implications]
- [Compliance requirements]
- [IP or licensing considerations]

## Strategic Fit
### Alignment with Objectives
- [How does this support current strategic goals?]
- [Priority relative to other initiatives]

### Resource Requirements
- [Engineering effort required]
- [Other team involvement needed]
- [Timeline estimates]

## Technical Feasibility
### Technical Requirements
- [Core technical components needed]
- [Technology stack implications]
- [Performance requirements]

### Dependencies
- [What does this depend on?]
- [Blocking factors or prerequisites]
- [Timeline impact of dependencies]

### Security & Risk Assessment
- [Security implications]
- [Technical risks and mitigation]
- [Failure scenarios and contingencies]

## Impact Assessment
### Downstream Dependencies
- [What systems/processes will be affected?]
- [Breaking changes or migration needs]
- [User impact and communication needs]

### Technical Debt
- [New technical debt introduced]
- [Existing technical debt addressed]
- [Long-term maintenance implications]

### Integration Requirements
- [How does this integrate with existing systems?]
- [API changes or new interfaces needed]
- [Documentation and training requirements]

## Implementation Plan (if detailed design requested)
[Detailed technical design and implementation approach]

## Success Metrics
- [How will we measure success?]
- [What metrics will we track?]

## Related Issues/Proposals
- [Links to related IPs or issues]
- [Dependencies on other proposals]

---

## Review Status
- [ ] Strategic Review Complete *(internal RFCs only)*
- [ ] Community Consensus Achieved *(external discussions only)*
- [ ] Technical Review Complete *(all GitHub comments resolved)*
- [ ] Comment Resolution Verified *(review team confirmation)*
- [ ] Final Approval Pending

## Tags
`proposal` `draft` <!-- Remove draft when ready for review -->
<!-- Add `details` if detailed design needed -->
<!-- Add `final` when ready for final review -->
<!-- Add `accepted` or `rejected` after final decision -->
```

## Comment Resolution Process

### **Purpose**

Comments drive the proposal evaluation process and ensure thorough review. **Open comments must be resolved before a proposal can be finalized.** This maintains quality and prevents important concerns from being overlooked.

### **Comment Types & Handling**

### **Strategic Comments (Notion-based)**

- **Business Case Questions**: Clarifications on value proposition or strategic fit
- **Resource Concerns**: Questions about timeline, budget, or team allocation
- **Priority Challenges**: Discussions about relative importance vs other initiatives

### **Technical Comments (GitHub-based)**

- **Implementation Questions**: Technical approach or feasibility concerns
- **Security Issues**: Risk identification and mitigation strategies
- **Integration Concerns**: Impact on existing systems or architecture
- **Performance Questions**: Scalability, efficiency, or resource utilization

### **Resolution Responsibilities**

### **Comment Author Responsibilities**

- **Open comments constructively**: Provide specific, actionable feedback
- **Close own comments**: Author is responsible for determining when their concern is addressed
- **Engage in discussion**: Participate actively in resolution efforts
- **Escalate when needed**: Flag complex issues requiring review sessions

### **Proposal Author Responsibilities**

- **Address comments promptly**: Respond within 48 hours during active review
- **Provide detailed responses**: Don't dismiss concerns—address them substantively
- **Update proposal content**: Incorporate feedback into proposal when appropriate
- **Request clarification**: Ask for specifics if comments are unclear

### **Review Team Responsibilities**

- **Monitor comment resolution**: Ensure progress is being made
- **Facilitate discussions**: Help resolve deadlocks or misunderstandings
- **Enforce standards**: Don't allow premature comment closure
- **Schedule review sessions**: Organize meetings for complex issues

### **Comment Resolution Workflow**

### **1. Comment Creation**

```
Comment Author:
1. Creates specific, actionable comment
2. Tags relevant reviewers if needed
3. Clearly states concern or question
```

### **2. Response & Discussion**

```
Proposal Author:
1. Acknowledges comment within 48 hours
2. Provides detailed response or requests clarification
3. Updates proposal if needed
4. Requests comment closure when addressed

Community:
1. Provides additional context or perspectives
2. Helps clarify technical or strategic points
3. Suggests alternative approaches
```

### **3. Comment Resolution**

```
Comment Author (ONLY):
1. Reviews response and updated proposal
2. Confirms concern is adequately addressed
3. Closes comment with resolution note
4. OR explains why concern remains unresolved
```

### **Complex Comment Escalation**

### **Triggers for Review Sessions**

- Comment thread exceeds 10 exchanges without resolution
- Technical disagreement between experts
- Strategic conflict requiring leadership decision
- Cross-functional coordination needed
- Timeline impact of unresolved comments

### **Review Session Process**

1. **Schedule**: Proposal author or reviewer requests session
2. **Participants**: Comment authors, proposal author, relevant experts
3. **Agenda**: Focus specifically on unresolved comments
4. **Outcome**: Clear resolution path or escalation decision
5. **Documentation**: Session notes added to proposal

### **Escalation Levels**

```
Level 1: Peer Review Session
- Technical leads + proposal author
- Focus on technical resolution

Level 2: Cross-Functional Review
- Multiple department leads
- Strategic and technical alignment

Level 3: Leadership Decision
- Leadership team final arbitration
- Used sparingly for deadlocked issues

```

### **Quality Standards**

### **Do NOT Close Comments When:**

- ❌ Response doesn't actually address the concern
- ❌ "We'll figure it out later" without concrete plan
- ❌ Proposal author asks you to close without resolution
- ❌ Concern is dismissed rather than addressed
- ❌ Technical debt is acknowledged but not mitigated

### **DO Close Comments When:**

- ✅ Concern is substantively addressed in proposal updates
- ✅ Alternative approach adequately mitigates the risk
- ✅ Additional context shows concern is not applicable
- ✅ Explicit mitigation strategy is documented
- ✅ Follow-up work is clearly defined and tracked

### **Process Gates**

### **Cannot Add `final` Tag Until:**

- All strategic comments in Notion are resolved
- All technical comments in GitHub are resolved
- Review sessions for complex issues are completed
- Proposal updates incorporate substantive feedback

### **Cannot Approve Proposal Until:**

- `final` tag has been applied
- Comment resolution is verified by review team
- No open threads remain in either Notion or GitHub

### **Tracking & Transparency**

### **Comment Status Tracking**

```
GitHub Issue Comments:
- Use 👍 reaction when concern is addressed
- Comment author confirms with "Resolved: [brief reason]"
- Proposal author summarizes resolution in proposal update

Notion Comments:
- Use comment resolution features
- Document resolution rationale
- Reference in strategic approval decision

```

### **Resolution Summary**

Before final approval, proposal author provides:

- **Comments Addressed**: Count and brief summary
- **Key Changes Made**: How proposal evolved based on feedback
- **Outstanding Risks**: Any concerns accepted but not mitigated

This ensures robust evaluation while maintaining forward momentum and preventing process paralysis.

### **IP → Epic Transition**

When IP is **accepted**:

1. **Epic Creation**: Use Epic Template with IP reference
2. **Pre-Implementation Checklist**: IP approval covers:
    - ✅ Product Design Review (Strategic RFC)
    - ✅ Architectural Review (Technical RFC)
    - ✅ Finalized Specifications (IP Issue)
3. **Feature Pipeline**: Epic enters implementation phase

### **Traceability Chain**

```
Strategic Need (Notion)
    ↓
Strategic RFC (Notion)
    ↓
Technical RFC (GitHub Discussions)
    ↓
IP Issue (GitHub Issues)
    ↓
Epic (GitHub Projects)
    ↓
Implementation Issues (GitHub Issues)
    ↓
Release (GitHub Releases)
```

## Notion ↔ GitHub Integration

### **Current State (Internal Focus)**

- **Strategic planning**: Notion-based
- **Technical evaluation**: GitHub-based
- **Cross-references**: Links between systems
- **Decision authority**: Leadership Team using both contexts

### **Future State (Public Contributions)**

- **External RFCs**: GitHub Discussions only
- **Internal strategic evaluation**: Notion assessment of external proposals
- **Unified technical process**: All technical evaluation on GitHub
- **Single source of truth**: GitHub becomes primary with Notion as strategic overlay

## Advantages of This Approach

### **1. Respects Current Workflow**

- Strategic teams continue using Notion
- Technical teams continue using GitHub
- Clear handoff points between phases

### **2. Prepares for Public Contributions**

- GitHub-based technical process ready for external contributors
- Strategic evaluation layer protects internal priorities
- Clean separation between public technical discussion and internal business decisions

### **3. Maintains Single Source of Truth**

- Each phase has clear ownership and location
- Cross-references maintain traceability
- Decision rationale captured in both systems

### **4. Integrates with FDD-Release**

- IP process = Architecture Pipeline
- Clear transition to Feature Pipeline via Epic creation
- Release checklist references IP completion

## Migration Strategy

### **Phase 1: Internal Implementation**

- Implement full IP process for internal proposals
- Establish Notion ↔ GitHub workflow
- Train teams on process and templates

### **Phase 2: Selective Public Opening**

- Open specific technical areas for external RFC
- Maintain strategic evaluation internally
- Test public contribution workflow

### **Phase 3: Full Public Process**

- Open full technical contribution process
- GitHub becomes primary system
- Notion becomes strategic oversight layer

## Private Development Support

### **Non-Public Development Requirements**

For development that cannot be public during implementation:

1. **Repository Forking**: Create private fork of relevant repository
2. **Private IP Process**: Follow same IP process in private fork
3. **Documentation Tracking**: Maintain ADRs and documentation in private fork
4. **Release Coordination**:
    - Push development branch to public repository when ready
    - Transfer IP documentation as part of release epic
    - Update public documentation to reflect new features
    - Maintain traceability from private IP to public release

### **Private-to-Public Transition**

- **Documentation Task**: Include IP transfer in release epic checklist
- **Community Communication**: Announce new features with reference to transferred IP
- **Historical Continuity**: Maintain decision rationale even when moving from private to public

This approach ensures consistent process regardless of development visibility while protecting sensitive development when necessary.

---

**Last updated**: 2025-09-22

*This process is regularly reviewed and updated to reflect our evolving practices and organizational needs.*

