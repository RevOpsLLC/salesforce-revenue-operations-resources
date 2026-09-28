# Salesforce Health Check Checklist

A practical Salesforce health check framework for evaluating whether your Salesforce environment is secure, scalable, maintainable, and aligned with your business processes.

Created by [Revenue Ops LLC](https://www.revenueopsllc.com/), a Salesforce consulting partner providing advisory, implementation, optimization, and managed services.

---

## What Is a Salesforce Health Check?

A Salesforce health check is a structured assessment of your Salesforce environment.

It should evaluate more than technical configuration. A comprehensive assessment considers how Salesforce supports the people, processes, technology, and data across your organization.

A Salesforce health check should answer questions such as:

- Is Salesforce supporting the way the business actually operates?
- Are users consistently adopting the platform?
- Is the data reliable?
- Are automations maintainable?
- Are security and permissions appropriate?
- Are integrations working reliably?
- Can leadership trust Salesforce reporting?
- Has unnecessary technical debt accumulated?
- Is the environment prepared for future growth?

Use this checklist to conduct a structured review.

---

# 1. Business Process Alignment

Start by determining whether Salesforce reflects the way the organization actually operates.

- [ ] Document major business processes
- [ ] Compare Salesforce workflows to actual workflows
- [ ] Identify processes occurring outside Salesforce
- [ ] Identify spreadsheet-based processes
- [ ] Identify duplicate data entry
- [ ] Identify unnecessary manual steps
- [ ] Identify process workarounds
- [ ] Review departmental handoffs
- [ ] Identify missing automation
- [ ] Identify processes that no longer reflect current operations

### Key Question

**Does Salesforce support the business process, or have users created workarounds because Salesforce does not meet their needs?**

---

# 2. Salesforce Adoption

Evaluate how consistently users interact with Salesforce.

Review:

- [ ] Active users
- [ ] Login frequency
- [ ] Record creation
- [ ] Record updates
- [ ] Opportunity updates
- [ ] Activity capture
- [ ] Required field completion
- [ ] Pipeline hygiene
- [ ] Dashboard usage
- [ ] Process compliance

Low adoption does not automatically indicate a training problem.

Potential causes include:

- Poor user experience
- Excessive data entry
- Missing automation
- Confusing processes
- Duplicate systems
- Irrelevant fields
- Poor data quality
- Lack of management adoption

---

# 3. Data Quality

Salesforce is only as useful as the information it contains.

Evaluate:

- [ ] Duplicate Accounts
- [ ] Duplicate Contacts
- [ ] Duplicate Leads
- [ ] Incomplete records
- [ ] Invalid data
- [ ] Inconsistent picklist values
- [ ] Obsolete records
- [ ] Record ownership
- [ ] Required fields
- [ ] Naming conventions
- [ ] Data standardization
- [ ] Data validation

Identify where data quality issues originate.

The solution may require changes to processes, integrations, automation, or governance rather than simply cleaning existing records.

---

# 4. Data Architecture

Review how information is structured within Salesforce.

- [ ] Review standard objects
- [ ] Review custom objects
- [ ] Review object relationships
- [ ] Review custom fields
- [ ] Identify unused fields
- [ ] Identify duplicate fields
- [ ] Review field types
- [ ] Review naming conventions
- [ ] Review required fields
- [ ] Review validation rules
- [ ] Identify unnecessary complexity

Every custom object and field should have a clear business purpose.

---

# 5. Security and Permissions

Evaluate whether users have appropriate access.

Review:

- [ ] Organization-wide defaults
- [ ] Role hierarchy
- [ ] Profiles
- [ ] Permission sets
- [ ] Permission set groups
- [ ] Sharing rules
- [ ] Teams
- [ ] Field-level security
- [ ] Administrative access
- [ ] Integration users
- [ ] Inactive users
- [ ] Sensitive data access

Apply the principle of least privilege wherever practical.

---

# 6. Automation

Review the automation running within Salesforce.

This may include:

- Flow
- Approval processes
- Assignment rules
- Validation rules
- Apex
- Scheduled automation
- Notifications
- Integrations

Evaluate:

- [ ] Automation purpose
- [ ] Business ownership
- [ ] Trigger conditions
- [ ] Error handling
- [ ] Exception handling
- [ ] Duplicate automation
- [ ] Conflicting automation
- [ ] Failed automation
- [ ] Obsolete automation
- [ ] Documentation
- [ ] Maintainability

Automation should simplify operations rather than create hidden complexity.

---

# 7. Integrations

Identify every system connected to Salesforce.

For each integration, document:

- [ ] Business purpose
- [ ] Source system
- [ ] Destination system
- [ ] System of record
- [ ] Data exchanged
- [ ] Synchronization frequency
- [ ] Integration owner
- [ ] Authentication method
- [ ] Error handling
- [ ] Monitoring
- [ ] Failure notifications

Look specifically for processes where employees manually move information between systems.

Instead of:

**System A → Employee → Spreadsheet → Employee → System B**

Work toward:

**System A → Governed Integration → System B**

---

# 8. Reports and Dashboards

Determine whether Salesforce reporting provides reliable business insight.

Review:

- [ ] Executive dashboards
- [ ] Management dashboards
- [ ] Operational reports
- [ ] KPI definitions
- [ ] Metric calculations
- [ ] Report ownership
- [ ] Duplicate reports
- [ ] Obsolete reports
- [ ] Dashboard filters
- [ ] Data completeness

Ask stakeholders:

**Do you trust the numbers in Salesforce?**

If the answer is no, determine whether the problem originates with data, process, reporting logic, or governance.

---

# 9. User Experience

Evaluate how easy Salesforce is to use.

Review:

- [ ] Lightning record pages
- [ ] Page layouts
- [ ] Dynamic forms
- [ ] Related lists
- [ ] Quick actions
- [ ] Navigation
- [ ] Required fields
- [ ] Screen flows
- [ ] Mobile experience
- [ ] Role-specific experiences

Look for opportunities to reduce clicks, unnecessary fields, and repetitive data entry.

---

# 10. Technical Debt

Technical debt accumulates as Salesforce changes over time.

Look for:

- [ ] Unused custom fields
- [ ] Unused objects
- [ ] Obsolete automation
- [ ] Duplicate automation
- [ ] Old validation rules
- [ ] Unused reports
- [ ] Unused dashboards
- [ ] Inactive users
- [ ] Legacy integrations
- [ ] Inconsistent naming conventions
- [ ] Undocumented customization

Technical debt should be prioritized based on business impact and risk.

---

# 11. Documentation

Evaluate whether administrators and business stakeholders understand how the environment works.

Review documentation for:

- [ ] Business processes
- [ ] Data model
- [ ] Automations
- [ ] Integrations
- [ ] Security architecture
- [ ] Reports and KPIs
- [ ] Administrative procedures
- [ ] Release processes
- [ ] Known issues
- [ ] System ownership

Documentation reduces dependency on individual employees and makes future changes safer.

---

# 12. Salesforce Governance

Determine how changes to Salesforce are requested, evaluated, developed, tested, and deployed.

- [ ] Establish enhancement request process
- [ ] Define prioritization criteria
- [ ] Define business ownership
- [ ] Establish development standards
- [ ] Establish testing requirements
- [ ] Establish deployment procedures
- [ ] Establish documentation requirements
- [ ] Establish release management
- [ ] Define administrative ownership
- [ ] Maintain a Salesforce roadmap

---

# 13. AI and Agentforce Readiness

If the organization plans to use Salesforce AI or Agentforce, evaluate whether the underlying environment is ready.

Review:

- [ ] Data quality
- [ ] Data accessibility
- [ ] Permissions
- [ ] Process consistency
- [ ] Knowledge availability
- [ ] Integration reliability
- [ ] Exception handling
- [ ] AI governance
- [ ] Human approval requirements
- [ ] Measurement strategy

AI will not eliminate underlying data and process problems.

Organizations generally receive greater value from AI when trusted data, consistent processes, and appropriate governance are already in place.

---

# 14. Platform Scalability

Evaluate whether the current architecture can support future requirements.

Consider:

- [ ] Expected user growth
- [ ] Data growth
- [ ] New business units
- [ ] New products or services
- [ ] Additional integrations
- [ ] Additional automation
- [ ] New reporting requirements
- [ ] AI use cases
- [ ] Platform limits
- [ ] Administrative capacity

The goal is not to design for every possible future scenario, but to avoid architecture that unnecessarily restricts future growth.

---

# Salesforce Health Check Summary

A comprehensive Salesforce health check should evaluate:

- [ ] Business process alignment
- [ ] User adoption
- [ ] Data quality
- [ ] Data architecture
- [ ] Security and permissions
- [ ] Automation
- [ ] Integrations
- [ ] Reporting and analytics
- [ ] User experience
- [ ] Technical debt
- [ ] Documentation
- [ ] Governance
- [ ] AI and Agentforce readiness
- [ ] Scalability

---

# Turning Findings Into a Roadmap

A health check should result in an actionable improvement plan.

A useful approach is:

**Assess → Identify → Prioritize → Remediate → Measure**

Consider organizing recommendations into three phases:

### Crawl

Address foundational issues such as:

- Security risks
- Critical data problems
- Broken processes
- Integration failures
- Major adoption barriers

### Walk

Improve:

- Automation
- User experience
- Reporting
- Data governance
- Process consistency

### Run

Introduce more advanced capabilities such as:

- Advanced analytics
- AI and Agentforce
- Proactive automation
- Cross-functional intelligence
- Continuous optimization

---

# Need Help Evaluating Your Salesforce Environment?

[Revenue Ops LLC](https://www.revenueopsllc.com/) helps organizations evaluate, optimize, and manage Salesforce environments.

Our services include:

- Salesforce Advisory
- Salesforce Health Checks
- Salesforce Optimization
- Salesforce Implementation
- Revenue Operations Consulting
- Data and Integration Strategy
- Business Process Automation
- AI and Agentforce
- Salesforce Managed Services

Visit **[RevenueOpsLLC.com](https://www.revenueopsllc.com/)** to learn more.

Explore additional [Salesforce and Revenue Operations resources](https://www.revenueopsllc.com/resources/).

---

## About Revenue Ops LLC

Revenue Ops LLC is a Salesforce consulting partner focused on connecting people, processes, technology, and data to create scalable revenue operations.

This checklist is maintained as part of the Revenue Ops LLC collection of open Salesforce and Revenue Operations resources.
