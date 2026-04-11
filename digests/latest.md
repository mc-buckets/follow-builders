AI Builders Digest — April 11, 2026


*X / TWITTER*

*Andrej Karpathy* (karpathy on X) — former Director of AI at Tesla, OpenAI founding team

In a thread that landed 18K+ likes, Karpathy walked through his workflow for using LLMs to build personal knowledge bases. The setup: ingest raw sources (articles, papers, repos, images) into a `raw/` directory, have an LLM compile them into a wiki of `.md` files in Obsidian — summaries, backlinks, categorized concept articles — then run complex Q&A against the wiki via CLI tools rather than reaching for RAG. Outputs (slides, charts, markdown) get filed back into the wiki, so explorations "always add up." He runs LLM health checks to surface inconsistencies and suggest new articles. His conclusion: "I think there is room here for an incredible new product instead of a hacky collection of scripts." In a follow-up, he extrapolates the next step: every frontier query could spawn a whole team of LLMs to auto-build an ephemeral wiki, lint it, and deliver a full report — "Way beyond a `.decode()`."

- <https://x.com/karpathy/status/2039805659525644595|LLM Knowledge Bases thread>
- <https://x.com/karpathy/status/2039808711452246261|Follow-up on teams of LLMs>

*Aaron Levie* (levie on X) — CEO at Box

Levie shared hard-won lessons from building AI agents: be "brutally unsentimental" about your architecture. As models improve, the scaffolding you built to compensate for their earlier limitations doesn't just become unnecessary — it actively hurts performance. The loop he describes: build scaffolding → model improves and renders it redundant → strip it to unlock new gains → harder problems emerge → repeat. He saw this firsthand with Box Agent, where multiple harness components had to be ripped out before launch as models got better at complex reasoning, tool use, and context handling. "Always make sure you're taking advantage of the frontier capabilities and don't become nostalgic around the tech you've already built."

- <https://x.com/levie/status/2039931799414194621|Full post on building AI agents>

*Ryo Lu* (ryolu_ on X) — Design at Cursor

Published a full manifesto on Cursor's "glass vs. black box" design philosophy. His argument: AI made the black box more addictive — you type a wish, pull a lever, and accept or reject the output whole. Glass breaks that open. Cursor shows you agent state, diffs, plans — everything is editable and stoppable. The same tool, he argues, surfaces different depth for different people: PMs see a plan come to life, new programmers read every diff and build intuition, experts let it flow and steer when something feels off. As AI gets more powerful, visibility gets more important, not less. He also announced Cursor 3 — simpler interface that unfolds more tools on demand, works local and cloud.

- <https://x.com/ryolu_/status/2039895634313187619|Glass vs. black box manifesto>
- <https://x.com/ryolu_/status/2039780768847958359|Cursor 3 announcement>

*Peter Steinberger* (steipete on X) — co-founder at OpenClaw

Flagged an alarming data point for open source sustainability: AI-generated security reports to the Linux kernel list have exploded — from 2–3 per week two years ago, to ~10 per week last year, to 5–10 *per day* now. What makes it worse: most of the reports are correct, forcing maintainers to bring in extra help just to keep up with the volume. His prediction: "This is gonna kill some OSS projects."

- <https://x.com/steipete/status/2039782190838686088|AI flooding OSS maintainers>

*Amjad Masad* (amasad on X) — CEO at Replit

Announced Replit opened a sales office in Salt Lake City, Utah and is hiring. Also promoted two new capabilities: a no-setup enterprise-grade auth solution and an SEO audit tool that runs on your site.

- <https://x.com/amasad/status/2039777772701413396|Salt Lake City office>
- <https://x.com/amasad/status/2039774118443421887|Enterprise auth>
- <https://x.com/amasad/status/2039838798671126728|SEO audit tool>

*Peter Yang* (petergyang on X) — Product at Roblox, AI newsletter writer

Tried Cursor 3 and praised the cleaner interface — "far too many buttons and toggles" in the old one got in the way of just talking to the agent. He wonders why the streamlined view isn't the default instead of requiring a keyboard shortcut. Also joked that someone should build a Tron-aesthetic IDE or terminal skin.

