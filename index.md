# Welcome to Experts Inside's Azure Governance Approach

This doc is an example on how you can manage your Azure Governance in your organization.

## The webinars

We will cover the aspects in five different webinars. Later we will add the recordings.

1. 18.05.2021: [Initialzündung](https://www.eventbrite.ch/e/webinar-hiking-to-mount-azure-governance-initialzundung-tickets-153506487035)
2. 01.06.2021: [Governance Light](https://www.eventbrite.ch/e/webinar-hiking-to-mount-azure-governance-governance-light-tickets-154540166799)
3. 08.06.2021
4. 15.06.2021
5. 22.06.2021

## Navigation 

- [Involved Teams](#involved-teams)
- [The Workflow](#the-workflow)
- [Guidelines](#guidelines)

## Involved Teams

Two teams are required to separate "guideline definition" from "guideline implementation". This is required like it is in politics (executive and legislative). This way the implemenatation team can't create own guidelines that would ultimatelly lead to bad quality.

### Governance Team

- Respects the IT strategy guidelines
- Defines cloud guidelines on a high level (NOK: "S2S VPN SKU must always be 'basic'"; OK: "S2S VPN is allowed if the security guidelines A, B, C can be respected")
- Promotes close alignement to the IT Architecture Board
- Promotes guidelines to service owners through common communication channels (Team Meeting, Intranet, etc.)
- Defines working areas (resource organization (management group and subscription hierarchy, tags), identity and security, cost management, security and identity, etc.)
- Documents all guidelines in an accessible way (wiki, documents, etc.)
- Members: IT Lead, IT Strategy, IT Architect, Implementation Team Representative, Licensing Guy, one or two Implementation Team members

### Implementation Team

- This team is implemented by the Governance Team
- Respects the IT strategy guidelines
- Respects and challenges the cloud guidelines (e.g. gives feedback to guidelines)
- States new guideline requests to the Governance Team
- Documents all guidelines in an accessible way (wiki, documents, etc.)
- Members: Network Guy, Security Guy, Monitoring Guy, Developer, Cloud Engineers

## The workflow

1. Guidelines are implemented via this repository
3. The Implementation Team can create pull requests to this guidelines
4. The Governance Team reviews new guidelines via pull requests
5. Approved guidelines become effective after the pull request is approved


## Guidelines

### Areas

- Foundation: Guidelines that define the "how we work".
- Governance: Resource organization, policies, tags
- Security: 
  - General security guidelines like allowed owners, AAD groups to manage RBAC 
  - Features from AAD like PIM, Conditional Access 
- Networking: VPN, Network Security Group, Routing Tables, DNS
- Cost: Cost controls like budget, cost alerts, reporting, payment methods

### Guideline numbering schema

Important: Don't change the Ids if possible. This allows to reference the guidelines.

- G\[defined number for area\].\[ascending number for each guidelines\]
- \[defined number for area\]:
- Important sub-areas can get a new number instead of the defined below (ex. Foundation - Training = 110, Foundation - Processes = 120)
  - 000: Foundation
    - 010: Training
    - 020: Processes
  - 100: Governance
  - 200: Security
  - 300: Networking
  - 400: Cost
- \[ascending number for each guideline\]
  - Start with 1 and count up


Id | Area | Description
------------ | ------------- | -------------
G000.1 | Fundation | Exceptions to guidelines are always possible. They need to be approved by the Governance Team.
G010.1 | Fundation | Training is always allowed up to 4h per week.
G100.1 | Governance | Allowed locations "Switzerland North", "West Europe". Other locations need to be explained to the Governance Team.
G100.2 | Governance | Tag "ServiceOwner" required on all subscriptions.
G200.1 | Security | Only two subscription owners allowed.
G200.2 | Security | PIM for Admin Accounts required.
G300.1 | Networking | S2S VPN to on-premises is allowed if the company's security guidelines are followed.
G400.1 | Cost | A monthly cost report splited by service is created. The IT lead and cost manager has access to these reports.
G400.2 | Cost | A budget limit can be set through the implementation team.
G400.3 | Cost | ABC


## Next Steps

- [Azure Tips and Tricks](https://microsoft.github.io/AzureTipsAndTricks)
- [Azure Governance Visualizer](https://github.com/microsoft/CloudAdoptionFramework/tree/master/govern/AzureGovernanceVisualizer)
- [Assign Pull Requests to defined project](https://github.com/apps/project-bot)
