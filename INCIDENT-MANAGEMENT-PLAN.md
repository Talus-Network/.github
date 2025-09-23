# Talus Incident Management Plan

## Table of Contents

- [Goals](#Goals)
- [What is an Incident?](#What-is-an-Incident)
- [Roles and Stakeholders](#Roles-and-Stakeholders)
- [Communication](#Communication)
- [Crisis Management Steps](#Crisis-Management-Steps)
- [Incident Stages](#Incident-Stages)
- [Release Process Integration](#Release-Process-Integration)
- [Postmortem Analysis](#Postmortem-Analysis)
- [Specific Crisis Handling](#Specific-Crisis-Handling)

## Goals

- Provide a framework for effective and timely resolution of incidents affecting Nexus platform and its users
- Minimize bottlenecks and reliance on individual knowledge while resolving incidents
- Maintain effective communication and coordination during incidents
- Provide guidelines for effective documentation and postmortems
- Ensure incident response integrates smoothly with release processes
- Protect user assets and maintain platform integrity

## What is an Incident?

An event qualifies as an incident if one or more of the following is true:

### **Critical Incidents (Immediate Response Required)**

- Any public Nexus service is offline and outage is visible to users
- Loss or unauthorized movement of user funds through Nexus platform
- Known security vulnerability in Nexus protocol or core components
- Smart contract exploit affecting Nexus-deployed contracts
- Leader network failure affecting more than 30% of active leaders
- Data breach affecting user information or platform integrity
- Sui Network issues directly impacting Nexus functionality

### **Major Incident Indicators (Urgent Attention and Monitoring Required)**

- Multiple users consistently reporting unexpected behavior
- Performance degradation affecting majority of platform operations
- External dependency failure requiring immediate attention
- Critical security advisory from upstream dependencies
- Regulatory compliance issues requiring immediate action

### **Minor Incidents (Standard Response)**

- Individual user issues affecting isolated transactions
- Non-critical service degradation with workarounds available
- Documentation or communication issues requiring clarification

## Roles and Stakeholders

### **Incident Commander (IC)**

The person who declares the incident typically assumes the IC role and directs the high-level incident response. The IC role can later be transferred to another member, including for better time zone coordination.

**Responsibilities:**

- Commands and coordinates incident response, delegating roles as needed
- Maintains overall incident state and decision-making authority
- Ensures all communications are recorded in #nexus-incidents Slack channel
- Interfaces with external stakeholders as needed
- Makes final decisions on release process impacts

**Qualifications:** Anyone with sufficient knowledge of Nexus platform and stakeholder responsibilities.

### **Operations Lead (OL)**

Applies operational tools to mitigate or resolve the incident.

**Responsibilities:**

- Leads technical response and resolution efforts
- Coordinates engineering resources for incident response
- Reports progress to IC throughout incident
- Prepares technical portions of postmortem
- Interfaces with Sui Network validators/infrastructure as needed

**Assignment:** Typically assigned from Engineering team by IC.

### **Communications Lead (CL)**

Manages all internal and external communications during incident.

**Responsibilities:**

- Maintains communication across all channels
- Coordinates with community management
- Prepares external communications (with legal approval)
- Manages stakeholder notifications
- Documents communication timeline

**Stakeholder Groups:**

- **Internal Team**: Engineering, Product, Leadership
- **Developer Community**: Tool developers, integrators
- **Users**: Platform users and asset holders
- **External Partners**: Sui Network, oracle providers, integrated platforms
- **Leaders**: Decentralized leader network participants

### **External Stakeholders**

- **Sui Network Validators**: For protocol-level issues
- **Oracle Providers**: For data feed issues
- **Tool Developers**: For integration impacts
- **Security Auditors**: For security-related incidents

## Communication

### **Command Post**

All incident-related communication must occur in **#nexus-incidents** Slack channel, preferably under a single thread with accompanying Slack huddle.

**Communication Hierarchy:**

1. **Slack**: Primary mode for ongoing incident communication
2. **Video Call**: Initial incident evaluation and critical decision points
3. **Phone**: Emergency escalation when Slack unavailable

### **Live Incident State Document**

The IC maintains a living incident document in Notion with concurrent editing capability.

**Required Information:**

- Incident timeline and current status
- Roles and contact information
- Action items and owners
- Decision log with rationale
- External communication log
- Impact assessment and affected systems

**Documentation Standards:**

- Designate note-taker for all calls and meetings
- Link all documentation in master incident folder
- Maintain clear historical record for postmortem analysis
- Track any ongoing support requirements

## Crisis Management Steps

### **1. Identification**

**Recognition:** Individual identifying potential crisis becomes IC initially.

**Initial Assessment:**

- **Severity**: Impact on platform, users, and business operations
- **Timeline**: Incident start time and initial resolution estimate
- **Scope**: Affected systems, users, and stakeholders
- **Release Impact**: Effect on current or planned releases

### **2. Role Assignment**

**IC Responsibilities:**

- Assign Operations Lead (OL) for technical response
- Assign Communications Lead (CL) for stakeholder management
- Maintain overall coordination and decision authority

### **3. Stakeholder Notification**

**Internal Escalation:**

- Leadership Team (immediate for Critical incidents)
- Engineering Team (as directed by OL)
- Product Team (for user-facing impacts)

**External Notification (as appropriate):**

- Sui Network validators
- Oracle providers
- Developer community
- Platform users

## Incident Stages

### **Stage 1: Immediate Response**

**Objectives:**

- Contain and assess the incident
- Prevent further damage or exposure
- Establish communication channels

**Actions:**

1. **Containment**: Remove or isolate crisis indicators if necessary
2. **Assessment**: Determine scope, impact, and required resources
3. **Communication Setup**: Establish incident channels and stakeholder contacts
4. **Release Process Check**: Assess impact on current releases

### **Stage 2: Investigation and Planning**

**Objectives:**

- Understand root cause and extent of incident
- Develop resolution plan with clear action items
- Coordinate resources and timeline

**Actions:**

1. **Root Cause Analysis**: Technical investigation led by OL
2. **Resource Coordination**: Identify required engineering and external resources
3. **Communication Strategy**: Prepare internal and external messaging
4. **Release Coordination**: Determine if emergency release required

### **Stage 3: Resolution Execution**

**Objectives:**

- Execute resolution plan
- Monitor progress and adjust as needed
- Maintain stakeholder communication

**Actions:**

1. **Technical Resolution**: Implement fixes, patches, or workarounds
2. **Progress Communication**: Regular updates to stakeholders
3. **Release Integration**: Execute emergency releases if required
4. **Validation**: Confirm incident resolution and system stability

### **Stage 4: Recovery and Communication**

**Objectives:**

- Restore normal operations
- Communicate resolution to affected parties
- Begin postmortem process

**Actions:**

1. **System Validation**: Confirm all systems operating normally
2. **Stakeholder Notification**: Inform affected parties of resolution
3. **Documentation**: Complete incident documentation
4. **Handoff**: Transition from incident mode to normal operations

## Release Process Integration

### **Emergency Release Triggers**

Incidents may trigger emergency releases for:

- Critical security patches
- Upstream dependency updates
- Platform vulnerability fixes
- Smart contract upgrades

### **Emergency Release Process**

When incident requires immediate release:

1. **IC Decision**: IC determines if emergency release required
2. **Simplified Epic**: Create emergency epic with abbreviated checklist:
    - [ ]  **Incident Response Reference** *(link to incident documentation)*
    - [ ]  **Security Review** *(expedited review for security fixes)*
    - [ ]  **Critical Testing** *(focused testing on fix functionality)*
    - [ ]  **Emergency Deployment** *(streamlined deployment process)*
    - [ ]  **Communication** *(coordinate with incident CL)*
3. **Accelerated Timeline**: Standard quality gates with compressed timelines
4. **Documentation**: All emergency changes documented in incident postmortem
5. **Follow-up**: Normal release process for any additional work identified

### **Ongoing Release Impact**

For incidents affecting current releases:

- **Testing Phase**: Pause testing, assess incident impact, resume with modified plan
- **Pre-Release**: Evaluate if incident affects release readiness
- **Post-Release**: Monitor for incident-related issues in new deployment

## Postmortem Analysis

### **Postmortem Meeting**

**Timing**: Within 5 business days of incident resolution
**Leadership**: IC and OL
**Participants**: All incident responders and affected stakeholders

**Agenda:**

1. Incident timeline and response effectiveness
2. Root cause analysis and contributing factors
3. Response process evaluation and improvements
4. Action items to prevent recurrence
5. Release process improvements (if applicable)

### **Postmortem Documentation**

**Internal Report Includes:**

- Detailed incident timeline
- Technical root cause analysis
- Response effectiveness assessment
- Process improvement recommendations
- Cost and impact analysis

**Community Communication** (CL prepares, Legal reviews):

- Sanitized incident overview
- User impact summary
- Resolution steps taken
- Preventive measures implemented
- Transparency without compromising security

## Specific Crisis Handling

### **Smart Contract Exploit**

**Activation:**

1. Notify management team and security advisors
2. Pull in smart contract auditors and security experts
3. Assess severity and potential fund exposure

**Response:**

1. Isolate affected contracts if possible
2. Coordinate with Sui Network for any protocol-level response needed
3. Prepare emergency contract updates or migration
4. Document all fund movements and affected users

**Conclusion:**

1. Deploy fixed contracts through emergency release process
2. Coordinate user fund recovery if applicable
3. Legal-reviewed public disclosure
4. Enhanced security measures implementation

### **Leader Network Failure**

**Activation:**

1. Assess leader network status and failure scope
2. Determine if centralized fallback required
3. Coordinate with affected leader operators

**Response:**

1. Implement fallback mechanisms to maintain service
2. Diagnose and resolve leader network issues
3. Coordinate leader network restoration
4. Monitor network stability during recovery

**Conclusion:**

1. Restore full decentralized operation
2. Analyze failure modes and improve resilience
3. Update leader network documentation and procedures

### **Upstream Dependency Security Advisory**

**Activation:**

1. Assess security advisory impact on Nexus platform
2. Determine if immediate action required
3. Coordinate with dependency maintainers

**Response:**

1. Evaluate patch urgency and compatibility
2. Test patches in isolated environment
3. Prepare emergency release if critical
4. Coordinate deployment timing

**Conclusion:**

1. Deploy updated dependencies
2. Validate platform security post-update
3. Document dependency management improvements

### **Data Breach**

**Activation:**

1. Immediately notify management and legal teams
2. Isolate affected systems
3. Assess scope of data exposure

**Response:**

1. Contain breach and secure systems
2. Conduct forensic analysis
3. Prepare legal notifications as required
4. Coordinate with law enforcement if necessary

**Conclusion:**

1. Implement additional security measures
2. Complete legal notification requirements
3. Provide user guidance and support
4. Enhanced monitoring and security procedures

### **Sui Network Protocol Issues**

**Activation:**

1. Monitor Sui Network status and validator communications
2. Assess impact on Nexus platform operations
3. Coordinate with Sui Network incident response

**Response:**

1. Implement platform-level mitigations if possible
2. Coordinate with Sui validators for protocol fixes
3. Prepare user communications about service impact
4. Monitor Sui Network recovery progress

**Conclusion:**

1. Restore full platform functionality
2. Document Sui Network dependency risks
3. Evaluate additional platform resilience measures
