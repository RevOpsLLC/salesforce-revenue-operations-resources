# Salesforce Agentforce Readiness Checklist

A practical framework for evaluating whether your organization, Salesforce environment, data, processes, and governance are ready for Agentforce.

Created by [Revenue Ops LLC](https://www.revenueopsllc.com/), a Salesforce consulting partner helping organizations improve Salesforce, Revenue Operations, automation, data, and AI.

---

## What Is Agentforce Readiness?

Successful Agentforce implementations require more than creating an agent.

Before deploying AI into a business process, organizations should understand:

- What business problem the agent should solve
- Which processes the agent will support
- What information the agent needs
- Where that information is stored
- What actions the agent can perform
- Which decisions require human involvement
- How exceptions will be handled
- How security and permissions will be maintained
- How performance will be measured

Use this checklist to evaluate whether the foundation for an Agentforce implementation is in place.

---

# 1. Define the Business Use Case

Start with a specific business problem rather than the technology.

- [ ] Define the business problem
- [ ] Identify the users or customers affected
- [ ] Document the current process
- [ ] Identify current pain points
- [ ] Define the desired future state
- [ ] Identify the expected business value
- [ ] Define measurable success criteria
- [ ] Identify an executive or business owner
- [ ] Establish implementation scope

### Good Agentforce Use Cases

Strong use cases typically involve work that is:

- Repetitive
- Information intensive
- Rules based
- Time consuming
- High volume
- Dependent on information from multiple sources
- Suitable for clearly defined actions

Avoid beginning with:

**"Where can we use AI?"**

Instead ask:

**"Which business process are we trying to improve, and what role should AI play in that process?"**

---

# 2. Document the Current Process

Before introducing an agent, document how the work happens today.

For the target process:

- [ ] Identify the trigger
- [ ] Document each process step
- [ ] Identify required information
- [ ] Identify decision points
- [ ] Identify business rules
- [ ] Identify exceptions
- [ ] Identify approvals
- [ ] Identify systems involved
- [ ] Identify the final outcome
- [ ] Identify process ownership

A useful model is:

**Trigger → Context → Decision → Action → Validation → Outcome**

Agentforce should improve a defined process rather than compensate for an undefined one.

---

# 3. Evaluate Data Readiness

AI requires access to accurate and relevant information.

Evaluate:

- [ ] Data completeness
- [ ] Data accuracy
- [ ] Duplicate records
- [ ] Data consistency
- [ ] Record ownership
- [ ] Data freshness
- [ ] Structured data
- [ ] Unstructured data
- [ ] Historical data
- [ ] Data accessibility

Ask:

- Does the information the agent needs exist?
- Is it accurate?
- Is it current?
- Can Salesforce access it?
- Can the agent access it appropriately?

Poor data quality will limit the value of even a well-designed agent.

---

# 4. Identify Knowledge Sources

Determine what information the agent needs in order to respond or act appropriately.

Potential sources include:

- Salesforce records
- Knowledge articles
- Product documentation
- Policies
- Procedures
- Websites
- Customer information
- Case history
- Sales history
- Data Cloud
- Connected enterprise systems

For each source:

- [ ] Identify the owner
- [ ] Confirm accuracy
- [ ] Confirm accessibility
- [ ] Confirm appropriate permissions
- [ ] Establish maintenance responsibility
- [ ] Determine how frequently information changes

The agent needs governed information, not simply more information.

---

# 5. Evaluate Salesforce Data Architecture

Review whether Salesforce contains the necessary business context.

Evaluate:

- [ ] Accounts
- [ ] Contacts
- [ ] Leads
- [ ] Opportunities
- [ ] Cases
- [ ] Activities
- [ ] Products
- [ ] Orders
- [ ] Contracts
- [ ] Custom objects
- [ ] Object relationships
- [ ] Record ownership

Determine whether the agent can obtain a complete enough picture to perform its intended role.

---

# 6. Evaluate Integrations

Agentforce may need information or actions from systems outside Salesforce.

Identify required systems such as:

- ERP
- Accounting
- Ecommerce
- Marketing automation
- Customer support
- Scheduling
- Inventory
- Order management
- Payment platforms
- Data warehouses

For each integration:

- [ ] Define its business purpose
- [ ] Identify required data
- [ ] Define system of record
- [ ] Confirm integration reliability
- [ ] Define synchronization frequency
- [ ] Define error handling
- [ ] Establish monitoring
- [ ] Confirm security

An agent cannot reliably orchestrate a process if critical system connections are unreliable.

---

# 7. Define Agent Actions

Clearly define what the agent should be allowed to do.

Potential actions might include:

- Retrieve information
- Summarize records
- Answer questions
- Create records
- Update records
- Create tasks
- Route work
- Send communications
- Initiate workflows
- Trigger integrations
- Escalate to a human

For every action:

- [ ] Define when it can occur
- [ ] Define required inputs
- [ ] Define permissions
- [ ] Define validation
- [ ] Define expected outcome
- [ ] Define exceptions
- [ ] Define logging requirements
- [ ] Determine whether human approval is required

---

# 8. Establish Human-in-the-Loop Requirements

Not every decision should be delegated to AI.

Determine where humans should:

- Approve
- Review
- Correct
- Escalate
- Override
- Investigate

A useful pattern is:

**Agent Identifies → Agent Prepares → Human Reviews → Approved Action Occurs**

More autonomous patterns may be appropriate when the process is sufficiently predictable and governed:

**Agent Identifies → Validates → Acts → Logs → Monitors**

For each use case:

- [ ] Define autonomous actions
- [ ] Define approval-required actions
- [ ] Define escalation conditions
- [ ] Define exception handling
- [ ] Define override procedures

---

# 9. Review Security and Permissions

Agentforce should operate within appropriate security boundaries.

Review:

- [ ] User permissions
- [ ] Agent permissions
- [ ] Object access
- [ ] Field-level access
- [ ] Record access
- [ ] Sensitive information
- [ ] Integration credentials
- [ ] External system access
- [ ] Data sharing
- [ ] Audit requirements

Apply least-privilege principles wherever practical.

An agent should have the access required to perform its role, but no more.

---

# 10. Define Guardrails

Establish clear boundaries for agent behavior.

Define:

- [ ] Topics the agent can address
- [ ] Topics the agent should not address
- [ ] Actions the agent can perform
- [ ] Actions requiring approval
- [ ] Prohibited actions
- [ ] Escalation conditions
- [ ] Error handling
- [ ] Customer-facing limitations
- [ ] Compliance requirements

Guardrails should be based on the business risk associated with the use case.

---

# 11. Design Exception Management

Real-world processes contain exceptions.

Identify situations where:

- Required information is missing
- Data conflicts
- A customer request falls outside policy
- An integration fails
- The agent lacks confidence or context
- An action cannot be completed
- Human judgment is required

For each exception:

- [ ] Define detection
- [ ] Define routing
- [ ] Define ownership
- [ ] Define expected response time
- [ ] Define resolution process
- [ ] Define logging

A strong AI implementation does not eliminate exceptions.

It makes exceptions easier to identify, route, and resolve.

---

# 12. Establish AI Governance

Define how Agentforce will be managed after deployment.

Governance should include:

- [ ] Agent ownership
- [ ] Business ownership
- [ ] Technical ownership
- [ ] Change management
- [ ] Testing standards
- [ ] Release management
- [ ] Monitoring
- [ ] Security reviews
- [ ] Documentation
- [ ] Incident management

Treat agents as operational capabilities that require ongoing management.

---

# 13. Define Success Metrics

Establish measurements before deployment.

Potential metrics include:

### Efficiency

- Time saved
- Reduced manual work
- Response time
- Resolution time
- Automation rate

### Quality

- Accuracy
- Completion rate
- Exception rate
- Escalation rate
- Rework

### Adoption

- Agent usage
- User adoption
- Employee satisfaction
- Customer adoption

### Business Outcomes

- Pipeline impact
- Conversion
- Customer satisfaction
- Retention
- Cost reduction
- Revenue impact

Do not measure success only by the number of AI interactions.

Measure whether the underlying business process improved.

---

# 14. Build a Testing Strategy

Agentforce testing should include realistic business scenarios.

Test:

- [ ] Standard scenarios
- [ ] Edge cases
- [ ] Missing information
- [ ] Incorrect information
- [ ] Permission restrictions
- [ ] Integration failures
- [ ] Exceptions
- [ ] Escalations
- [ ] Human handoffs
- [ ] Prohibited requests

Validate both what the agent **should do** and what it **should not do**.

---

# 15. Start With a Controlled Deployment

Avoid trying to automate an entire customer lifecycle in the first release.

Start with:

- A specific use case
- A defined user population
- Clear actions
- Known data sources
- Measurable outcomes
- Appropriate human oversight

Then:

**Deploy → Measure → Learn → Improve → Expand**

---

# Agentforce Readiness Scorecard

Before beginning implementation, confirm that you can answer yes to most of the following:

## Business

- [ ] We have a specific business use case.
- [ ] The current process is documented.
- [ ] The desired outcome is measurable.
- [ ] A business owner has been identified.

## Data

- [ ] Required data exists.
- [ ] Data quality is acceptable.
- [ ] Systems of record are defined.
- [ ] Required information is accessible.

## Process

- [ ] Business rules are documented.
- [ ] Exceptions are understood.
- [ ] Human approval points are defined.
- [ ] Escalation paths are established.

## Technology

- [ ] Required Salesforce functionality exists.
- [ ] Required integrations are available.
- [ ] Integrations are reliable.
- [ ] Security requirements are understood.

## Governance

- [ ] Agent permissions are defined.
- [ ] Guardrails are defined.
- [ ] Monitoring is established.
- [ ] Ownership is established.
- [ ] Change management is established.

## Measurement

- [ ] Baseline performance is understood.
- [ ] Success metrics are defined.
- [ ] Results can be measured.
- [ ] A continuous improvement process exists.

---

# Agentforce Readiness Maturity

Organizations can think about readiness in three stages.

## Crawl

Establish the foundation:

- Document processes
- Improve data quality
- Define systems of record
- Establish governance
- Identify initial use cases
- Define security

## Walk

Deploy controlled use cases:

- Connect required information
- Implement agent actions
- Establish human review
- Monitor outcomes
- Improve exception handling
- Measure performance

## Run

Expand intelligently:

- Increase appropriate autonomy
- Connect additional processes
- Introduce proactive actions
- Use cross-functional context
- Improve analytics
- Continuously optimize agents

The objective should not be maximum autonomy.

The objective should be the appropriate level of autonomy for the process, risk, and business outcome.

---

# Need Help With Agentforce?

[Revenue Ops LLC](https://www.revenueopsllc.com/) helps organizations identify, design, and implement practical Salesforce and AI use cases.

Our services include:

- Salesforce Advisory
- Agentforce Strategy
- Agentforce Implementation
- AI Readiness Assessments
- Salesforce Implementation
- Revenue Operations Consulting
- Data Strategy
- Integration Strategy
- Business Process Automation
- Salesforce Managed Services

Visit **[RevenueOpsLLC.com](https://www.revenueopsllc.com/)** to learn more.

Explore additional [Salesforce and Revenue Operations resources](https://www.revenueopsllc.com/resources/).

---

## About Revenue Ops LLC

Revenue Ops LLC is a Salesforce consulting partner helping organizations connect people, processes, technology, data, automation, and AI.

This checklist is maintained as part of the Revenue Ops LLC collection of open Salesforce and Revenue Operations resources.
