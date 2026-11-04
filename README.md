# ClinicalTrials.gov Scraper & Trial Change Tracker: PubMed + FDA: examples

Track clinical trials from the official ClinicalTrials.gov API v2: status changes, completion-date slips, results posted, new trials. Optional add-ons: linked PubMed papers and FDA approval status (openFDA). Clean rows, no contact PII.

This repo shows how to call the [Clinical Trial & Cure Tracker](https://apify.com/clearfeedlabs/clinical-trial-tracker) Apify Actor from JavaScript or Python, and what the output looks like.

## What's new
- Primary/secondary outcomes, top-level min/max age and brief summary on every trial.

## Use cases
- Biotech and pharma competitive intelligence on rival pipelines
- Investors and analysts watching trial readouts and delays
- CROs and site-selection teams
- Patient-advocacy groups and health journalists

## Quick start
1. Create a free Apify account and copy your API token from Settings > Integrations.
2. Set it as an environment variable: `export APIFY_TOKEN=...` (never commit it).
3. Edit `input.json`, then run one of:
   - JavaScript: `npm i apify-client && node run.mjs`
   - Python: `pip install apify-client && python run.py`

## Output fields (first of many)
`rowType`, `nctId`, `title`, `officialTitle`, `acronym`, `overallStatus`, `whyStopped`, `studyType`, `phases`, `conditions`, `keywords`, `interventions`, `leadSponsor`, `sponsorClass`, `collaborators`, `enrollment`, `enrollmentType`, `startDate`

See `sample-output.json` for one trimmed record.

## Ready-made example tasks
- [Glioblastoma recruiting trials fda pubmed](https://apify.com/clearfeedlabs/clinical-trial-tracker/examples/glioblastoma-recruiting-trials-fda-pubmed)
- [Obesity competitor watch](https://apify.com/clearfeedlabs/clinical-trial-tracker/examples/obesity-competitor-watch)

## Pricing
Pay per result: **$2.00 per 1,000 trials**, with no subscription. The [Store page](https://apify.com/clearfeedlabs/clinical-trial-tracker) always shows current prices and every optional add-on event.

## Related Clearfeed Labs Actors
- [Grants.gov Scraper & Grant Finder API: NSF, NIH Fellowships](https://apify.com/clearfeedlabs/grant-fellowship-radar): federal grants and fellowships with deadlines
- [SEC Form D Scraper: Startup Funding Leads Feed (EDGAR)](https://apify.com/clearfeedlabs/form-d-funding-feed): newly funded companies from SEC Form D
- [Research Lab Finder: Funded Labs by Topic (NIH, NSF, PubMed)](https://apify.com/clearfeedlabs/paper-to-lab-research-finder): funded research labs by topic from NIH and NSF grants
- [All Clearfeed Labs Actors](https://apify.com/clearfeedlabs)

## FAQ
**Is this data official?** Yes. It comes from the public source named above, and each record links back to it.
**Do I need a login or proxy?** No. It uses documented public endpoints only.
**Can I schedule it?** Yes. Use Apify Schedules, the API or integrations (Zapier, Make, webhooks, MCP-compatible AI agents).

## Links
- Actor on the Apify Store: https://apify.com/clearfeedlabs/clinical-trial-tracker
- Details & pricing: https://clearfeedlabs.com/actors/clinical-trial-tracker/
- Clearfeed Labs: https://clearfeedlabs.com
- Bugs or questions: open an issue on the Actor's Issues tab on Apify.

Data comes from public sources and is provided as-is. Check the original source before relying on it. Not legal, financial or investment advice.

License: MIT
