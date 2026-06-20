# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Release Manager

### Role Summary
Release Managers coordinate release planning, execution, and rollback procedures. They ensure reliable deployments with clear communication and safe fallback paths.

### Responsibilities
- Schedule and coordinate release windows across teams
- Verify pre-release checklists (smoke tests, runbooks, sign-offs)
- Coordinate communication with stakeholders, support, and operations
- Maintain and execute rollback procedures when needed
- Document release outcomes and post-release metrics

### Goals
- Enable safe, predictable deployments
- Reduce deployment-related incidents and delays
- Maintain clear communication across release teams

### Interactions
- Works with **Project Manager** on release timing and stakeholder coordination
- Works with **Developers** on code readiness and deployment prerequisites
- Works with **QA** on pre-release verification and acceptance testing
- Works with **Platform/DevOps Engineer** on deployment operations and infrastructure readiness
- Works with **Support Lead** on post-release monitoring and escalation procedures

### Typical Communication
- Release schedules and deployment coordination meetings
- Pre-release checklists and approval gates
- Release notes and stakeholder announcements
- Post-release monitoring reports and incident updates

---

## Platform / DevOps Engineer

### Role Summary
Platform/DevOps Engineers maintain CI/CD infrastructure, deployment pipelines, and production environments. They enable reliable, automated delivery and operational excellence.

### Responsibilities
- Build and maintain CI/CD pipelines for automated testing and deployment
- Manage staging and production environments and infrastructure
- Implement deployment automation and reduce manual steps
- Monitor infrastructure health and respond to incidents
- Establish runbooks and standard operating procedures
- Support observability, logging, and alerting

### Goals
- Enable fast, reliable deployments
- Minimize deployment-related incidents and manual toil
- Maintain high system availability and performance

### Interactions
- Works with **Developers** on environment setup, deployment processes, and infrastructure troubleshooting
- Works with **Release Manager** on deployment runbooks and release operations
- Works with **QA** on test environment provisioning and environment configuration
- Works with **Security Champion** on secure infrastructure practices and compliance controls
- Works with **Project Manager** on infrastructure planning and dependency management

### Typical Communication
- Infrastructure status and incident reports
- CI/CD pipeline updates and deployment automation
- Environment setup and maintenance notifications
- Infrastructure capacity and performance metrics

---

## Security Champion

### Role Summary
Security Champions are embedded security advocates within the delivery team who drive secure design, vulnerability triage, and compliance alignment. They own security risk mitigation within the project.

### Responsibilities
- Conduct threat modeling and architecture reviews
- Surface and prioritize security scan findings
- Ensure security gates and checks are in place within CI/CD
- Advise on secure coding practices and design patterns
- Coordinate security incident triage and remediation with the Security team
- Track security-related risks and mitigations

### Goals
- Shift security left by identifying issues early
- Build security awareness and best practices into development
- Reduce security vulnerabilities in production
- Maintain compliance with organizational security policies

### Interactions
- Works with **Developers** on secure implementation and vulnerability remediation
- Works with **Project Manager** on risk communication and mitigation prioritization
- Works with **Product Manager** on prioritization of security fixes vs. features
- Works with **Platform/DevOps Engineer** on secure infrastructure controls
- Escalates to Security team on critical or compliance-related issues

### Typical Communication
- Threat modeling reviews and design guidance
- Security scan reports and remediation tracking
- Security training and awareness sessions
- Risk register updates and incident reports

---

## Data Analyst / Analytics Owner

### Role Summary
Data Analysts own success metrics definition, instrumentation, and measurement. They validate data quality and provide insights to measure project impact.

### Responsibilities
- Define success metrics aligned with business goals
- Specify event schemas and instrumentation requirements
- Validate dashboard accuracy and data quality
- Analyze project impact post-launch (A/B tests, experiments)
- Provide insights and trends for decision-making
- Track KPIs and report on outcomes

### Goals
- Ensure metrics are actionable and connected to business value
- Provide timely, accurate insights for decision-making
- Support data-driven prioritization and iteration

### Interactions
- Works with **Product Manager** on success metrics and outcome measurement
- Works with **Developers** on instrumentation implementation and data accuracy
- Works with **Project Manager** on reporting cadence and stakeholder communication
- Consults with **Business Analyst** on business requirement alignment

### Typical Communication
- Metric specifications and event schemas
- Data dashboards and performance reports
- Experiment results and insights
- Quarterly business reviews (QBRs) and stakeholder updates

---

## UX Researcher / Designer

### Role Summary
UX Researchers and Designers lead user research, validate usability, and ensure user-centered design. They own the quality of user experience across deliverables.