- <https://x.com/petergyang/status/2039850011044016291|Cursor 3 reaction>

*Dan Shipper* (danshipper on X) — CEO at Every

His team spent a week testing Cursor 3.0 and published a full vibe check. Also shared encouraging updates on an unnamed project getting its icons filled out — "just keep going."

- <https://x.com/danshipper/status/2039770244361662920|Cursor 3.0 vibe check>

*Sam Altman* (sama on X) — CEO at OpenAI

Called TBPN his favorite tech show and endorsed their acquisition deal with dry self-deprecation: "I don't expect them to go any easier on us, am sure I'll do my part to help enable that with occasional stupid decisions."

- <https://x.com/sama/status/2039773740586918137|Tweet>

*Swyx* (swyx on X) — AI builder, Latent Space podcast, AI Engineer

Reacted to news of TBPN being acquired, half-jokingly asking if it's time for a "Dario x Dwarkesh" crossover episode. Also shared a quote tweet riffing on how low prices can go in the current AI market.

- <https://x.com/swyx/status/2039773480980480431|TBPN acquisition reaction>
- <https://x.com/swyx/status/2039812100206604787|How low is low>

*Garry Tan* (garrytan on X) — President & CEO at Y Combinator

Called Perplexity Computer "quite special." Also shared a quote tweet about loving your work.

- <https://x.com/garrytan/status/2039943351278190840|Perplexity Computer>

*Nan Yu* (thenanyu on X) — Head of Product at Linear

Floated "TBPN for sports" as a concept worth building. Also posted a couple of quote tweets on how AI can flexibly step into the role of a PM or product marketer on demand.

- <https://x.com/thenanyu/status/2039832290490994970|TBPN for sports>

*Claude AI* (claudeai on X) — Anthropic

Announced that computer use in Claude Cowork and Claude Code Desktop is now available on Windows.

- <https://x.com/claudeai/status/2039836891508261106|Windows computer use announcement>


*PODCASTS*

*Training Data — "How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly"*

_The Takeaway:_ AI reasoning models paired with robotic labs can already outperform human scientists on experimental benchmarks — and the advantage isn't that AI is smarter, it's that it never sleeps, never hoards data, and nearly eliminates overhead costs.

Jason Kelly, founder and CEO of Ginkgo Bioworks, has spent 17 years trying to make biology easier to engineer — treating DNA as code and cells as programmable factories. He bootstrapped the company for six years after founding it straight out of MIT's bioengineering PhD program, eventually landing in Y Combinator in 2014 after cold-emailing a then-lesser-known Sam Altman.

His core conviction, sharpened over those years: every previous tech revolution was "back office IT crap" for biopharma. AI is categorically different — it's changing the fundamentals of how science gets done.

The evidence: Ginkgo partnered with OpenAI to test whether a reasoning model could run experimental science using a robotic lab. They picked a biochemistry benchmark — optimizing cell-free protein synthesis — set by a Stanford lab in August 2023. The AI ran batches of ~30,000 experiments per round, designing the next set based on data from the last. After four rounds, it beat state of the art. After six, it beat it by 40%.

Kelly's key insight is that the scientific method — form hypothesis, design experiment, collect data, iterate — is fundamentally just logic. You don't need to model biology or simulate anything. The AI doesn't have to be more creative than a human scientist; it just needs to design experiments like one. And then it does something humans can't: run 100 parallel experiments daily, share all the raw data across every line of inquiry, and keep going 24 hours a day.

The structural advantage is even bigger than the intelligence argument. Today, less than 5% of research spending goes to reagents — the actual materials you consume doing experiments. The rest is overhead: lab space, people, and equipment sitting idle 16 hours a day. Autonomous labs flip that ratio, making 10x more data per dollar possible.

_"All of the previous revolutions in tech — Internet, social media, whatever — have been totally meaningless to biotechnology and biopharma... Not this. This is actually going to change the fundamentals of how we do science."_

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
