# LinkedIn Ad Library

The **LinkedIn Ad Library** workflow is designed to discover and qualify opportunities from companies running ads on LinkedIn, then reach decision-makers with personalized outreach.

This workflow is usually strongest for targeting **larger companies at scale**.

If your main goal is to engage solo-preneurs and people who post frequently on LinkedIn, use the **[LinkedIn Public Feed](./linkedin-public-feed.md)** workflow instead.

## High-Level Flow

The workflow configures one main source that scrapes LinkedIn Ad Library data and then runs automated qualification, enrichment, and outreach rules.

1. **Collect leads and companies from LinkedIn Ad Library**
The source ingests leads and company records from public ad listings.

2. **Find company owners**
Rules identify likely owners or key decision-makers connected to those companies.

3. **Append owner country and email**
The workflow enriches owner profiles with country and email data to improve targeting and contactability.

4. **Run outreach branches**
The workflow can trigger:
- LinkedIn sequence steps (connection + follow-up)
- Email verification and personalized email sequence

5. **Mark opportunities for download and tracking**
Qualified outcomes are tagged as opportunities and become available for reporting/export.

## Best Fit

Use this workflow when:

- You want to target companies already investing in paid acquisition.
- Your ICP includes medium and large organizations.
- You want a company-first approach before reaching individual decision-makers.
