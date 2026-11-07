AI Builders Digest — November 7, 2026

*X / TWITTER*

*Thibault Sottiaux* (OpenAI Codex & ChatGPT engineer)
Bold prediction on the future of infrastructure: "I can confidently say that humans were not very good at writing secure infrastructure. The endstate will be hypersecure infrastructure and software for all, but we're going to go through some turbulence before we reach that." He also argues that formal proofs for tens of millions of lines of code are "not a ridiculous thing anymore" and should be factored into how new systems are designed.
- <https://x.com/thsottiaux/status/2118569235953893573|Hypersecure infrastructure is coming>
- <https://x.com/thsottiaux/status/2118569441860723112|Formal proofs at scale>

*Thariq* (formerly Claude Code at Anthropic)
Shared a high-signal agent prompt pattern that's getting traction: location-based reminders. His example — track when you've done laundry, then bug you 30 minutes after you get home on a weekday until you confirm or delay. Simple idea, but it illustrates what persistent agents can do that apps never could.
- <https://x.com/trq212/status/2118399561324699655|Location-based agent reminder example>

*Replit CEO Amjad Masad*
Replit's custom kernel build dodges 96% of Linux zero-day vulnerabilities — shared a post on their new sandbox design. Also claimed Replit is the only collaborative AI coding system out there.
- <https://x.com/amasad/status/2118503241390665776|Replit sandbox design>
- <https://x.com/amasad/status/2118506378440400951|Only collaborative AI coding system>

*Vercel CEO Guillermo Rauch*
Sees an emerging creator loop nearly closing: get an X subscription → build with Bot or Cursor → deploy to Vercel → distribute on X → monetize with X Money. He's also highlighting that Grok and Cursor can now build, deploy, and scale on Vercel. Separately, he's bullish on Vercel Schedules as "cron on steroids" for agents that do work over time — referencing Muse and Instinct as examples of agents that consolidate memories at night and remind you in the morning.
- <https://x.com/rauchg/status/2118474519925158186|The creator loop is closing>
- <https://x.com/rauchg/status/2118464177211940997|Grok and Cursor deploy to Vercel>
- <https://x.com/rauchg/status/2118440831355068671|"Doing stuff for you over time" is the killer app>

*Box CEO Aaron Levie*
Enterprise AI prediction: we'll have 100X more agents than people working with enterprise data and systems. The core constraint is that 90% of enterprise data is unstructured — living in documents, contracts, and research files. Announced a partnership with NVIDIA for advanced context retrieval in Box, combining lexical and semantic search with enterprise security and access controls so agents can find the right information without overstepping permissions.
- <https://x.com/levie/status/2118498574497665316|Box × NVIDIA enterprise context retrieval>

*YC President & CEO Garry Tan*
Post-election take: a rare bipartisan window to curb Big Tech's market power abuse. His argument — inventing powerful AI is only half the job; people need to actually be able to use it, and trillion-dollar distribution moats block that. Calls on Congress to let thousands of startups compete. Also flagged a new "first long horizon benchmark for PE/IB work," saying that solving high finance is on the path to AGI.
- <https://x.com/garrytan/status/2118557763156733984|Open markets for Little Tech>
- <https://x.com/garrytan/status/2118527182092071179|High finance benchmark for AGI path>

*Peter Steinberger* (OpenClaw + OpenAI)
Questioning Apple's Safari narrative: "Is my perception off or is Apple just lying here? Anytime I build for or use Safari, it's slower, has fewer features, weird bugs and plenty websites just don't work."
- <https://x.com/steipete/status/2118492097917628704|Safari vs Chrome take>

*Anthropic (claudeai)*
Launched Personal Finance in Claude, now in beta for US users. Connect your financial accounts and ask Claude about your balances and transactions in plain language. Access is read-only — Claude can't move, manage, or invest money. No ads, no sponsored recommendations. Rolling out gradually on Pro, Max, and Ultra plans.
- <https://x.com/claudeai/status/2118403114890137895|Personal Finance launch>
- <https://x.com/claudeai/status/2118403117779988744|No ads, read-only, gradual rollout details>

*Swyx* (smol_ai, Cognition, Latent Space)
Provided context on a confusing Sequoia-related situation: says there was a communication gap on his end and inaccuracies in a quoted tweet he can't fully address publicly. Clarifies the situation is unrelated to the broader Sequoia restructuring announced this week. Also recommending Britt Walker as a scout for founders looking for a sharp, experienced partner.
- <https://x.com/swyx/status/2118538896434999759|Sequoia situation context>
- <https://x.com/swyx/status/2118542845556691411|Scout recommendation for Britt Walker>

*SPC General Partner Aditya Agarwal*
Shared a sharp reminder for founders: "Just because someone is willing to invest at a certain valuation doesn't mean it's the right valuation for your company." Also shared a full conversation with Trae Stephens at SPC.
- <https://x.com/adityaag/status/2118477020325884357|Valuation discipline reminder>
- <https://x.com/adityaag/status/2118477023891058762|Full conversation with Trae Stephens>

*Every CEO Dan Shipper*
Announced Thesis 2027, a live event in Brooklyn.
- <https://x.com/danshipper/status/2118421854666838338|Thesis 2027 — live from Brooklyn>

*PODCASTS*

*Unsupervised Learning — Ep 97: Jev Creator on Decision Models, Benchmark Fatigue & Why the Labs Missed It*

*The Takeaway:* The AI field is suffering from a kind of Stockholm syndrome — developers plan around whatever model providers ship instead of demanding what they actually need, and that dynamic is holding back software more than any capability gap.

Jogo, CEO of TypeSave (makers of JEV), became one of the more watched voices in AI after a viral launch about a month ago. He's building what he calls "system one" decision models — not LLMs optimized for human-readable prose, but models designed for machine consumption: fast, reliable, structured outputs that software can depend on. His core argument: the vast majority of LLM calls in the future will be for computers, not people. Strings are almost never what a computer wants. The field built for the minority use case first.

His most contrarian takes from the conversation:

- *Benchmark fatigue arrived faster than expected.* People have already been burned so many times by models that crush benchmarks but disappoint in production that they've stopped caring about new releases. He sees that as bad for the field (genuinely good things get ignored) but good for JEV specifically.

- *The shape of the task matters less than its reliability.* Everyone rushing to build new "shapes" of models is missing the point — it took about a week to build the architecture; the years of work are in making it actually useful.

- *Coding agents give 20–40% productivity gains on average* — decent but far from the transformations being priced in. For some tasks it's infinite leverage; for others, it's as slow as writing code by hand.

- *Anthropic's greatest strength may be financial engineering,* not models or product — specifically how they structure compute deals.

- On Anthropic's IPO: "The let them cure cancer is going to be like Marie Antoinette's let them eat cake."

He also went deep on what he calls the "tyranny of the KV cache" — how nearly every coding agent design decision is constrained by the append-only nature of context. His vision: agents that share context in real time, semantic compaction that reorganizes state around the new task instead of blindly truncating, and distributed history shared across a team's coding sessions.

"I get the sense that a lot of the expectations baked in are ones that are not just product level, but based on misunderstandings of the future of AI and what it can do."

<https://www.youtube.com/@RedpointAI|Unsupervised Learning on YouTube>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
