# LinkedIn Public Feed

The **LinkedIn Public Feed** workflow is designed to discover and qualify opportunities from people actively posting on LinkedIn, then reach them with personalized outreach.

This workflow is usually strongest for **solo-preneurs, founders, independent professionals, and small teams** who are visibly active in public conversations.

If your main goal is to target **larger companies at scale**, use the **[LinkedIn Ad Library](reference-workflows/linkedin-ad-library.md)** workflow instead.

## High-Level Flow

The workflow configures one main source that scrapes LinkedIn public feed activity and then runs automated qualification and outreach rules.

1. **Collect leads from LinkedIn Public Feed**
The source ingests leads from the configured LinkedIn feed URL.

2. **Qualify leads**
Rules enrich and filter leads (including country/company context) and move approved leads through internal tags.

3. **Run outreach branches**
The workflow can trigger:
- LinkedIn sequence steps (connection + follow-up)
- Email enrichment, verification, and personalized email sequence

4. **Personalize messages with AI agents**
The setup creates an outreach agent that uses your campaign prompt to generate personalized first-touch messages.

5. **Mark opportunities for download and tracking**
Qualified outcomes are tagged as opportunities and become available for reporting/export.

## Best Fit

Use this workflow when:

- You want to engage people who are currently active and visible on LinkedIn.
- Your ICP includes smaller operators and decision-makers who post frequently.
- You need a fast path from discovery to personalized outreach.

