AI Builders Digest — July 12, 2026


*PODCASTS*

*The MAD Podcast with Matt Turck — "Stripe's AI Chief: How AI Agents Will Buy, Sell, and Pay"*

*The Takeaway:* Token theft — not payment fraud — is the most underrated existential threat in AI right now, with more than one in six signups at AI companies being some form of abuse.

Emily Sens is head of data and AI at Stripe, sitting at one of the best data vantage points in the AI economy: Stripe processes roughly 2% of global GDP, and the density of AI buyers and sellers on their network gives her insight that most analysts can only speculate about.

The conventional framing of agentic commerce is that AI agents will eventually shop for us. Sens reframes it as a full spectrum — from a human clicking "buy" after an AI recommendation, all the way to a fully autonomous agent that discovers, negotiates, purchases, and integrates a service without any human in the loop. She's built a literal L1–L5 framework for this (mirroring self-driving car autonomy levels). Today most consumer activity hovers around L2. The harder story is what infrastructure has to exist to support every level of that spectrum, and that's what Stripe's agentic commerce suite is building for.

The underreported story she keeps coming back to is token theft. Fraudsters don't need to steal money or credentials anymore — they just steal tokens, which have real resale value. Three active abuse patterns she tracks: multi-account abuse (spinning up fake accounts to drain new-user credits), free trial abuse (which has more than doubled on Stripe in six months, mostly driven by AI companies), and usage-based dine-and-dash (racking up thousands in token costs and vanishing). There are Taobao marketplaces where stolen tokens get packaged and sold as competing AI products, sometimes as full clones of the original service.

> "Fraudsters have figured out that in AI, you actually don't really need to steal money or credentials. You can just steal tokens. And the scale of this actually shocked me when I looked at the data. More than one in six signups at AI companies are this kind of abuse."

On the macro: new business registrations are up 80% in France and 70% in Finland, and Stripe Atlas startups from the 2026 cohort are tracking to *five times* the revenue of last year's class at the same point in their lifecycle. Vibe coding is effectively solved — agent traffic is now 40% of Stripe's documentation traffic and 70% of CLI API requests come from agents, not developers. The bottleneck has shifted to *vibe deployment*: getting an app live still requires bouncing between database, auth, and hosting dashboards, all designed for humans clicking through setup wizards. Stripe Projects addresses this by letting agents provision Vercel, Supabase, Cloudflare, Clerk, and 16+ other partners directly from the command line.

On billing: per-seat SaaS models are breaking for AI companies because marginal costs are no longer near-zero — every prompt costs real money. Most scaled AI companies now run hybrid models: a fixed subscription up to a credit threshold, then usage-based billing above it. The future she's most excited about is real-time streaming payments (built with Metronome for metering and Tempo blockchain for instant micro-settlements in stablecoins), so agents can pay down token costs as they're consumed rather than running up a month-end invoice they may never honor.

On where agentic commerce lands in 12 months: not just an agent that buys things for you, but an agent that runs a business — buying, selling, provisioning infrastructure, and generating profit. She calls this the "agent as micro-firm" model, and thinks we'll see early real examples of it before the end of 2026.

https://www.youtube.com/@DataDrivenNYC/videos


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
