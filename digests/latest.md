*AI Builders Digest — April 18, 2026*


*X / TWITTER*

*Andrej Karpathy* (former Tesla AI Director, OpenAI founding team)

Karpathy shared a detailed workflow for using LLMs to build personal knowledge bases — a method he's finding more useful than traditional RAG. The process: ingest raw documents (articles, papers, repos) into a directory, have an LLM "compile" a wiki of interconnected `.md` files with summaries and backlinks, then query the wiki with complex research questions. He uses Obsidian as the frontend and vibe-coded a small search engine the LLM can call as a CLI tool. He notes that as the repo grows, the natural next step is synthetic data generation and fine-tuning so the LLM "knows" the data in its weights. His conclusion: "I think there is room here for an incredible new product instead of a hacky collection of scripts."

Separately, he floated the idea that frontier LLM queries could naturally expand into spawning entire ephemeral teams of LLMs to research, lint, and write full reports — well beyond a simple decode().

- <https://x.com/karpathy/status/2039805659525644595|LLM Knowledge Bases thread>
- <https://x.com/karpathy/status/2039808711452246261|On LLM teams for queries>


*Aaron Levie* (Box CEO)

Levie shared the most clarifying framework yet for AI agent development: be "brutally unsentimental" about your architecture. His observed loop — build scaffolding around an LLM → models improve and render that scaffolding redundant → rip it out → new harder problems emerge → repeat. He says in building Box Agent, multiple components of the agent harness had to be replaced simply because earlier mitigations (for context chunking, search accuracy) started producing lower quality results once models got smarter. The lesson: "Always make sure you're taking advantage of the frontier capabilities and don't become nostalgic around the tech you've already built."

- <https://x.com/levie/status/2039931799414194621|Full thread>


*Ryo Lu* (Cursor Design)

Ryo announced Cursor 3 and published a manifesto on "glass vs. black box" design philosophy. The argument: AI tools have kept the black box — you type a wish, pull the lever, accept or reject the whole thing. Cursor 3 breaks that open so agents are visible, diffs are inspectable, plans are editable, and state is clear. "As AI gets more powerful, glass gets more important. Not because you need to watch every move. But because the best work happens when you know you can." Cursor 3 works across local and cloud projects.

- <https://x.com/ryolu_/status/2039780768847958359|Cursor 3 launch>
- <https://x.com/ryolu_/status/2039895634313187619|Glass vs. black box manifesto>


*Sam Altman* (OpenAI CEO)

Confirmed that OpenAI has backed TBPN (the tech podcast), calling it his "favorite tech show." He noted he doesn't expect the hosts to go easier on OpenAI as a result — and acknowledged he'll probably give them fresh material with "occasional stupid decisions."

- <https://x.com/sama/status/2039773740586918137|Tweet>


*Amjad Masad* (Replit CEO)

Announced three Replit expansions: a new SEO audit tool, a no-setup enterprise-grade auth solution, and a new sales office in Salt Lake City. Mostly product and hiring news.

- <https://x.com/amasad/status/2039838798671126728|SEO audit>
- <https://x.com/amasad/status/2039774118443421887|Enterprise auth>
- <https://x.com/amasad/status/2039777772701413396|SLC sales office>


*Peter Yang* (Roblox Product, Creator Science newsletter)

Noted that Cursor 3's new interface is a significant improvement — fewer buttons and toggles — and questioned why the simplified agent view isn't just the default.

- <https://x.com/petergyang/status/2039850011044016291|Tweet>


*Dan Shipper* (Every CEO)

Published Every's week-long vibe check of Cursor 3.0 after testing it ahead of launch.

- <https://x.com/danshipper/status/2039770244361662920|Cursor 3.0 vibe check>


*Peter Steinberger* (OpenClaw)

Flagged a concerning signal for open source projects: the Linux kernel security list is now receiving 5–10 AI-generated bug reports per day (up from 2–3 per week two years ago), with most being technically correct but requiring significant maintainer bandwidth to process. He predicts this pace will overwhelm some OSS projects.

- <https://x.com/steipete/status/2039782190838686088|Tweet>


*Garry Tan* (YC President & CEO)

Called Perplexity Computer "quite special" — a notable endorsement from one of tech's highest-signal voices.

- <https://x.com/garrytan/status/2039943351278190840|Tweet>


*Claude* (Anthropic)

Computer use in Claude Code Desktop is now available on Windows.

- <https://x.com/claudeai/status/2039836891508261106|Tweet>


*PODCASTS*

*Training Data — How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly*

*The Takeaway:* AI won't just make biotech faster — it will flip the economic model of science entirely, turning overhead-dominated research into reagent-dominated research and potentially democratizing lab access the way personal computers democratized programming.

Jason Kelly, founder and CEO of Ginkgo Bioworks, built the company from 2008 to make biology programmable — bootstrapping for six years before YC and Sam Altman convinced him that the Silicon Valley model could work for deep tech. For 15 years Ginkgo focused on two problems: making it cheaper to test biological designs, and making those designs more accurate. AI is now changing both, but Kelly has deliberately stepped back from the design side (where companies like Chai Bio and Arc Institute are competing) to focus entirely on the testing infrastructure — autonomous robotic labs.

The economic case is striking: today, less than 5% of a typical research budget goes to actual reagents (the materials consumed doing experiments). Everything else is overhead — people, lab space, equipment sitting idle nights and weekends. Autonomous labs running 24/7 could flip that ratio, getting 10x more data per dollar without models even needing to be smarter than human scientists.

Ginkgo currently runs what Kelly believes is a unique experiment: 50 scientists in Boston submitting jobs to a single centralized robotic setup. One breakthrough enabling this was using AI coding tools to replace visual programming environments like LabVIEW, which scientists universally hated. "From now on, the way we're going to interact with writing the code is through Claude Code or Codex. You will now submit a written protocol of what you want, and the model will figure it out."

Kelly's longer-term vision echoes the personal computer revolution: if lab access stops being gated by physical infrastructure, ordinary people with scientific curiosity could simply order experiments. The analogy he reaches for: in the 1960s, you'd have been called insane for predicting that kids would program computers.

<https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8|Watch on YouTube>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
