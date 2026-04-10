*AI Builders Digest — April 10, 2026*


*X / TWITTER*

*Andrej Karpathy* (ex-Director of AI at Tesla, founding team at OpenAI)

Karpathy shared a detailed breakdown of how he's using LLMs to build personal knowledge bases. He indexes raw documents (articles, papers, repos, images) into a raw/ directory, then uses an LLM to compile a wiki of .md files — summaries, backlinks, categorized concept articles — all viewable in Obsidian. Complex Q&A runs against the wiki via CLI tools, and outputs (slides, markdown, charts) get filed back in, so explorations "always add up." He runs LLM health checks to find inconsistencies and suggest new articles. His conclusion: "I think there is room here for an incredible new product instead of a hacky collection of scripts." In a follow-up, he extrapolated: frontier LLMs could soon spawn whole teams of sub-LLMs to auto-build ephemeral wikis and write full reports for every query — "Way beyond a `.decode()`."

- <https://x.com/karpathy/status/2039805659525644595|LLM Knowledge Bases thread>
- <https://x.com/karpathy/status/2039808711452246261|Extrapolation: LLM spawning teams of LLMs>

*Box CEO Aaron Levie* (levie on X)

Levie shared hard-won lessons from building AI agents: be "brutally unsentimental" about your architecture. As models improve, scaffolding you built to compensate for their limitations becomes a drag — strip it to unlock new performance. He describes the loop: build scaffolding → models improve → strip scaffolding → new harder problems emerge → repeat. In Box Agent's development, multiple harness components had to be ripped out before launch because early mitigations started producing lower quality as models got better. "Always make sure you're taking advantage of the frontier capabilities and don't become nostalgic around the tech you've already built."

- <https://x.com/levie/status/2039931799414194621|Full thread on building AI agents>

*Ryo Lu* (ryolu_ on X) — Design at Cursor

Lu posted a manifesto on Cursor's "glass vs. black box" design philosophy: as AI becomes more powerful, visibility becomes more important, not less. Cursor lets you watch agents work, edit their plans, read every diff, and steer at any moment — "give away the wheel and you get mediocre, keep it and you get to build something great." He also announced Cursor 3: "Where power meets simplicity. Works across all your projects, local and cloud. It starts simple, then unfolds more tools when you need them."

- <https://x.com/ryolu_/status/2039895634313187619|Glass vs. Black Box manifesto>
- <https://x.com/ryolu_/status/2039780768847958359|Cursor 3 announcement>

*Sam Altman* (sama on X) — CEO at OpenAI

Altman called TBPN his favorite tech show and blessed their fundraise with dry self-deprecation: "I don't expect them to go any easier on us, am sure I'll do my part to help enable that with occasional stupid decisions."

- <https://x.com/sama/status/2039773740586918137|Tweet>

*Claude / Anthropic* (claudeai on X)

Computer use in Claude Cowork and Claude Code Desktop is now available on Windows.

- <https://x.com/claudeai/status/2039836891508261106|Tweet>

*Peter Steinberger* (steipete on X) — co-founder at OpenClaw

Steinberger flagged an alarming signal for open source: AI-generated security reports to the Linux kernel list have exploded from 2–3/week two years ago, to ~10/week last year, to 5–10 *per day* now — forcing maintainers to bring in extra help. His prediction: "This is gonna kill some OSS projects."

- <https://x.com/steipete/status/2039782190838686088|Tweet>

*Peter Yang* (petergyang on X) — Product at Roblox

Yang tried Cursor 3 and praised the cleaner interface: "The old one had far too many buttons and toggles that got in the way of just talking to the agent." He wonders why the streamlined view isn't the default.

- <https://x.com/petergyang/status/2039850011044016291|Tweet>

*Amjad Masad* (amasad on X) — CEO at Replit

Masad announced Replit is opening a sales office in Salt Lake City, Utah and is hiring.

- <https://x.com/amasad/status/2039777772701413396|Tweet>

*Dan Shipper* (danshipper on X) — CEO at Every

Shipper's team tested Cursor 3.0 for a week and published a full vibe check review.

- <https://x.com/danshipper/status/2039770244361662920|Tweet>


*PODCASTS*

*Training Data — How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly*

_The Takeaway: AI will do to biology what computers did to information — and Jason Kelly has been building the infrastructure for that for 17 years._

Jason Kelly, CEO of Ginkgo Bioworks, draws a sharp distinction most tech founders can't: every previous tech wave — the internet, social media — was essentially "back office IT crap" for biopharma. AI is categorically different. For the first time, it's changing the fundamental science.

Ginkgo's model is the "cell foundry": program DNA, and cells manufacture whatever you want. The same way factories automated physical production, Ginkgo is automating biology with robots on maglev tracks. The key insight isn't just more robots — it's utilization. Traditional labs run at sub-20% equipment utilization because they're organized around humans walking hallways to find available benches. Autonomous labs can hit 70%, centralize geographically, and fit in far less space. Ginkgo just sold 97 automated rack units to the Department of Energy for the government's AI-for-science initiative.

The bigger vision: democratize science the way the PC democratized computing. Ginkgo launched a Cloud Lab service where anyone can run experiments starting at $39 — no physical lab required, just order online and get data back. "Science is thought of as this very precious genius thing. But really what it is, is formalized human curiosity... What if everyday people could order an experiment?" Kelly draws the analogy: in the 1960s, saying kids would program computers sounded insane. Democratized biology may sound equally insane today.

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
