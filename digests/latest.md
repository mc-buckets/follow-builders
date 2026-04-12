AI Builders Digest — April 12, 2026


*X / TWITTER*

*Andrej Karpathy* (karpathy on X) — former Director of AI at Tesla, OpenAI founding team

Karpathy published a detailed breakdown of a workflow he's been finding increasingly useful: using LLMs to build personal knowledge bases. The setup: ingest raw source documents (articles, papers, repos, datasets, images) into a `raw/` directory, then have an LLM "compile" a wiki of `.md` files — summaries, concept articles, backlinks — viewable in Obsidian. From there, you can run complex Q&A against the wiki via CLI tools and have the LLM generate outputs like slides, charts, or markdown files that feed back into the wiki. He also runs LLM "health checks" to catch inconsistencies and surface new article candidates. His conclusion: "I think there is room here for an incredible new product instead of a hacky collection of scripts." A follow-up extrapolates the idea further: every frontier LLM query could spawn a whole team of LLMs to auto-build an ephemeral wiki, lint it, loop a few times, and write a full report — "Way beyond a `.decode()`."

- <https://x.com/karpathy/status/2039805659525644595|LLM Knowledge Bases thread>
- <https://x.com/karpathy/status/2039808711452246261|Follow-up: teams of LLMs>

*Aaron Levie* (levie on X) — CEO at Box

Levie laid out the core lesson from building Box Agent: be "brutally unsentimental" in your architecture. The loop he describes — build scaffolding → model improves and renders it redundant → strip it to unlock new gains → harder problems emerge → repeat — means yesterday's clever workaround is tomorrow's performance drag. They had to evolve multiple components of the Box Agent harness between original design and launch, because mitigations they'd built for earlier model limitations (chunking text for context windows, custom retrieval logic) actively created constraints once models got smarter. "Always make sure you're taking advantage of the frontier capabilities and don't become nostalgic around the tech you've already built."

- <https://x.com/levie/status/2039931799414194621|Full post on building AI agents>

*Ryo Lu* (ryolu_ on X) — Design at Cursor

Published a full manifesto on Cursor's "glass vs. black box" design philosophy alongside the Cursor 3 launch. His argument: AI kept the black box and made it more addictive — you type a wish, pull the lever, accept or reject the whole output. Glass breaks that open so that a PM can watch a plan become real, a new programmer can read every diff and build intuition, and an expert can let it flow and steer when something feels off. Same tool, infinite depth, your way. "As AI gets more powerful, glass gets more important. Not because you need to watch every move. But because the best work happens when you know you can." Cursor 3 ships with a simpler interface that unfolds more tools on demand, works local and cloud.

- <https://x.com/ryolu_/status/2039895634313187619|Glass vs. black box manifesto>
- <https://x.com/ryolu_/status/2039780768847958359|Cursor 3 announcement>

*Peter Steinberger* (steipete on X) — co-founder at OpenClaw

Flagged a data point with serious implications for open source sustainability: AI-generated security reports to the Linux kernel security list have gone from 2–3 per week two years ago, to ~10 per week last year, to 5–10 *per day* now — with Fridays and Tuesdays being the worst. What makes it particularly hard: most of the reports are correct, so maintainers can't just bulk-dismiss them. They've already had to bring in extra maintainers just to keep up. His prediction: "This is gonna kill some OSS projects."

- <https://x.com/steipete/status/2039782190838686088|AI flooding OSS maintainers>

*Amjad Masad* (amasad on X) — CEO at Replit

Three quick product and company updates: Replit opened a sales office in Salt Lake City, Utah and is hiring; launched a no-setup enterprise-grade auth solution; and shipped an SEO audit tool that runs on your site.

- <https://x.com/amasad/status/2039777772701413396|Salt Lake City office>
- <https://x.com/amasad/status/2039774118443421887|Enterprise auth>
- <https://x.com/amasad/status/2039838798671126728|SEO audit tool>

