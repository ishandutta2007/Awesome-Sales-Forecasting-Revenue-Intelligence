# Awesome-Sales-Forecasting-Revenue-Intelligence

## Top Sales Forecasting & Revenue Intelligence Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Pipeline Forecasting, Conversation Intelligence & Self-Hosted Revenue Analytics*  

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Sales Forecasting & Revenue Intelligence**. These tools enable revenue teams to predict deal outcomes, analyze sales conversations, identify pipeline risk, and forecast revenue with confidence—turning gut-feel projections into data-backed commitments.



**Examples** include HubSpot Predictable AI Forecasting, Clari, Gong, BoostUp.ai, Revenue.io, Aviso, InsightSquared, Salesforce Einstein Forecasting, Salesloft, and Troops (the category leaders).



**Open-source emphasis**: Sales Forecasting & Revenue Intelligence is a domain where open-source tooling is **fragmented and largely immature for the full enterprise experience**, but genuinely viable for **specific slices** of the problem. **LedgerMind AI** provides the strongest standalone revenue intelligence engine—transaction-based revenue tracking, 30-day linear regression forecasting with confidence intervals, Z-score anomaly detection, and Claude AI-powered insights (with deterministic fallback) . **AI Business Intelligence Platform** (GeekYasuo) offers a broader enterprise BI stack with ML forecasting models for revenue, sales, and churn, plus natural language querying . For **conversation intelligence** (the Gong equivalent), there is **no mature open-source platform**—the closest is **agentic-os**'s Gong-to-Insight pipeline, a Python script that extracts objections, buying signals, and competitive mentions from call transcripts . The critical caveat: **no open-source project replicates Clari's multi-source pipeline aggregation or Gong's at-scale conversation analytics**—those require integrating CRM, email, calendar, and call recording systems that open-source tools address only piecemeal.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[HubSpot Predictable AI Forecasting](https://www.hubspot.com/)**  

  AI-powered revenue forecasting within HubSpot's Sales Hub; predicts deal outcomes and pipeline revenue based on historical patterns and CRM activity.