### Responsibilities
- Conduct user research and usability testing
- Translate research into design guidance and acceptance criteria
- Validate design solutions with end users
- Ensure accessibility and usability standards are met
- Provide design assets and implementation guidance to developers
- Track and improve user satisfaction metrics

### Goals
- Ensure features are usable and solve real user problems
- Reduce rework caused by UX misalignment
- Maintain high user satisfaction and adoption

### Interactions
- Works with **Product Manager** on user needs and problem definition
- Works with **Developers** on design specification clarity and implementation details
- Works with **QA** on UX-specific acceptance criteria and testing
- Consults with **Data Analyst** on user satisfaction and engagement metrics

### Typical Communication
- User research findings and insights
- Design specifications and prototypes
- Usability test results and feedback
- User satisfaction and adoption metrics

---

## Support Lead / Customer Success Liaison

### Role Summary
Support Leads are the primary contact for operational user issues and escalations. They triage customer reports, reproduce issues, and bridge communication between support, engineering, and product.

### Responsibilities
- Triage incoming customer issues and bug reports
- Provide initial troubleshooting and reproduction steps
- Track and escalate high-severity incidents
- Maintain support runbooks and FAQs
- Communicate status and resolution timelines to customers
- Capture customer feedback for future improvements
- Monitor post-release stability and performance

### Goals
- Reduce customer impact from issues
- Speed resolution through early triage and escalation
- Build customer trust through responsive communication
- Drive continuous improvement based on customer feedback

### Interactions
- Works with **Project Manager** on incident escalation and status communication
- Works with **Developers** on bug reproduction and fix prioritization
- Works with **Release Manager** on post-release monitoring and stability verification
- Works with **Product Manager** on customer feedback and feature prioritization
- Works with **Platform/DevOps Engineer** on infrastructure-related incidents

### Typical Communication
- Customer issue reports and severity assessments
- Incident escalations and status updates
- Post-incident root cause analysis and follow-ups
- Customer feedback summaries and trends

---

## Business Analyst

### Role Summary
Business Analysts translate stakeholder requirements into clear, actionable backlog items and acceptance criteria. They bridge business needs with technical delivery.

### Responsibilities
- Gather and clarify stakeholder requirements
- Translate requirements into user stories and acceptance criteria
- Map business processes and dependencies
- Maintain traceability between business objectives and backlog
- Facilitate requirements discussions and conflict resolution
- Define scope boundaries and change management

### Goals
- Ensure features deliver intended business value
- Reduce rework from unclear or misaligned requirements
- Maintain clear traceability from strategy to delivery

### Interactions
- Works with **Product Manager** on business objectives and requirement prioritization
- Works with **Project Manager** on scope definition and change management
- Works with **Developers** on technical feasibility and implementation clarity
- Consults with **Data Analyst** on metrics and success criteria

### Typical Communication
- Requirements specifications and user story documents
- Requirements review meetings and walkthroughs
- Scope and change management updates
- Business process documentation and diagrams

---

## Legal / Compliance Liaison

### Role Summary
Legal/Compliance Liaisons ensure that regulatory, contractual, and policy obligations are incorporated into project planning and delivery. They mitigate legal and compliance risk.

### Responsibilities
- Review privacy and data protection implications of features
- Advise on contractual obligations and constraints
- Identify regulatory compliance requirements (e.g., GDPR, HIPAA)
- Approve compliance-critical changes and mitigations
- Establish compliance verification and audit procedures
- Escalate compliance violations or policy breaches

### Goals
- Prevent legal and compliance violations
- Build compliance into the delivery process early
- Maintain organizational risk management standards

### Interactions
- Works with **Project Manager** on compliance planning and risk management
- Works with **Product Manager** on feature compliance and business impact
- Works with **Security Champion** on technical controls and compliance verification
- Works with **Developers** on compliance implementation and audit trails
- Escalates to Legal/Compliance teams on policy interpretation or major changes

### Typical Communication
- Compliance requirement specifications
- Risk assessments and mitigation plans
- Compliance sign-offs and approvals
- Audit and compliance verification reports

---

## Cross-Functional Coordination Summary

The personas above represent a complete delivery ecosystem. Key collaboration patterns include:

- **Planning & Requirements:** Business Analyst → Product Manager → Project Manager → Development team
- **Execution & Quality:** Developers → QA (implicit) → Security Champion → Platform/DevOps → Release Manager
- **Monitoring & Learning:** Support Lead → Data Analyst → Product Manager → Retrospectives
- **Compliance & Risk:** Legal/Compliance Liaison → Security Champion → Project Manager → Risk Register

## How these personas are used in the exercise

- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Reference interaction patterns to understand dependencies and communication flows.
- When addressing a specific problem, consider which personas should be involved and what their perspectives are.