*Peter Yang* (petergyang on X) — Product at Roblox, AI newsletter writer

Tried Cursor 3 and called the new interface clearly better. The old one had "far too many buttons and toggles that got in the way of just talking to the agent." He questions why the cleaner view isn't the default rather than requiring a keyboard shortcut.

- <https://x.com/petergyang/status/2039850011044016291|Cursor 3 reaction>

*Dan Shipper* (danshipper on X) — CEO at Every

His team spent a week testing Cursor 3.0 and published a full vibe check.

- <https://x.com/danshipper/status/2039770244361662920|Cursor 3.0 vibe check>

*Sam Altman* (sama on X) — CEO at OpenAI

Called TBPN his favorite tech show and endorsed their acquisition with characteristic self-deprecation: "I don't expect them to go any easier on us, am sure I'll do my part to help enable that with occasional stupid decisions."

- <https://x.com/sama/status/2039773740586918137|Tweet>

*Swyx* (swyx on X) — AI builder, Latent Space podcast, AI Engineer

Reacted to TBPN's acquisition news with a half-joking pitch: "time for dario x dwarkesh?"

- <https://x.com/swyx/status/2039773480980480431|TBPN reaction>

*Garry Tan* (garrytan on X) — President & CEO at Y Combinator

Brief but notable: called Perplexity Computer "quite special actually."

- <https://x.com/garrytan/status/2039943351278190840|Perplexity Computer>

*Claude AI* (claudeai on X) — Anthropic

Computer use in Claude Cowork and Claude Code Desktop is now available on Windows.

- <https://x.com/claudeai/status/2039836891508261106|Windows computer use announcement>


*PODCASTS*

*Training Data — "How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly"*

_The Takeaway:_ A reasoning model paired with a robotic lab just beat the state-of-the-art scientific benchmark by 40% — and the reason it won wasn't that the AI was smarter than a human scientist. It was that it could run experiments continuously, share every data point across every line of inquiry, and never stop.

Jason Kelly founded Ginkgo Bioworks in 2008 straight out of MIT's bioengineering PhD program with a deceptively simple premise: DNA is code, cells are programmable like computers, and if you can design that code more effectively, you unlock a massive market. He bootstrapped for six years before landing in Y Combinator in 2014, after cold-emailing a then-less-famous Sam Altman.

His core conviction, sharpened over nearly two decades: every previous tech revolution was "totally meaningless to biotechnology and biopharma... just some back office IT crap." AI is categorically different — it's changing the fundamentals of how experimental science gets done.

The proof: Ginkgo partnered with OpenAI to test whether a reasoning model could run real experimental science using Ginkgo's autonomous robotic lab. They picked a published benchmark — optimizing cell-free protein synthesis — set by a Stanford lab. The model ran ~30,000 experiments per round, received raw data back, and designed the next round of experiments. After four rounds it beat the benchmark. After six rounds it beat it by 40%.

Kelly's insight is that the scientific method — form hypothesis, design experiment, collect data, iterate — is fundamentally just logic. It doesn't require modeling biology or simulating anything. "It just requires you to be almost like a programmer. You need to be logical, run through a set of things, do data analysis, and draw conclusions." The AI doesn't need to be more creative than a human; it just needs to be as good at designing experiments. And then it does what humans can't: run 100 parallel hypotheses simultaneously, share all raw data across every line of inquiry daily, and keep the lab running around the clock.

The structural economics are even more compelling than the intelligence argument. Today, less than 5% of research spending goes to reagents — the actual materials consumed by experiments. The rest is overhead: salaries, lab space, redundant equipment sitting idle 16 hours a day. Autonomous labs collapse that ratio, making an order-of-magnitude more science per dollar achievable.

_"All of the previous revolutions in tech — Internet, social media, whatever — have been totally meaningless to biotechnology and biopharma. Not this. This is actually going to change the fundamentals of how we do science."_

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