- **[Clari](https://www.clari.com/)**  

  The benchmark for revenue intelligence; aggregates CRM, email, calendar, and call data to forecast revenue, identify pipeline risk, and surface deal insights for revenue leaders.



- **[Gong](https://www.gong.io/)**  

  Conversation intelligence platform; records and analyzes sales calls to extract objections, buying signals, and coaching insights, then correlates them with deal outcomes and forecasts.



- **[BoostUp.ai](https://www.boostup.ai/)**  

  Revenue intelligence platform combining forecasting, pipeline analytics, and conversation intelligence; positioned for revenue operations teams.



- **[Revenue.io](https://www.revenue.io/)**  

  Revenue operations platform with real-time guidance during calls and AI-powered forecasting.



- **[Aviso](https://www.aviso.com/)**  

  AI-driven revenue intelligence platform with forecasting, pipeline inspection, and deal risk scoring.



- **[InsightSquared](https://www.insightsquared.com/)**  

  Revenue analytics and forecasting platform; provides pipeline visibility and predictive insights for sales leaders.



- **[Salesforce Einstein Forecasting](https://www.salesforce.com/)**  

  AI-powered forecasting within Salesforce CRM; predicts deal outcomes and revenue based on historical data and activity patterns.



- **[Salesloft](https://salesloft.com/)**  

  Sales engagement platform with forecasting and revenue intelligence capabilities; combines cadences, conversations, and deal analytics.



- **[Troops](https://www.troops.ai/)**  

  Revenue intelligence platform (acquired by Salesforce) with pipeline alerts, forecasting, and deal insights delivered through Slack.



## Open-Source GitHub Projects



### Revenue Intelligence & Forecasting Engines



- **[LedgerMind AI](https://github.com/Auspicious14/ledgermind-ai)**  

  The most focused open-source **revenue intelligence engine** for small businesses . Features: **revenue and profit tracking** with daily/monthly aggregations; product performance and margin analysis; **30-day revenue forecast** via linear regression with confidence intervals and transparent R² accuracy; **Z-score anomaly detection** with spike/drop classification, severity levels, and human-readable explanations; **Claude AI integration** for 6 insight categories (revenue, profitability, risk, opportunity, warning, general) with priority scoring and actionable recommendations, plus deterministic fallback when API is unavailable; PDF/HTML export of business health reports; Next.js dashboard with KPI cards, interactive charts, and responsive design . CSV upload for transaction data; PostgreSQL via Prisma . **Best for small businesses wanting AI-powered revenue intelligence with forecasting and anomaly detection**—but it is transaction-data-focused, not a CRM-native pipeline forecasting tool.



- **[AI Business Intelligence Platform (GeekYasuo)](https://github.com/GeekYasuo/ai-business-intelligence-platform)**  

  Enterprise AI-powered **business intelligence platform** with ML forecasting and natural language querying . Features: **revenue, sales, and churn forecasting models** with confidence intervals and model accuracy tracking; **real-time anomaly detection** using Isolation Forest and LSTM autoencoders; **natural language querying** ("What were our top 3 products by revenue last quarter?") with AI-powered responses and visualizations; modern React/TypeScript frontend with Redux Toolkit and Chart.js/D3; Node.js/Express backend with GraphQL; Python ML services (FastAPI, TensorFlow, scikit-learn, OpenAI GPT-4) . Docker/Kubernetes deployment. **Best for teams wanting a full BI stack with ML forecasting and NL querying**—but it is a broad platform rather than a sales-specific revenue intelligence tool, and requires OpenAI API access.



### Conversation Intelligence (Gong Alternative)



- **[agentic-os Gong-to-Insight Pipeline](https://github.com/LazyIsEfficient/agentic-os/blob/main/.claude/skills/revenue-intelligence/README.md)**  

  The closest open-source equivalent to **conversation intelligence**, but it is a **Python script**, not a platform . Works with the Gong API or plain transcript files . Extracts: **objections** categorized as pricing, timing, competition, authority, or need; **buying signals** (budget confirmed, timeline mentioned, decision maker engaged, champion identified); **competitive mentions** with sentiment; **pricing discussions** with dollar amounts; **content topics** for recurring objection patterns; and **follow-up drafts** for personalized outbound . Outputs structured JSON with call temperature (WARM/HOT/COLD) . **Best for teams wanting transcript analysis without Gong's cost**—but it requires transcripts (from Gong or elsewhere) and does not record or transcribe calls itself.



### Sales Forecasting & Analytics Dashboards



- **[Horilla CRM](https://github.com/horilla/horilla-crm)**  

  Free and open-source **HR and CRM software** (LGPL-2.1) with a **Forecasting** module for revenue predictions and sales analytics alongside Big Deal Alerts for high-value opportunities . Features: leads, opportunities with customizable stages, campaign management with ROI analysis, activity tracking, email integration, interactive dashboards, and advanced reports . Docker deployment with PostgreSQL . **Best for teams wanting a full CRM with built-in forecasting**—but the forecasting is basic compared to dedicated revenue intelligence platforms .



- **[Django-CRM](https://github.com/DjangoCRM/DjangoCRM)**  

  Comprehensive open-source **enterprise CRM** with **Sales Forecasting & Analytics** generating detailed forecasts and reports . Features: lead management, deal management, email integration, collaborative CRM, mass mailing, and analytics including income summaries and sales funnels . Django 5.2/Python 3.10+, MySQL/PostgreSQL . **Best for Django teams wanting CRM with forecasting**—but like Horilla, forecasting is a module rather than a specialized engine .



- **[SalesIQ](https://github.com/badrr06/SalesIq)**  

  Open-source **sales management and forecasting system** (Flask, Chart.js) . Features: CRUD for products/customers/sales; dashboard with KPIs; **monthly sales + 6-month forecast** (ARIMA if statsmodels available, else Linear Regression); top products; CSV export . MySQL or SQLite . **Best for small businesses wanting lightweight sales tracking and forecasting**—but it is sales-only, without CRM or conversation data .



- **[MarketIQ](https://github.com/AmirhosseinHonardoust/Market-IQ)**  

  Open-source **Streamlit-powered analytics platform** with SQL-driven pipelines, interactive visualization, and **Prophet forecasting** . Features: KPI dashboard (revenue, orders, customers, AOV, MoM trends); Prophet predicts future sales with confidence intervals; multi-view charts; real-time filters; CSV/image export . SQLite/PostgreSQL-ready . **Best for analysts wanting a quick sales forecasting dashboard**—but it is a standalone analytics tool, not integrated with CRM or pipeline data .



### Revenue Attribution & Content ROI



- **[agentic-os Revenue Attribution Mapper](https://github.com/LazyIsEfficient/agentic-os/blob/main/.claude/skills/revenue-intelligence/README.md)**  

  Python script that maps content (blog posts, videos, podcasts, webinars) to **closed deals** using first-touch, linear, or time-decay attribution models . Produces content-to-revenue mapping, CPA by content type, and content gap analysis by funnel stage . **Best for content-led growth teams** wanting to prove content ROI—but it is a script requiring your content and deal data, not a platform .



### Additional Strong Open-Source Options



- **RevenueOS** — Self-hosted "revenue department" (MIT) that crawls your site, ad exports, lead lists, and mailbox to find opportunities; executes approved actions (SEO content, ads fixes, outreach) and measures outcomes . **Requires human approval for every action**—no automatic sends/spends . **Best for founders wanting an AI-assisted revenue ops workflow**—but it is early-stage and action-oriented rather than forecasting-focused .

- **skill-analytics-reporting (zavora-ai)** — Revenue intelligence **skill for AI agents** (Apache-2.0) with 28 MCP tools for metrics, funnels, anomaly detection, forecasting, and dashboards . **Not a platform**—it is a skill library for AI agents to query analytics data, requiring `mcp-analytics` and data sources .

- **Green-AI-Hub ai-based-sales-forecasting** — Open-source sales forecasting backend (Flask) with AI model training and optional frontend; MIT licensed . **Research project**—verify production maturity, but demonstrates the model-training-to-API pattern .

- **Superstore Analytics Portfolio** — Streamlit dashboard with Holt-Winters forecasting, RFM segmentation, and ROI simulation . **Portfolio project**—for learning patterns, not production deployment .



**Frameworks for building custom systems**: For **standalone revenue intelligence with forecasting and anomaly detection**, LedgerMind AI . For **broad BI with ML forecasting and NL querying**, AI Business Intelligence Platform . For **conversation transcript analysis**, agentic-os Gong-to-Insight pipeline (requires transcripts) . For **CRM with basic forecasting**, Horilla or Django-CRM . For **content ROI attribution**, agentic-os Revenue Attribution Mapper . No open-source project replicates **Clari's multi-source pipeline aggregation** or **Gong's at-scale call recording and analysis**—those require commercial platforms.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Sales forecasting and revenue intelligence platforms handling deal data and call recordings must comply with applicable privacy regulations (GDPR, CCPA) and call recording consent laws; **AI-generated forecasts and insights should be treated as decision support, not guarantees**—model accuracy varies and human judgment remains essential.

- **Open-source sales forecasting and revenue intelligence is fragmented and immature for the full enterprise experience**—LedgerMind AI provides a focused revenue intelligence engine , and the agentic-os scripts demonstrate conversation analysis patterns . However, **no open-source project replicates Clari's multi-source pipeline aggregation or Gong's at-scale conversation recording and analysis**—organizations requiring those capabilities should evaluate commercial platforms or invest in significant custom integration.

- Verify license terms for commercial use; LedgerMind AI is open-source (check repository) , Horilla CRM uses LGPL-2.1 , and Django-CRM is open-source .



---



**Made for revenue operations leaders, sales analysts, and teams building forecasting and intelligence infrastructure.**  

Let's make sales forecasting more open, but with clear eyes about the multi-source integration and conversation intelligence gaps that commercial platforms still fill.
