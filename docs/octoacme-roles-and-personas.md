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

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Personas

The following personas expand the core roles to include common operational and cross-functional responsibilities that affect planning, execution, releases, and incident response.

### Delivery Lead

Role Summary
- Coordinates day-to-day delivery activities for multi-team initiatives, ensuring cross-team dependencies are tracked and resolved.

Responsibilities
- Drive cross-team scheduling and timeline alignment
- Track and unblock inter-team dependencies
- Ensure readiness for demos and releases
- Coordinate delivery-level risk mitigation and communications

Typical Decisions
- Prioritize inter-team dependency resolution
- Adjust delivery sequencing to meet milestone commitments

Key Interactions (one-liner)
- Works with PM to track schedule and status; partners with Tech Leads to resolve technical dependencies; syncs with QA on release readiness.

Example handoffs
- Handoff from PM: Delivery scope and milestone dates; Delivery Lead operationalizes the schedule and manages cross-team coordination.
- Handoff to Release Engineer: Confirms release window and dependency list for deployment planning.

---

### Tech Lead

Role Summary
- Technical owner for a code area or feature set who guides architecture, quality, and technical direction.

Responsibilities
- Make architecture and design decisions for the code area
- Define technical standards and review major design changes
- Mentor developers and support technical onboarding
- Estimate effort for complex technical work

Typical Decisions
- Approve or reject major design changes
- Select libraries, frameworks, and patterns for the code area

Key Interactions (one-liner)
- Partners with Developers and Engineering Manager on staffing and estimates; advises PM/PdM on technical trade-offs and delivery risk.

Example handoffs
- Handoff from Developer: Request for design review or approval for significant change; Tech Lead provides guidance and acceptance criteria for implementation.

---

### Engineering Manager

Role Summary
- People and delivery manager responsible for team capacity, hiring, and performance coaching.

Responsibilities
- Capacity planning and resource allocation
- Performance coaching and career development
- Hiring and team structure decisions
- Resolve resourcing conflicts and support retention

Typical Decisions
- Approve team assignments and reallocation of resources
- Decisions about hiring, promotion, and coaching priorities

Key Interactions (one-liner)
- Aligns with PM on resource allocation and delivery risk; works with Tech Leads and Developers on capacity and performance matters.

Example handoffs
- Handoff from PM: Request for additional capacity or staffing changes; Engineering Manager evaluates and commits to resource changes or alternatives.

---

### UX Researcher / Designer

Role Summary
- Owns user research, design validation, and usability decisions to ensure product solutions meet user needs.

Responsibilities
- Conduct user research and usability testing
- Produce designs, prototypes, and interaction specs
- Validate acceptance criteria from a user perspective
- Collaborate on accessibility and UX quality

Typical Decisions
- Finalize UI/UX approaches for features and flows
- Determine sufficiency of research evidence for design choices

Key Interactions (one-liner)
- Works with PdM to shape requirements, with Developers to clarify implementation, and with QA to define UX acceptance checks.

Example handoffs
- Handoff from PdM: Design requirements and user outcomes; Designer provides prototypes and acceptance criteria for implementation and testing.

---

### Release Engineer / CI/CD Owner

RoleSummary
- Maintains build and release pipelines, deployment automation, and rollback mechanisms.

Responsibilities
- Build, maintain, and secure CI/CD pipelines
- Implement deployment strategies (canary, blue/green, feature flags)
- Maintain release automation and rollback procedures
- Improve pipeline performance and reliability

Typical Decisions
- Approve deployment strategies and pipeline changes
- Decide on rollback or mitigation approaches when releases fail

Key Interactions (one-liner)
- Works with Developers and SRE on deployment automation; coordinates with PM for deployment windows and rollback plans.

Example handoffs
- Handoff from Delivery Lead/PM: Confirmed release window and deployment constraints; Release Engineer schedules pipeline changes and release steps.

---

### Site Reliability / Observability Engineer (SRE)

Role Summary
- Ensures system reliability, defines SLOs, and maintains monitoring and alerting to protect production health.

Responsibilities
- Define and maintain SLOs/SLIs and alerting thresholds
- Implement instrumentation and monitoring dashboards
- Participate in on-call rotations and incident response
- Run post-deploy verifications and help triage production issues

Typical Decisions
- Tune alerts and SLO thresholds
- Escalate production incidents and recommend mitigations or rollbacks

Key Interactions (one-liner)
- Collaborates with Developers on instrumentation, with Release Engineer on rollout risk, and with PM on incident impact communications.

Example handoffs
- Handoff from Developers: Instrumentation requests and runbooks; SRE validates monitoring and adds alerts/dashboards.

---

### Support Lead / Customer Success Liaison

Role Summary
- Acts as the voice of the customer post-release, triaging issues and channeling critical feedback into priorities.

Responsibilities
- Triage customer-reported defects and questions
- Provide severity and customer impact context
- Track escalations and coordinate with engineering for fixes
- Communicate status and workarounds to customers

Typical Decisions
- Classify severity of customer issues and escalate appropriately
- Recommend temporary workarounds or prioritization for fixes

Key Interactions (one-liner)
- Feeds critical issues to PM and SRE; helps PdM prioritize fixes based on customer impact.

Example handoffs
- Handoff from Customer Support: Incident report with logs and reproduction steps; Support Lead ensures engineering has required context and priority.

---

### Data Analyst / Insights Partner

Role Summary
- Provides data and analysis to validate impact, track success metrics, and support product decisions.

Responsibilities
- Define instrumentation needs and event schemas
- Build dashboards and reports for success metrics
- Analyze experiments and provide insights
- Advise on measurement strategy and data quality

Typical Decisions
- Approve dashboards and metric definitions
- Determine whether metrics show sufficient signal to inform decisions

Key Interactions (one-liner)
- Works with PdM on success metrics, with Developers on telemetry implementation, and with PM to report progress and outcomes.

Example handoffs
- Handoff from PdM: Desired success metrics and experimental questions; Data Analyst configures dashboards and validates instrumentation.

---

## Review and Next Steps
- Review this expanded section with PM, PdM, Engineering Managers, SRE, and Support stakeholders.
- Add short example handoff checklists to project templates where helpful.
- Link these personas from project READMEs and the Project One-pager to make expectations discoverable.
