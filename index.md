# Welcome to Experts Inside's Azure Governance Approach

This doc is an example on how you can manage your Azure Governance in your organization.

## The webinars

We will cover the aspects in five different webinars. Later we will add the recordings.

1. 18.05.2021: [Initialzündung](https://www.eventbrite.ch/e/webinar-hiking-to-mount-azure-governance-initialzundung-tickets-153506487035)
2. 01.06.2021: Governance Light
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

Id | Description
------------ | -------------
G100.1 | Only two subscription owners allowed.
G100.2 | PIM for Admin Accounts required.
