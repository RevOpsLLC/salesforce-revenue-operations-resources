# Data Governance Checklist for Salesforce and Revenue Operations

A practical data governance framework for organizations using Salesforce and other Revenue Operations systems.

Created by [Revenue Ops LLC](https://www.revenueopsllc.com/), a Salesforce consulting partner helping organizations improve the processes, technology, data, automation, and AI that support the customer lifecycle.

---

## What Is Data Governance?

Data governance defines how business data is created, maintained, protected, shared, and used.

Effective data governance helps organizations answer:

- What information do we maintain?
- Where should that information live?
- Which system is authoritative?
- Who owns the data?
- Who can access it?
- What makes a record complete?
- How should information be standardized?
- How are duplicates prevented?
- How long should data be retained?
- How is data shared between systems?
- How are data quality problems identified and resolved?

Data governance is not simply a Salesforce administration responsibility.

It requires participation from the business teams that create, maintain, and use the information.

---

# 1. Identify Critical Data Domains

Begin by identifying the major categories of information used across the organization.

Examples include:

- Leads
- Accounts
- Contacts
- Opportunities
- Customers
- Products
- Pricing
- Quotes
- Contracts
- Orders
- Cases
- Jobs
- Invoices
- Payments
- Marketing engagement
- Employee information

For each domain:

- [ ] Define its business purpose
- [ ] Identify the business owner
- [ ] Identify the system of record
- [ ] Identify downstream systems
- [ ] Define access requirements
- [ ] Define quality requirements

---

# 2. Define Systems of Record

Every important data domain should have an authoritative source.

Create a matrix such as:

| Data Domain | System of Record |
| --- | --- |
| Lead | Salesforce |
| Account | Salesforce |
| Contact | Salesforce |
| Opportunity | Salesforce |
| Product | Salesforce or ERP |
| Order | ERP or Operational System |
| Invoice | Accounting or ERP |
| Payment | Accounting or Payment Platform |

Your specific architecture may differ.

What matters is having a clearly defined answer.

For each data domain:

- [ ] Identify the authoritative system
- [ ] Identify systems that consume the data
- [ ] Define where records are created
- [ ] Define where records can be updated
- [ ] Define synchronization rules
- [ ] Define conflict resolution

Avoid situations where multiple systems are treated as equally authoritative for the same information without defined synchronization rules.

---

# 3. Establish Data Ownership

Technology teams can administer data, but the business should own its meaning and quality.

For each data domain, identify:

### Business Owner

Responsible for:

- Business definition
- Usage requirements
- Quality expectations
- Process decisions

### Technical Owner

Responsible for:

- Configuration
- Integration
- Security
- Technical maintenance

### Data Steward

Responsible for:

- Monitoring quality
- Resolving issues
- Maintaining standards
- Supporting users

- [ ] Assign business owners
- [ ] Assign technical owners
- [ ] Assign data stewards
- [ ] Document responsibilities
- [ ] Establish escalation procedures

---

# 4. Define Data Standards

Establish consistent rules for how information is entered and maintained.

Standards may include:

- Naming conventions
- Required fields
- Picklist values
- Address formatting
- Phone formatting
- Country values
- State values
- Industry classifications
- Account naming
- Opportunity naming
- Product naming
- Date formats

For each standard:

- [ ] Document the rule
- [ ] Identify where it applies
- [ ] Determine whether it can be enforced technically
- [ ] Define exceptions
- [ ] Assign ownership

Use system controls where practical rather than relying entirely on user memory.

---

# 5. Define Required Data

Not every field needs to be required.

Require information when it is necessary for:

- A business process
- A downstream process
- Reporting
- Automation
- Compliance
- Integration
- Customer service
- Decision making

For each required field:

- [ ] Document why it is required
- [ ] Identify when it becomes required
- [ ] Identify who provides it
- [ ] Determine how it is validated

Avoid requiring information earlier in the process than users can reasonably know it.

---

# 6. Establish Data Quality Rules

Define what good data means for each critical data domain.

Common dimensions include:

### Completeness

Is required information present?

### Accuracy

Does the information correctly represent reality?

### Consistency

Is information represented consistently across records and systems?

### Timeliness

Is the information current?

### Uniqueness

Are duplicate records controlled?

### Validity

Does the information conform to defined business rules?

Establish measurable data quality expectations whenever possible.

---

# 7. Prevent Duplicate Data

Duplicate prevention should occur before records are created whenever practical.

Evaluate:

- [ ] Salesforce matching rules
- [ ] Duplicate rules
- [ ] Integration matching logic
- [ ] Unique identifiers
- [ ] Lead conversion processes
- [ ] Account creation processes
- [ ] Contact creation processes
- [ ] Imports
- [ ] Marketing automation synchronization

Define how duplicates will be:

**Detected → Reviewed → Merged → Prevented**

Do not rely exclusively on periodic cleanup.

---

# 8. Govern Data Imports

Imports are a common source of data quality problems.

Before importing data:

- [ ] Identify the source
- [ ] Validate the data
- [ ] Remove duplicates
- [ ] Standardize formats
- [ ] Map fields
- [ ] Define record matching
- [ ] Validate ownership
- [ ] Test the import
- [ ] Document the import
- [ ] Validate results

Restrict large-scale import capabilities to appropriate users.

---

# 9. Govern Integrations

Integrations should have explicit data ownership rules.

For every integration:

- [ ] Define the source system
- [ ] Define the destination system
- [ ] Identify data exchanged
- [ ] Define direction
- [ ] Define synchronization frequency
- [ ] Define system of record
- [ ] Define matching logic
- [ ] Define error handling
- [ ] Define monitoring
- [ ] Assign ownership

A governed integration should look like:

**System A → Validation → Governed Integration → System B**

rather than:

**System A → Employee → Spreadsheet → Employee → System B**

---

# 10. Establish Data Security

Data governance includes determining who should have access to information.

Review:

- [ ] Organization-wide defaults
- [ ] Role hierarchy
- [ ] Profiles
- [ ] Permission sets
- [ ] Permission set groups
- [ ] Sharing rules
- [ ] Field-level security
- [ ] Integration users
- [ ] Administrative access
- [ ] Sensitive information

Apply least-privilege principles wherever practical.

Users, integrations, automation, and AI should receive the access required to perform their functions, but no more.

---

# 11. Establish Data Lifecycle Policies

Determine how information should be handled throughout its lifecycle.

Define:

**Create → Maintain → Use → Archive → Delete**

Consider:

- [ ] Record creation
- [ ] Ownership
- [ ] Maintenance
- [ ] Retention requirements
- [ ] Archiving
- [ ] Deletion
- [ ] Legal requirements
- [ ] Privacy requirements

Not all historical data needs to remain indefinitely in operational systems.

---

# 12. Govern Reporting Metrics

Data governance also applies to business metrics.

For important KPIs:

- [ ] Define the metric
- [ ] Define the calculation
- [ ] Identify the source data
- [ ] Identify the system of record
- [ ] Assign ownership
- [ ] Establish reporting frequency
- [ ] Document exclusions
- [ ] Document business rules

Avoid situations where multiple departments use the same KPI name but calculate it differently.

The goal is:

**Trusted Data → Consistent Metrics → Automated Reporting**

---

# 13. Monitor Data Quality

Data governance requires ongoing monitoring.

Create dashboards or reports for:

- Duplicate records
- Missing required information
- Invalid values
- Unassigned records
- Stale records
- Integration failures
- Incomplete lifecycle stages
- Records failing business rules

Assign ownership for resolving identified problems.

A dashboard nobody owns does not create governance.

---

# 14. Establish Change Governance

Changes to the data model should follow a defined process.

Before creating a new field, object, or data structure, ask:

- Does this information already exist?
- Why is it needed?
- Who will populate it?
- Who will use it?
- Is it required for reporting?
- Is it required for automation?
- Does it need to integrate with another system?
- Who owns it?
- How long will it remain relevant?

For Salesforce changes:

- [ ] Document the requirement
- [ ] Review architectural impact
- [ ] Review reporting impact
- [ ] Review automation impact
- [ ] Review integration impact
- [ ] Test the change
- [ ] Document the change

---

# 15. Prepare Data for AI and Agentforce

AI increases the importance of data governance.

Before using Salesforce Agentforce or other AI capabilities, evaluate:

- [ ] Data accuracy
- [ ] Data completeness
- [ ] Data accessibility
- [ ] Data permissions
- [ ] Knowledge quality
- [ ] Data freshness
- [ ] System-of-record definitions
- [ ] Integration reliability
- [ ] Sensitive data
- [ ] AI access controls

AI should operate on governed information whenever possible.

Giving an AI system access to more data does not automatically make it more useful.

The data needs to be relevant, trustworthy, appropriately permissioned, and understandable in the context of the business process.

---

# 16. Create a Data Governance Council

For larger organizations, establish a cross-functional governance group.

Potential participants include:

- Revenue Operations
- Sales
- Marketing
- Customer Service
- Finance
- Operations
- IT
- Salesforce Administration
- Data and Analytics
- Security or Compliance

The group can review:

- Data standards
- Quality issues
- New requirements
- Integration changes
- KPI definitions
- Data ownership
- AI use cases
- Governance policies

Governance should enable responsible use of data rather than create unnecessary bureaucracy.

---

# Data Governance Checklist Summary

A mature data governance program should address:

- [ ] Critical data domains
- [ ] Systems of record
- [ ] Data ownership
- [ ] Data standards
- [ ] Required information
- [ ] Data quality
- [ ] Duplicate prevention
- [ ] Data imports
- [ ] Integrations
- [ ] Security
- [ ] Data lifecycle
- [ ] Reporting metrics
- [ ] Quality monitoring
- [ ] Change governance
- [ ] AI and Agentforce readiness
- [ ] Cross-functional governance

---

# Data Governance Maturity

A practical roadmap can use a Crawl → Walk → Run model.

## Crawl

Establish the foundation:

- Identify systems of record
- Assign ownership
- Define critical data
- Address major quality problems
- Establish security
- Document standards

## Walk

Create consistent governance:

- Implement validation
- Improve duplicate prevention
- Govern integrations
- Standardize KPIs
- Monitor data quality
- Establish change governance

## Run

Use governed data strategically:

- Automated quality monitoring
- Cross-functional analytics
- Proactive data management
- AI-assisted workflows
- Agentforce
- Advanced analytics
- Continuous optimization

---

# Need Help With Salesforce Data Governance?

[Revenue Ops LLC](https://www.revenueopsllc.com/) helps organizations build Salesforce and Revenue Operations environments supported by reliable, governed data.

Our services include:

- Salesforce Advisory
- Salesforce Implementation
- Revenue Operations Consulting
- Data Governance
- CRM Architecture
- Data and Integration Strategy
- Reporting and Analytics
- Business Process Automation
- AI and Agentforce
- Salesforce Managed Services

Visit **[RevenueOpsLLC.com](https://www.revenueopsllc.com/)** to learn more.

Explore additional [Salesforce and Revenue Operations resources](https://www.revenueopsllc.com/resources/).

---

## About Revenue Ops LLC

Revenue Ops LLC is a Salesforce consulting partner helping organizations connect their people, processes, technology, and data across the customer lifecycle.

This checklist is maintained as part of the Revenue Ops LLC collection of open Salesforce and Revenue Operations resources.
