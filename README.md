# LinkedIn Ads MCP Starter Kit — Manage LinkedIn Ads with AI

[![MCP Compatible](https://img.shields.io/badge/MCP-compatible-blue)](https://modelcontextprotocol.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform: LinkedIn Ads](https://img.shields.io/badge/Platform-LinkedIn%20Ads-0A66C2)](https://business.linkedin.com/marketing-solutions)

**The B2B advertiser's secret weapon.** Open this repo in Amp, Cursor, or VS Code and manage LinkedIn ad campaigns with AI — target by job title, company size, industry, and seniority without wrestling with LinkedIn's complex Campaign Manager.

---

## Why LinkedIn Ads + AI?

LinkedIn is the only advertising platform where you can target "VP of Engineering at Series B+ SaaS companies with 50-200 employees." No other platform comes close for B2B precision.

But LinkedIn's Campaign Manager is notoriously painful. The Rest.li API is complex, CPCs run $8-15 (vs $2-3 on Google), and the UI makes simple tasks feel hard. Most B2B marketers know LinkedIn Ads should work for them — they just can't justify the time investment.

That's where AI agents change the game. The agent handles LinkedIn's complex API, knows the targeting taxonomy, and can build campaigns that would take a human 45 minutes in under 60 seconds.

**Best for:** Enterprise sales, B2B SaaS, recruiting, professional services, account-based marketing (ABM), event promotion to professional audiences.

---

## Quick Start (30 Seconds)

### Amp / Cursor / VS Code (Copilot)

1. **Get a free API key** at [syntermedia.ai/developer](https://syntermedia.ai/developer)
2. **Set the key:**
   ```bash
   export SYNTER_API_KEY=syn_your_key_here
   ```
3. **Open this repo** in your editor
4. **Start chatting** — MCP tools are pre-configured in `.mcp.json`

### Claude Desktop

Copy `claude_desktop_config.json` to your Claude config directory and replace the API key:

- **macOS:** `~/Library/Application Support/Claude/claude_desktop_config.json`
- **Windows:** `%APPDATA%\Claude\claude_desktop_config.json`

---

## What You Can Do

| Capability | Example |
|-----------|---------|
| **Create Sponsored Content** | "Launch a Sponsored Content campaign targeting CTOs at fintech companies" |
| **Lead Gen Forms** | "Set up a Lead Gen Form campaign for our whitepaper download" |
| **Job Title Targeting** | "Target Director+ level in Marketing, Sales, and RevOps" |
| **Company Targeting** | "Show ads only to employees at our target account list of 500 companies" |
| **InMail Campaigns** | "Create a Sponsored InMail campaign inviting VPs to our webinar" |
| **Audience Building** | "Build an audience of SaaS decision-makers at companies with 100-1000 employees" |
| **Budget Management** | "What's the minimum viable budget for testing LinkedIn Ads?" |
| **Creative Upload** | "Upload this infographic as a Sponsored Content image ad" |
| **Performance Reports** | "Show me cost per lead by job function — who converts cheapest?" |
| **ABM Lists** | "Upload our ABM target account list and create a matched audience" |

---

## Example Conversations

### 1. First LinkedIn Campaign for a B2B SaaS

> **You:** I sell a $30k/year data analytics platform to mid-market companies. I want to try LinkedIn Ads. I've never run them before.
>
> **Agent:** LinkedIn is perfect for a $30k ACV product — the high CPCs ($8-15) are justified when each conversion is worth $30k.
>
> Here's my recommended first campaign:
>
> - **Objective:** Lead Generation (using LinkedIn Lead Gen Forms — 5x higher conversion rate than landing pages because the form auto-fills with LinkedIn profile data)
> - **Budget:** $100/day ($3,000/month) — this is the minimum I'd recommend for statistically meaningful results on LinkedIn
> - **Offer:** Not a demo request (too aggressive for cold traffic). Instead: "2026 Data Analytics Benchmarks Report" — valuable enough that Directors will trade their info
>
> **Targeting:**
> - Job function: IT, Engineering, Analytics
> - Seniority: Director, VP, C-Suite
> - Company size: 201-1000 employees
> - Industry: Technology, Financial Services, Healthcare
> - Geography: United States
> - **Estimated audience:** ~340,000 members
>
> **Expected performance:** $45-80 cost per lead, 37-65 leads/month
>
> **You:** That cost per lead seems high. Can we get it lower?
>
> **Agent:** On LinkedIn, $45-80 CPL for Director+ level at mid-market companies is actually strong. These aren't newsletter signups — they're qualified B2B leads with verified job titles. At your $30k ACV, you only need to close 1 in 50 leads to make this campaign wildly profitable.
>
> That said, here's how to optimize CPL over time:
> 1. Test Sponsored Content (image + text) vs Document Ads (carousel)
> 2. Target by job *function* not job *title* (broader reach, lower CPMs)
> 3. Exclude competitors by company name
> 4. After 2 weeks, create a Lookalike audience from lead form submitters

### 2. Account-Based Marketing (ABM)

> **You:** Our sales team has a target account list of 200 companies. Can we show ads only to people at those companies?
>
> **Agent:** Absolutely — this is LinkedIn's killer feature for ABM. I'll set up a matched audience.
>
> **What I need:** A CSV with company names (and ideally LinkedIn Company Page URLs or domains for better match rates).
>
> **What I'll build:**
> 1. Upload the list → Matched Audience (usually 70-85% match rate on LinkedIn)
> 2. Layer seniority targeting: Director+ only (no point showing ads to interns at target accounts)
> 3. Create 3 campaign tiers:
>    - **Awareness:** Thought leadership content → build brand recognition
>    - **Consideration:** Case study from a similar company → prove value
>    - **Conversion:** "Book a personalized demo" → capture demand
>
> With 200 target accounts, your audience will be ~15,000-40,000 people. Budget recommendation: $50/day ($1,500/month). This is a high-frequency, small-audience play — expect frequency of 3-5x per month, which is ideal for ABM.
>
> **You:** Here's the CSV. Start with the awareness tier only.
>
> **Agent:** Uploaded. Matched 174 of 200 companies (87% match rate). The 26 unmatched companies are mostly small startups without LinkedIn Company Pages. Campaign created targeting Director+ at these 174 companies with your thought leadership article. PAUSED until you say go.

### 3. Comparing Campaign Performance by Audience Segment

> **You:** Which audience segments are performing best across my 4 campaigns?
>
> **Agent:** Pulling performance data segmented by job function and seniority...
>
> **Top findings:**
>
> | Segment | CPL | Conversion Rate | Lead Quality Score |
> |---|---|---|---|
> | VP, Engineering | $52.30 | 4.2% | 8.5/10 |
> | Director, IT | $48.70 | 3.8% | 7.2/10 |
> | C-Suite, All | $91.20 | 1.9% | 9.1/10 |
> | Manager, Analytics | $31.40 | 5.1% | 5.3/10 |
>
> **Key insight:** Managers convert at the highest rate and lowest cost, but their Lead Quality Score is only 5.3 — they likely can't sign a $30k contract. VPs in Engineering are your sweet spot: reasonable CPL ($52), good conversion rate, and high quality.
>
> **Recommendation:** Increase budget on VP-level targeting by 40%, reduce Manager targeting by 50%. The C-Suite campaigns are expensive but those leads close at 3x the rate — keep the budget steady.

### 4. Document Ads for Content Marketing

> **You:** I have a 15-page PDF guide. Can I turn it into an ad?
>
> **Agent:** Yes — LinkedIn Document Ads are perfect for this. They let users swipe through your PDF directly in the feed without leaving LinkedIn. Engagement rates are typically 2-3x higher than standard image ads.
>
> Here's how I'll set it up:
> 1. Upload your PDF as a Document Ad creative
> 2. LinkedIn will render it as a swipeable carousel in the feed
> 3. Users can preview 3-4 pages, then must submit a Lead Gen Form to download the full PDF
> 4. This "gated preview" approach gets 40% higher form completion than a blind download offer
>
> **Creative tips for Document Ads:**
> - Make page 1 a compelling cover (it's your ad creative)
> - Pages 2-3 should deliver real value (earn the form submission)
> - Page 4 should be a teaser — "See the full analysis..."
> - Use data visualizations — they stop the scroll
>
> Want me to create this campaign targeting your existing audience?

### 5. LinkedIn vs Google for B2B

> **You:** Should I run LinkedIn Ads or Google Ads for B2B lead gen?
>
> **Agent:** Both, but for different reasons. Let me pull your data to compare...
>
> | Metric | LinkedIn | Google Search |
> |---|---|---|
> | Cost per Lead | $62.40 | $28.50 |
> | Lead-to-SQL Rate | 23% | 11% |
> | Cost per SQL | $271 | $259 |
> | SQL-to-Close Rate | 18% | 9% |
> | Cost per Customer | $1,506 | $2,878 |
>
> **The full picture changes everything.** Google leads are cheaper, but LinkedIn leads close at 2x the rate. Your actual cost per customer is **47% lower on LinkedIn** ($1,506 vs $2,878).
>
> This makes sense: LinkedIn lets you target decision-makers directly, while Google captures anyone searching "data analytics software" — including students, researchers, and tire-kickers.
>
> **My recommendation:** Keep both, but reallocate 60% of budget to LinkedIn since it produces cheaper customers despite more expensive leads.

---

## LinkedIn Ads Tips from the Pros

1. **Target by job function, not job title.** "VP of Sales" misses "VP of Revenue," "VP of Commercial," and "Head of Sales." Job function "Sales" + Seniority "VP" catches them all.
2. **Minimum budget: $25/day.** LinkedIn's auction is expensive — $25/day gives you enough to win impressions for a targeted B2B audience. Below this, your ads barely deliver.
3. **Lead Gen Forms crush landing pages.** LinkedIn auto-fills name, email, company, and title. Conversion rates are 3-5x higher than sending traffic to your website.
4. **Frequency is your friend in ABM.** Unlike consumer ads where high frequency means annoyance, B2B decision-makers need to see your brand 7-10 times before they engage. Don't panic at frequency of 4-5.
5. **Exclude competitors.** Always add competitor company names as exclusions. You don't want Salesforce employees downloading your "Why Switch from Salesforce" guide.
6. **Most expensive CPC, highest quality leads.** LinkedIn CPCs ($8-15) scare people away, but for high-ACV B2B products ($10k+), the cost per *qualified* opportunity is often lower than any other channel.
7. **Refresh creative monthly.** LinkedIn audiences are small — creative fatigue hits faster than on Meta. Rotate between image ads, carousels, Document Ads, and video.

---

## FAQ

### Is there an MCP for LinkedIn Ads?
Yes — this repo. It pre-configures the Synter MCP server for LinkedIn Ads management. Works with Amp, Cursor, VS Code, and Claude Desktop.

### Can AI manage LinkedIn advertising?
Absolutely. With this MCP starter kit, your AI agent can create campaigns, build audiences, upload creatives, set up Lead Gen Forms, and pull performance reports — all through the LinkedIn Marketing API.

### Why are LinkedIn Ads so expensive?
LinkedIn CPCs are $8-15 because you're targeting verified professionals by exact job title, company, and seniority. No other platform offers this precision. For B2B products with $10k+ ACV, the cost per qualified opportunity is often lower than cheaper platforms.

### Can I target specific companies on LinkedIn?
Yes. Upload a list of company names and the agent will create a Matched Audience. LinkedIn typically matches 70-85% of company names. You can then layer seniority and job function targeting on top.

### Does this support Lead Gen Forms?
Yes. The agent can create Lead Gen Form campaigns with custom questions, thank-you messages, and CRM integrations. LinkedIn auto-fills most fields, which dramatically improves conversion rates.

### Can I run ABM campaigns with this?
Yes. Upload your target account list, and the agent builds a Matched Audience, sets up multi-tier campaigns (awareness → consideration → conversion), and reports on engagement by account.

---

## Related Repos

- [google-ads-agent](https://github.com/Synter-Media-AI/google-ads-agent) — Search intent capture
- [salesforce-agent](https://github.com/Synter-Media-AI/salesforce-agent) — Sync Salesforce leads to LinkedIn audiences
- [hubspot-agent](https://github.com/Synter-Media-AI/hubspot-agent) — Sync HubSpot contacts for targeting
- [audience-sync-agent](https://github.com/Synter-Media-AI/audience-sync-agent) — Upload audiences to LinkedIn
- [cross-platform-ads-agent](https://github.com/Synter-Media-AI/cross-platform-ads-agent) — Compare LinkedIn vs other channels
- [attio-crm-agent](https://github.com/Synter-Media-AI/attio-crm-agent) — Export CRM contacts for targeting

---

## License

MIT — see [LICENSE](LICENSE) for details.

Built by [Synter](https://syntermedia.ai) · [Get API Key](https://syntermedia.ai/developer) · [Documentation](https://syntermedia.ai/docs)
