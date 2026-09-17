*AI Builders Digest — September 17, 2026*

*X / TWITTER*

*Josh Woodward* — VP at Google Labs / Gemini App
Google Notebook just got two useful student-focused upgrades: live spoken Q&A with class materials in ~100 languages, and automatic audio note saving for recorded lectures. University students in 140+ countries can access a free Google AI Plan with bigger limits.
- <https://x.com/joshwoodward/status/2099921866014306633|View tweet>

*Thibault Sottiaux* — Codex & ChatGPT at OpenAI
Teasing an efficiency-themed moment: "2026 is the year of efficiency and Tuesday is for random swag drops on your door handle." Likely hinting at a Codex or OpenAI product drop.
- <https://x.com/thsottiaux/status/2099922755655479624|View tweet>

*Peter Yang* — AI educator and solopreneur
Shared bot access codes with his community, spotlighting use cases like automated ad account monitoring, Jira blocker flagging, support ticket triage, hotel booking flow testing, and research desk automation. His advice to solopreneurs: design the business so you're doing work you enjoy, and delegate the boring stuff to bots. Also joined the Grok bot live stream.
- <https://x.com/petergyang/status/2099968897323778416|On solopreneur advice>
- <https://x.com/petergyang/status/2100027487681953834|Bot use cases roundup>

*Thariq* — Claude Code at Anthropic
Bold take: MCPs are now better than CLIs for most integrations. With models improving at tool calling, stateless MCP, and deferred tools, the tradeoffs have shifted. His tip: add `query` params to MCP tools when you need to compose or filter data.
- <https://x.com/trq212/status/2099958388230873165|View tweet>

*Amjad Masad* — CEO of Replit
Asked why, if your output domain is known in advance, you wouldn't just train a model to produce logprobs over enums instead of using structured generation. Also skewered AI movement naming: "AI Safety firm made AI unsafe. Effective Altruists are both ineffective and enabling criminal activity. Irregular is regularly incompetent."
- <https://x.com/amasad/status/2100056178705514703|On logprobs vs enums>
- <https://x.com/amasad/status/2099760428314411232|On AI naming curse>

*Guillermo Rauch* — CEO of Vercel
Launched Vercel Labs publicly — Vercel's in-public research and experimentation arm — to share what they're supporting, researching, and what didn't pan out. Also: "The future is multi-model. Trying to hide the choice confuses and hurts customers." Noted Safari 27's new JSPI WebAssembly support as a sign that more native code going through the browser will make WebAssembly increasingly important.
- <https://x.com/rauchg/status/2099911447598059812|Vercel Labs launch>
- <https://x.com/rauchg/status/2099905740505055680|On multi-model future>

*Aaron Levie* — CEO of Box
Published a detailed thread on the growing gap between AI model power and enterprise workflow automation. His thesis: the applied AI layer must connect intelligence to workflows, reengineer processes, aggregate data, handle human-in-the-loop moments, drive change management, run domain-specific evals, and manage security. "Even as models improve at incredible rates, this layer still must exist — and may become even more important." See the Training Data podcast below for the full conversation.
- <https://x.com/levie/status/2099976021311398230|View tweet>

*Garry Tan* — President & CEO of Y Combinator
Bullish on Muse winning the AI assistant race. Also sharing results with capy.ai: it finished a set of GitHub issue/PR fixes in about half the time that raw Codex or Claude Code would have taken, using the same frontier models.
- <https://x.com/garrytan/status/2099980972641124629|On Muse>
- <https://x.com/garrytan/status/2099964487667454097|On capy.ai>

*Nikunj Kothari* — Partner at FPV Ventures
Warning for founders: don't assume the funding spigot always flows. Advice: first lock in the default path that keeps your company alive and self-sustaining, then map out how capital abundance or scarcity changes that picture. Capital markets over the next 6–18 months are an unknown.
- <https://x.com/nikunj/status/2100008917980102863|View tweet>

*Dan Shipper* — CEO of Every
Flagged a model worth watching: one that produces probabilities rather than words as output. In Every's testing it's 25x faster and 600x cheaper than a Fable-level model while working well as an LLM judge. He called it "the kind of thing that will be obviously indispensable in 6–12 months."
- <https://x.com/danshipper/status/2099947471518474522|View tweet>

*Aditya Agarwal* — General Partner at SPC
Profound, which started at SPC and has grown to a $1.8B valuation, announced a $180M Series D co-led by Sequoia and Kleiner Perkins. The AI marketing platform now runs at one third of the Fortune 100.
- <https://x.com/adityaag/status/2099939685657141257|View tweet>

*Sam Altman* — CEO of OpenAI
Teasing a big ship week followed by even more releases at DevDay. No details, just ships.
- <https://x.com/sama/status/2099872600977760451|View tweet>

*Claude* — Anthropic's AI assistant
Salesforce in Claude launched in beta, bringing accounts, opportunities, and pipeline data directly into Claude with 37 pre-built sales skills. Use it to prep calls, review deals, create pipeline dashboards, or send forecasts without leaving the conversation.
- <https://x.com/claudeai/status/2099876514330206578|View tweet>

*OFFICIAL BLOGS*

*Claude Blog — "Claude for Small Business launches new workflows, integrations, and training programs"*

Claude for Small Business added 43 new workflows and 27 new integrations — including Shopify, Salesforce, TikTok, Atlassian, Zoom, Xero, Gusto, Square, Stripe, and Zapier — pushing coverage from back-office automation into business growth: lead generation, inbound inquiry handling, and proposal writing. The product has been installed more than 900,000 times since its May launch. A fall in-person workshop tour covers 10 US cities, with 150+ certified trainers running 750+ additional community sessions.

Owners who've used it report results like: "$20,000 in the last month and a half using Claude to do professional proposals" and cutting 120-hour tasks down to 5 minutes.

<https://claude.com/blog/claude-for-small-business-launches-new-workflows-integrations-and-training-programs|Read the full post>

*PODCASTS*

*Training Data — "Box's Aaron Levie: On Reinventing Yourself in the AI Age and Enterprise Diffusion"*

_The Takeaway:_ Between a frontier model and a fully automated enterprise workflow sits a massive, underappreciated gap — and filling that gap is where the biggest business opportunity in AI currently lives.

Box CEO Aaron Levie, who has spent 20 years building content and collaboration infrastructure for enterprises, argues that application layer companies — not just the model labs — are where the real value of this AI wave accumulates. His reasoning: AI models may be getting smarter fast, but real-world adoption constraints have nothing to do with model intelligence. Enterprises still need someone to connect the model to legacy data systems, manage access controls, retrain workflows, drive change management, and run domain-specific evals. "The model could be the most intelligent superintelligence in the world, but that workflow still requires you to connect up to other data systems, still requires moments where there's a human in the loop."

On the coding-vs-everything-else diffusion gap: coding agents spread fast because code's value is almost entirely in the text it produces, the audience is technical, the data lives in GitHub, and productivity gains are immediately measurable. Every other knowledge domain is harder — a sales rep's output is constrained by whether customers respond, not by how fast they type. Levie predicts 90% of enterprise tokens in five years will be tasks a user never kicked off; they'll just see a result show up.

Box runs domain-specific evals across life sciences, financial services, and tech, and ships a Box-tuned agent that consistently outperforms generic LLM calls on document-centric work. On the model race: Fable 5.1 is currently top for document tasks; Gemini over-indexes on tool use; open weights are growing but still quirky. His verdict: "I just don't know that one or two labs get 95% of the value creation — there's going to be a much more dynamic environment."

<https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8|Watch on YouTube>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
