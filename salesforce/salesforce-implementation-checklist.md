# Salesforce Implementation Checklist

A practical Salesforce implementation checklist for planning, designing, building, testing, deploying, and optimizing a Salesforce CRM implementation.

Created by [Revenue Ops LLC](https://www.revenueopsllc.com/), a Salesforce consulting partner specializing in Salesforce advisory, implementation, and managed services.

---

## How to Use This Checklist

A successful Salesforce implementation starts with the business, not the technology.

Before configuring objects, fields, flows, reports, or integrations, organizations should understand:

- What business processes Salesforce needs to support
- Who will use Salesforce
- What information users need
- What information needs to be captured
- How work moves between teams
- What should be automated
- What systems need to integrate with Salesforce
- How success will be measured

Use this checklist as a framework for your Salesforce implementation project.

---

# 1. Define Business Objectives

Before beginning configuration, document why the organization is implementing or changing Salesforce.

- [ ] Define the primary business objectives
- [ ] Identify the business problems Salesforce should solve
- [ ] Identify executive sponsors
- [ ] Identify project stakeholders
- [ ] Define project scope
- [ ] Define what is explicitly out of scope
- [ ] Establish measurable success criteria
- [ ] Identify project risks and dependencies
- [ ] Establish a project governance process
- [ ] Define how decisions will be made

### Questions to Answer

- What should Salesforce enable the business to do that it cannot do today?
- What processes are currently inefficient?
- Where are employees relying on spreadsheets or manual work?
- What information is difficult to access?
- What business decisions require better data?
- What would make this implementation successful six months after launch?

---

# 2. Document the Customer Lifecycle

Salesforce should support the organization's actual customer lifecycle.

Document the lifecycle from initial engagement through ongoing customer relationships.

A simplified lifecycle might look like:

**Lead → Qualification → Opportunity → Quote → Customer → Delivery → Billing → Payment → Retention → Expansion**

- [ ] Document the complete customer lifecycle
- [ ] Identify each lifecycle stage
- [ ] Define entry criteria for each stage
- [ ] Define exit criteria for each stage
- [ ] Identify process owners
- [ ] Identify handoffs between departments
- [ ] Identify required information at each stage
- [ ] Identify exceptions and alternate paths
- [ ] Identify reporting requirements

---

# 3. Conduct Process Discovery

Do not automate a process until you understand it.

Document the current-state process before designing the future state.

- [ ] Interview key stakeholders
- [ ] Interview frontline users
- [ ] Document current processes
- [ ] Identify manual activities
- [ ] Identify duplicate data entry
- [ ] Identify spreadsheet-based processes
- [ ] Identify bottlenecks
- [ ] Identify approval requirements
- [ ] Identify process exceptions
- [ ] Identify unnecessary steps
- [ ] Design the future-state process

For each process, document:

**Trigger → Activities → Decisions → Exceptions → Outcome**

---

# 4. Define Salesforce Architecture

Determine how Salesforce will represent the business.

Common Salesforce objects may include:

- Leads
- Accounts
- Contacts
- Opportunities
- Products
- Quotes
- Contracts
- Cases
- Campaigns
- Custom Objects

For each object:

- [ ] Define its business purpose
- [ ] Define who creates records
- [ ] Define who owns records
- [ ] Define required fields
- [ ] Define relationships with other objects
- [ ] Define lifecycle/status values
- [ ] Define validation requirements
- [ ] Define automation requirements
- [ ] Define reporting requirements
- [ ] Define security requirements

Avoid creating custom objects or fields until there is a clear business requirement for them.

---

# 5. Design the Data Model

A scalable Salesforce implementation requires a deliberate data model.

- [ ] Identify core business entities
- [ ] Define relationships between entities
- [ ] Identify systems of record
- [ ] Define unique identifiers
- [ ] Establish naming conventions
- [ ] Define required fields
- [ ] Identify duplicate prevention requirements
- [ ] Define data retention requirements
- [ ] Establish data ownership
- [ ] Document the data model

Ask:

**Where should this information live, who owns it, and which system is authoritative?**

---

# 6. Assess Data Quality

Migrating bad data into Salesforce creates problems immediately.

Before migration:

- [ ] Profile existing data
- [ ] Identify duplicate records
- [ ] Identify incomplete records
- [ ] Identify invalid data
- [ ] Standardize formats
- [ ] Normalize picklist values
- [ ] Identify obsolete records
- [ ] Establish deduplication rules
- [ ] Determine what data should not be migrated
- [ ] Validate record ownership

Data migration should be treated as a business workstream, not simply a technical task.

---

# 7. Plan Data Migration

Create a documented migration strategy.

- [ ] Identify source systems
- [ ] Identify objects to migrate
- [ ] Map source fields to Salesforce fields
- [ ] Define transformation rules
- [ ] Define record matching rules
- [ ] Define duplicate handling
- [ ] Establish migration sequencing
- [ ] Create test migrations
- [ ] Validate migrated records
- [ ] Obtain business approval
- [ ] Create a final migration plan

Whenever possible, conduct multiple test migrations before production deployment.

---

# 8. Define Security and Access

Users should have access to the information they need without unnecessary exposure.

Review:

- [ ] User roles
- [ ] Profiles
- [ ] Permission sets
- [ ] Permission set groups
- [ ] Organization-wide defaults
- [ ] Role hierarchy
- [ ] Sharing rules
- [ ] Teams
- [ ] Field-level security
- [ ] Sensitive data
- [ ] Integration users
- [ ] Administrative access

Apply the principle of least privilege wherever practical.

---

# 9. Design Automation

Automation should reduce unnecessary work while maintaining appropriate controls.

Potential Salesforce automation includes:

- Flow
- Approval processes
- Assignment
- Notifications
- Record creation
- Record updates
- Task creation
- Routing
- Integrations
- AI-assisted workflows

For every automation:

- [ ] Define the trigger
- [ ] Define required inputs
- [ ] Define decision logic
- [ ] Define expected output
- [ ] Identify exceptions
- [ ] Define error handling
- [ ] Determine whether human approval is required
- [ ] Define monitoring requirements

A useful pattern is:

**Business Event → Validation → Automation → Exception Handling → Human Review → System Update**

---

# 10. Plan Integrations

Identify every system that needs to exchange information with Salesforce.

Examples may include:

- ERP
- Accounting
- Marketing automation
- Customer support
- Ecommerce
- Data warehouse
- Telephony
- Contract management
- Payment platforms
- Operational systems

For each integration:

- [ ] Define the business purpose
- [ ] Identify the source system
- [ ] Identify the destination system
- [ ] Define the system of record
- [ ] Identify data being exchanged
- [ ] Define synchronization frequency
- [ ] Define error handling
- [ ] Define monitoring
- [ ] Define integration ownership
- [ ] Document security requirements

Avoid using employees and spreadsheets as the integration layer between systems.

Instead of:

**System A → Employee → Spreadsheet → Employee → System B**

Work toward:

**System A → Governed Integration → System B**

---

# 11. Define Reporting and KPIs

Reporting requirements should be established before the implementation is complete.

- [ ] Identify executive KPIs
- [ ] Identify management reporting
- [ ] Identify operational reporting
- [ ] Define metric calculations
- [ ] Establish standard definitions
- [ ] Identify required dashboard filters
- [ ] Define reporting ownership
- [ ] Validate required data exists
- [ ] Create dashboards
- [ ] Validate results with stakeholders

A mature reporting environment progresses toward:

**Trusted Data → Consistent Metrics → Automated Reporting → Proactive Analytics → AI-Assisted Decision Support**

---

# 12. Design the User Experience

Salesforce should make it easier for users to perform their jobs.

Evaluate:

- [ ] Lightning record pages
- [ ] Page layouts
- [ ] Dynamic forms
- [ ] Related lists
- [ ] Quick actions
- [ ] Navigation
- [ ] Required fields
- [ ] Screen flows
- [ ] Mobile requirements
- [ ] User-specific experiences

Remove unnecessary information whenever possible.

More fields do not necessarily create better data.

---

# 13. Conduct User Acceptance Testing

User Acceptance Testing (UAT) should validate complete business scenarios.

Do not limit testing to individual features.

Test scenarios such as:

**New Lead → Qualification → Opportunity → Quote → Closed Won → Customer Handoff**

- [ ] Create realistic test scenarios
- [ ] Identify testers
- [ ] Define expected outcomes
- [ ] Test standard processes
- [ ] Test exceptions
- [ ] Test permissions
- [ ] Test automation
- [ ] Test integrations
- [ ] Test reports
- [ ] Document defects
- [ ] Retest resolved issues
- [ ] Obtain formal approval

---

# 14. Prepare Training

Training should focus on how employees perform their jobs in Salesforce.

- [ ] Identify user groups
- [ ] Develop role-specific training
- [ ] Create scenario-based training
- [ ] Create reference documentation
- [ ] Record training videos
- [ ] Train managers
- [ ] Train administrators
- [ ] Establish a support process
- [ ] Provide post-launch resources

Instead of teaching users every Salesforce feature, teach them how to complete the business processes they perform regularly.

---

# 15. Prepare for Deployment

Before production launch:

- [ ] Complete configuration
- [ ] Complete testing
- [ ] Resolve critical defects
- [ ] Validate integrations
- [ ] Validate permissions
- [ ] Complete data migration
- [ ] Validate migrated data
- [ ] Complete training
- [ ] Establish support procedures
- [ ] Create deployment plan
- [ ] Create rollback/contingency plan
- [ ] Communicate launch expectations

---

# 16. Launch Salesforce

During launch:

- [ ] Execute final migration
- [ ] Activate required automation
- [ ] Enable integrations
- [ ] Provision users
- [ ] Confirm permissions
- [ ] Validate critical processes
- [ ] Validate reporting
- [ ] Monitor errors
- [ ] Provide user support
- [ ] Track adoption

Treat launch as the beginning of Salesforce operations, not the end of the project.

---

# 17. Monitor Adoption

After launch, measure whether Salesforce is actually being used as intended.

Possible adoption indicators include:

- Login frequency
- Record creation
- Opportunity updates
- Required field completion
- Activity capture
- Pipeline hygiene
- Data completeness
- Dashboard usage
- Process compliance

When adoption is low, determine why before assuming additional training is the answer.

The problem may be:

- Poor process design
- Excessive data entry
- Missing automation
- Confusing page layouts
- Duplicate systems
- Lack of management adoption
- Poor data quality
- Unclear ownership

---

# 18. Establish Salesforce Governance

Salesforce should continue evolving after implementation.

Establish a governance process for:

- [ ] Enhancement requests
- [ ] New fields
- [ ] New automation
- [ ] New integrations
- [ ] User access
- [ ] Data quality
- [ ] Release management
- [ ] Documentation
- [ ] Technical debt
- [ ] Platform roadmap

Every requested change should be evaluated based on business value, user impact, architectural impact, and long-term maintainability.

---

# 19. Plan for Continuous Improvement

A Salesforce implementation is never truly finished.

Create a regular optimization cycle:

**Measure → Identify → Prioritize → Improve → Test → Deploy → Measure**

Review Salesforce regularly for:

- Adoption issues
- Data quality
- Manual processes
- Automation opportunities
- Technical debt
- Integration failures
- Reporting gaps
- New Salesforce capabilities
- AI opportunities
- Changing business requirements

---

# Salesforce Implementation Checklist Summary

Before considering an implementation successful, confirm that you have addressed:

- [ ] Business objectives
- [ ] Customer lifecycle
- [ ] Process discovery
- [ ] Salesforce architecture
- [ ] Data model
- [ ] Data quality
- [ ] Data migration
- [ ] Security
- [ ] Automation
- [ ] Integrations
- [ ] Reporting
- [ ] User experience
- [ ] User acceptance testing
- [ ] Training
- [ ] Deployment
- [ ] Adoption
- [ ] Governance
- [ ] Continuous improvement

---

# Need Help With Your Salesforce Implementation?

[Revenue Ops LLC](https://www.revenueopsllc.com/) helps organizations design, implement, optimize, and manage Salesforce environments that support their actual business processes.

Our services include:

- Salesforce Advisory
- Salesforce Implementation
- Salesforce Optimization
- Revenue Operations Consulting
- CRM Architecture
- Data and Integration Strategy
- Business Process Automation
- AI and Agentforce
- Salesforce Managed Services

Visit **[RevenueOpsLLC.com](https://www.revenueopsllc.com/)** to learn more.

You can also explore additional [Salesforce and Revenue Operations resources](https://www.revenueopsllc.com/resources/).

---

## About Revenue Ops LLC

Revenue Ops LLC is a Salesforce consulting partner focused on helping organizations connect their people, processes, technology, and data.

This checklist is maintained as part of the Revenue Ops LLC collection of open Salesforce and Revenue Operations resources.
