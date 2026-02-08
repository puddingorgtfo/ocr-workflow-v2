# OCR Workflow V2 – n8n Automated Insurance Declaration Page Scanner

**ocr-workflow-v2**

An **n8n workflow** designed for **automated OCR scanning** and structured data extraction from **insurance declaration pages** (dec pages), renewal notices, Acord forms, or similar homeowner/auto insurance documents.

This workflow takes uploaded/scanned insurance dec pages (PDFs or images), performs **OCR** to extract readable text, and uses intelligent extraction logic (via AI nodes, structured parsing, or regex + post-processing) to reliably pull key policy information.

### Key Extracted Fields
- Insured name / Named insured
- Mailing / Property address
- Policy number
- Carrier / Company name
- Policy effective & expiration dates
- Policy period
- Coverage limits (dwelling, other structures, personal property, liability, etc.)
- Deductibles (wind/hail, all other perils, etc.)
- Roof age / Year built / Construction year
- Premium amounts
- Mortgagee / Lienholder information
- Additional insureds / Loss payees
- And more… (easily extensible)

### Features
- Fully automated – trigger via webhook, email, file watcher, form upload, etc.
- Handles both clean digital PDFs and scanned/photographed documents
- Robust OCR + extraction pipeline (V2 improves accuracy and field coverage)
- Modular design – easy to customize fields, add validation rules, or route data to CRMs, spreadsheets, databases, Slack/email notifications, etc.
- MIT licensed – free to use, modify, and distribute

### Installation
1. Import `workflow.json` into your n8n instance
2. Configure required credentials  
   (e.g. OCR service, AI model provider, Google Sheets/Airtable, email, etc.)
3. Update any hardcoded workflow IDs, webhook URLs or node references to match your environment
4. Activate the workflow

### Detailed Setup
See [`docs/setup.md`](docs/setup.md) for:
- Node-by-node breakdown
- Required credentials & API keys
- Recommended OCR/AI services (Gemini, Mistral, OpenAI, OCR.space, etc.)
- Common customizations & troubleshooting
- Example input/output samples

### Use Cases
- Automate insurance quoting / renewal reviews
- Feed extracted data into rating engines or underwriting systems
- Populate CRM / policy management tools automatically
- Create audit trails or compliance reports
- Reduce manual data entry for agents, MGAs, or carriers

### License
[MIT License](LICENSE) – do whatever you want with it 😄

---

⭐ Star this repo if it saves you time processing dec pages!  
🐛 Issues & PRs welcome – especially field improvements or better extraction prompts.