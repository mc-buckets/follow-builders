AI Builders Digest — April 15, 2026

*X / TWITTER*

*Andrej Karpathy* — ex-Director of AI at Tesla, OpenAI founding team

Karpathy published one of his most widely shared posts in recent memory: a detailed walkthrough of using LLMs to build personal knowledge bases. His system ingests raw documents (articles, papers, repos, images) into a directory, then has an LLM "compile" them into a structured markdown wiki — complete with summaries, backlinks, and concept articles. He uses Obsidian as the viewing frontend, runs Q&A agents against the growing corpus, and loops LLM "health checks" to catch inconsistencies and surface new connections. His conclusion: "There is room here for an incredible new product instead of a hacky collection of scripts." He followed up with the natural extrapolation — frontier LLMs that spawn entire teams of LLMs to build ephemeral wikis, lint them, and write full reports in response to a single question.

- LLM knowledge base deep-dive: <https://x.com/karpathy/status/2039805659525644595>
- On LLM teams spawning ephemeral wikis: <https://x.com/karpathy/status/2039808711452246261>

*Aaron Levie* — CEO of Box

Levie shared a hard-won lesson from shipping Box Agent: building AI agents requires being "brutally unsentimental" about your architecture. His loop goes like this — build scaffolding to help the model handle specific tasks, watch the model improve and make that scaffolding redundant (or harmful), rip it out, unlock new capabilities, repeat. He cited concrete examples from Box Agent where their mitigations for early model limitations started producing lower quality results once the models got better. The main lesson: "Always make sure you're taking advantage of frontier capabilities and don't become nostalgic around the tech you've already built."

- <https://x.com/levie/status/2039931799414194621>

*Ryo Lu* — Designer at Cursor

Ryo announced Cursor 3 and paired it with a sharp manifesto on why transparency matters as AI gets more powerful. His "glass vs. black box" argument: the terminal was a black box, AI kept the box and made it more addictive, and Cursor breaks it open. The key line: "Give away the wheel and you get mediocre. Keep it and you get to build something great." Cursor 3 works across local and cloud projects, progressively reveals tools as needed, and keeps agents, diffs, and plans visible and editable.

- Cursor 3 launch: <https://x.com/ryolu_/status/2039780768847958359>
- Glass vs. black box manifesto: <https://x.com/ryolu_/status/2039895634313187619>

*Peter Steinberger* — Co-founder at OpenClaw

Steinberger flagged a signal that should concern anyone in open source: AI-generated security bug reports to the Linux kernel security list have jumped from 2–3 per week two years ago to 5–10 per day now — and many are technically valid. His prediction: the flood of AI-generated reports is going to overwhelm OSS maintainers and kill some projects. "Most of these reports are correct, to the point that we had to bring in more maintainers to help us," according to the kernel list. The volume problem, not the quality problem, is what's breaking things.

- <https://x.com/steipete/status/2039782190838686088>

*Peter Yang* — Product at Roblox, AI tutorials creator

Yang tested Cursor 3 and came away impressed by the cleaner interface — the old one had too many buttons and toggles getting in the way of just talking to the agent. His main question: why is the new simplified view hidden behind a keyboard shortcut (cmd+shift+p) instead of being the default?

- <https://x.com/petergyang/status/2039850011044016291>

*Amjad Masad* — CEO of Replit

Masad announced two moves this week: Replit launched a no-setup enterprise-grade auth solution for everyone, and opened a sales office in Salt Lake City. He also highlighted that Replit can now SEO-audit your site.

- Enterprise auth: <https://x.com/amasad/status/2039774118443421887>
- Salt Lake City office: <https://x.com/amasad/status/2039777772701413396>
- SEO audit: <https://x.com/amasad/status/2039838798671126728>

*Dan Shipper* — CEO of Every

Shipper's team spent a week testing Cursor 3.0 and published a full vibe check on Every.

- Cursor 3.0 vibe check: <https://x.com/danshipper/status/2039770244361662920>

*Garry Tan* — President & CEO of YCombinator

Tan called out Perplexity Computer as "quite special" — a brief but notable endorsement from the YC CEO given the competitive AI assistant landscape.

- <https://x.com/garrytan/status/2039943351278190840>

*Sam Altman* — CEO of OpenAI

Altman publicly backed TBPN — the tech news show — calling it his favorite tech show and noting OpenAI wants them to keep doing what they do well, including not going easy on OpenAI.

- <https://x.com/sama/status/2039773740586918137>

*Claude* — Anthropic's AI assistant

Computer use in Claude Code Desktop (and Claude.ai) is now available on Windows.

- <https://x.com/claudeai/status/2039836891508261106>

*PODCASTS*

*Training Data — How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly*

The takeaway: a reasoning model paired with a robotic lab just beat a Stanford benchmark for protein synthesis by 40% — and Jason Kelly thinks this is how we do all of science in 10 years.

Kelly founded Ginkgo Bioworks in 2008 to make biology programmable. He spent the first six years bootstrapping, pivoted into "foundry" infrastructure for biotech companies, and in the past two years has gone all-in on a single question: can you get the human being off the lab bench entirely?

The experiment that convinced him: Ginkgo partnered with OpenAI to test whether a reasoning model could run experimental science on its own. They gave the model a biochemistry problem — optimizing cell-free protein synthesis, essentially a miniature biological manufacturing process — and a robotic lab to run 384-well plates. After four rounds of experiment design, data collection, and autonomous re-design, the model beat the state-of-the-art Stanford benchmark. After six rounds, it beat it by 40%.

What the model did wasn't magic. "What really let it break through wasn't that it was so smart. It was that it could run experiments." The model designed experiments like a scientist, iterated logically on results, and kept going — 24 hours a day, sharing data across parallel hypotheses in real time.

Kelly's bigger argument cuts to the economics of science: today, less than 5% of a research budget goes to actual reagents — the chemicals and plastics you burn through doing experiments. Everything else is overhead: people, lab space, equipment sitting idle. In a robotic autonomous lab, that ratio flips. Suddenly you're spending 90% on reagents and almost nothing on overhead. That's a 10x increase in data per dollar — before you even factor in AI being faster or smarter than a human researcher.

His contrarian take: every previous tech revolution — internet, social media, mobile — was "totally meaningless to biotechnology and biopharma. Like, yeah, it's nice. We communicate slightly better or whatever. It's just some back office IT crap." This time is different. AI is the first tech shift that changes the fundamentals of how science gets done.

<https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
