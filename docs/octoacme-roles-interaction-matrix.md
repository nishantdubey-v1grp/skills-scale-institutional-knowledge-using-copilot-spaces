# OctoAcme Roles Interaction Matrix

## Purpose
Provides a quick reference for how roles interact across the project lifecycle and what they communicate about.

---

## Interaction Matrix

| From Role | To Role | Context | Communication | Frequency |
|-----------|---------|---------|-----------------|----------|
| **Project Manager** | Product Manager | Planning & prioritization | Backlog priorities, timeline, resource constraints | Weekly sync |
| **Project Manager** | Developers | Execution & coordination | Work assignments, blockers, timeline updates | Daily standup |
| **Project Manager** | Release Manager | Release coordination | Release window, go-live criteria, stakeholder comms | Weekly (pre-release daily) |
| **Project Manager** | Support Lead | Incident escalation | Critical issues, status updates, customer comms | As needed |
| **Product Manager** | Developers | Feature definition | Acceptance criteria, success metrics, design intent | Design & refinement |
| **Product Manager** | UX Researcher | User validation | Research findings, design feedback, user needs | Sprint planning & refinement |
| **Product Manager** | Data Analyst | Outcome measurement | Success metrics, dashboard specs, results analysis | Sprint & release cadence |
| **Product Manager** | Business Analyst | Requirements | Business objectives, use cases, success criteria | Planning & refinement |
| **Developer** | QA / Tester | Quality | Code readiness, test cases, acceptance criteria | Continuous |
| **Developer** | Security Champion | Risk mitigation | Code review findings, security scan results, remediation | Continuous |
| **Developer** | Platform/DevOps | Infrastructure | Environment setup, deployment, CI/CD troubleshooting | Daily |
| **Release Manager** | Platform/DevOps | Deployment ops | Deployment procedures, rollback plans, environment readiness | Pre-release |
| **Release Manager** | Support Lead | Post-release | Deployment status, issue triage, customer communication | Release day & post-release |
| **Security Champion** | Developers | Threat mitigation | Security guidance, vulnerability findings, remediation tracking | Continuous |
| **Security Champion** | Platform/DevOps | Infrastructure security | Secure infrastructure practices, compliance controls | Design & planning |
| **Data Analyst** | Product Manager | Measurement | Metric validation, impact analysis, insights | Sprint & release |
| **Data Analyst** | Developers | Instrumentation | Event specs, data accuracy, implementation guidance | Design & planning |
| **Support Lead** | Developers | Bug triage | Issue reproduction, severity assessment, root cause | Incident response |
| **Support Lead** | Product Manager | Customer feedback | Feature requests, pain points, adoption metrics | Monthly review |
| **Business Analyst** | Product Manager | Requirements clarity | Stakeholder requirements, scope definition, trade-offs | Planning & refinement |
| **Business Analyst** | Developers | Implementation clarity | Acceptance criteria, technical approach, scope boundaries | Refinement & sprint |
| **Legal/Compliance** | Project Manager | Risk management | Compliance requirements, approval gates, audit plans | Planning & pre-release |
| **Legal/Compliance** | Security Champion | Technical controls | Compliance verification, technical controls, policy alignment | Design & planning |

---

## Communication Artifacts by Interaction

### Planning & Prioritization
- **Artifacts:** Project Charter, One-pager, Backlog, Roadmap
- **Key Roles:** Project Manager ↔ Product Manager ↔ Business Analyst
- **Cadence:** Weekly sync, sprint planning

### Feature Development & Quality
- **Artifacts:** Acceptance Criteria, Design Specs, Code Reviews, Test Plans
- **Key Roles:** Product Manager → Developers → QA → Security Champion
- **Cadence:** Continuous during sprint

### Risk & Compliance
- **Artifacts:** Risk Register, Threat Models, Compliance Checklist
- **Key Roles:** Project Manager ↔ Security Champion ↔ Legal/Compliance
- **Cadence:** Weekly risk review, pre-release verification

### Release & Deployment
- **Artifacts:** Release Notes, Deployment Checklist, Runbooks, Rollback Plans
- **Key Roles:** Release Manager ↔ Platform/DevOps ↔ Support Lead
- **Cadence:** Daily during release window

### Measurement & Learning
- **Artifacts:** Dashboards, Metrics Reports, Post-Launch Analysis
- **Key Roles:** Data Analyst ↔ Product Manager ↔ Developers
- **Cadence:** Sprint review, monthly QBR

### Customer Feedback & Support
- **Artifacts:** Issue Reports, Customer Feedback Summaries, Support Runbooks
- **Key Roles:** Support Lead ↔ Developers ↔ Product Manager
- **Cadence:** Daily triage, monthly trends

---

## Cross-Functional Workflows

### Workflow 1: Feature Definition to Delivery

```
Business Analyst → gathers requirements
     ↓
Product Manager → defines success metrics & priorities
     ↓
UX Researcher → validates user needs & design
     ↓
Developers → implement with acceptance criteria
     ↓
Security Champion → review code & threat model
     ↓
Data Analyst → instrument for measurement
     ↓
Release Manager → coordinate go-live
     ↓
Support Lead → monitor and triage post-release
     ↓
Data Analyst → measure impact & report results
```

### Workflow 2: Issue Triage to Resolution

```
Support Lead → triages customer report
     ↓
Project Manager → assesses priority & impact
     ↓
Developers → reproduce & diagnose
     ↓
Security Champion → assess if security-related
     ↓
Developers → implement fix
     ↓
Release Manager → schedule patch release
     ↓
Support Lead → verify fix & close with customer
```

### Workflow 3: Risk Identification to Mitigation

```
Project Manager → identifies risk in planning
     ↓
Legal/Compliance → assesses compliance impact
     ↓
Security Champion → assesses security impact
     ↓
Product Manager → prioritizes mitigation
     ↓
Developers → implement mitigations
     ↓
Project Manager → monitor and update risk register
     ↓
Retrospective → capture learnings
```

---

## Quick Reference: Who to Involve When

### You're planning a new initiative
- ✓ Product Manager, Project Manager, Business Analyst, Developers (estimation)

### You're defining success metrics
- ✓ Product Manager, Data Analyst, Business Analyst

### You have a critical bug in production
- ✓ Support Lead, Developers, Release Manager, Project Manager

### You need to review security implications
- ✓ Security Champion, Product Manager, Legal/Compliance Liaison

### You're preparing for a release
- ✓ Release Manager, Platform/DevOps, QA, Project Manager, Support Lead

### You're planning infrastructure changes
- ✓ Platform/DevOps, Security Champion, Project Manager, Developers

### You're resolving a compliance requirement
- ✓ Legal/Compliance, Security Champion, Product Manager, Project Manager

---

## Tips for Effective Cross-Functional Collaboration

1. **Clarify ownership:** Know who owns the decision and who are advisors
2. **Use async-first communication:** Leverage docs and updates to reduce meeting load
3. **Establish escalation paths:** Know when and to whom to escalate
4. **Regular syncs:** Weekly PM + Product sync, daily standups, sprint planning/review
5. **Shared artifacts:** Keep docs updated and accessible in the project repo
6. **Feedback loops:** Retrospectives and post-release reviews to improve collaboration
