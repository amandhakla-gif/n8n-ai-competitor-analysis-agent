# n8n-ai-competitor-analysis-agent
An n8n AI agent that automates end-to-end competitor analysis using LLMs and web search.
# n8n AI Competitor Analysis Agent

This project contains an n8n-based AI agent that automates end-to-end competitor analysis.
The agent identifies direct competitors, researches their products, pricing, recent news,
and unique value propositions, and compiles structured results into Google Docs/Sheets.

## What This Agent Does

1. Accepts company and industry inputs via an n8n form
2. Identifies top competitors using Exa.ai and Perplexity
3. Iterates over competitor URLs
4. Conducts deep research on each competitor:
   - Product and feature analysis (Perplexity)
   - Latest news and updates (Tavily)
5. Summarizes findings using an LLM
6. Outputs structured results to Google Docs/Google Sheets

## Key Design Decisions

- **Exa.ai** for high-precision competitor discovery
- **Perplexity** for structured research and reasoning
- **Tavily** for fresh news signals
- **Code nodes** for deterministic parsing and reliability
- **Google Docs & Sheets** for stakeholder-ready outputs

## How to Run This Workflow

1. Import `workflow.json` into n8n
2. Add credentials for:
   - Perplexity API
   - Exa.ai API
   - Tavily API
   - Groq API
   - Google Docs & Google Sheets
3. Activate the workflow
4. Open the form trigger endpoint
5. Submit company and industry details

## Notes

- API keys are **not included**
- Please use your API Keys & Credentials and replace it in the json file.
