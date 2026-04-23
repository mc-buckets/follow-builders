AI Builders Digest — April 23, 2026


*X / TWITTER*

*Andrej Karpathy* — former Tesla AI Director, independent AI researcher

Karpathy shared a detailed workflow for using LLMs to build personal knowledge bases — and it's become one of his primary uses of AI lately. The setup: ingest raw source material (articles, papers, repos, images) into a directory, then have an LLM "compile" it into a structured wiki of markdown files with summaries, backlinks, and concept articles, all viewable in Obsidian. Once the wiki grows large enough (~100 articles, ~400K words), you can query it with LLM agents for complex research questions — no fancy RAG required. He also runs "health checks" to find inconsistencies and surface new article candidates. His conclusion: "I think there is room here for an incredible new product instead of a hacky collection of scripts." He followed up with the natural extrapolation: every question to a frontier LLM could spawn a team of LLMs to construct an entire ephemeral wiki, lint it, loop a few times, and write a full report.
- <https://x.com/karpathy/status/2039805659525644595|Full knowledge base thread>
- <https://x.com/karpathy/status/2039808711452246261|Ephemeral wiki extrapolation>


*Aaron Levie* — Box CEO

Levie shared his sharpest lesson from building AI agents at Box: be "brutally unsentimental" in your architecture. The cycle is: build scaffolding around LLMs to solve specific tasks → models dramatically improve, rendering that scaffolding redundant or harmful → strip it out to unlock new performance → new model capabilities open harder problems → repeat. On the Box Agent, components baked into the original architecture had to be ripped out before launch because they were creating unnecessary constraints as models got better at reasoning, search, and handling context windows. "Always make sure you're taking advantage of the frontier capabilities and don't become nostalgic around the tech you've already built."
- <https://x.com/levie/status/2039931799414194621|Full thread>


*Ryo Lu* — Design at Cursor

Lu published a long manifesto on Cursor's "glass vs. black box" philosophy, timed with the Cursor 3 launch. The argument: AI tools kept the black box and made it more addictive — you type a wish, pull a lever, accept or reject the whole thing. "You see less and think less as the model became better. You became a product of the model." Cursor bets the other direction: visible agents, editable plans, stoppable diffs, nothing hidden. "As AI gets more powerful, glass gets more important. Not because you need to watch every move. But because the best work happens when you know you can." Cursor 3 works across local and cloud projects, starts simple, and surfaces more tools progressively as you need them.
- <https://x.com/ryolu_/status/2039895634313187619|Glass vs. black box essay>
- <https://x.com/ryolu_/status/2039780768847958359|Cursor 3 launch tweet>


*Peter Steinberger* — AI builder, ClawFather

Steinberger flagged a signal worth watching: the Linux kernel security list is now receiving 5–10 AI-generated bug reports per day, up from 2–3 per week two years ago. Notably, most are technically correct — which means maintainers have to actually process them. His prediction: the sustained volume will kill some OSS projects that can't absorb the overhead.
- <https://x.com/steipete/status/2039782190838686088|Tweet>


*Peter Yang* — AI tutorials creator, 140K+ newsletter readers

Yang tried Cursor 3 and liked the direction: the old interface had too many buttons and toggles that got in the way of just talking to the agent. He thinks the simplified view should simply be the default instead of hidden behind a keyboard shortcut.
- <https://x.com/petergyang/status/2039850011044016291|Tweet>


*Dan Shipper* — Every CEO

Shipper's team ran a week-long test of Cursor 3.0 before launch and published their full vibe check.
- <https://x.com/danshipper/status/2039770244361662920|Tweet with link to vibe check>


*Amjad Masad* — Replit CEO

Two product moves from Masad: Replit now offers a no-setup enterprise-grade auth solution, and the company has opened a sales office in Salt Lake City, Utah.
- <https://x.com/amasad/status/2039774118443421887|Auth announcement>
- <https://x.com/amasad/status/2039777772701413396|SLC office tweet>


*Sam Altman* — OpenAI CEO

Altman called TBPN his favorite tech show and said OpenAI wants it to keep going — including not going any easier on them. He deadpanned he'll keep providing material with "occasional stupid decisions."
- <https://x.com/sama/status/2039773740586918137|Tweet>


*Claude* — Anthropic

Computer use in Claude Cowork and Claude Code Desktop is now available on Windows.
- <https://x.com/claudeai/status/2039836891508261106|Announcement>


*Swyx* — AI engineer, Latent Space podcast

Reacted to TBPN selling their podcast with a half-joking question: "time for dario x dwarkesh?" Also posted a cryptic pricing reaction — "HOW LOW IS LOW / HOW LOW / IS LOW" — suggesting significant AI cost compression in the news.
- <https://x.com/swyx/status/2039773480980480431|TBPN tweet>
- <https://x.com/swyx/status/2039812100206604787|Pricing reaction>


*Nan Yu* — Head of Product at Linear

Posted a brief set of observations framing AI as a flexible collaborator that can serve as a PM, product marketer, or whatever role you need in the moment. Also pitched a half-joke concept: TBPN for sports.
- <https://x.com/thenanyu/status/2039832290490994970|TBPN for sports>
- <https://x.com/thenanyu/status/2039823494398001448|AI as PM>
- <https://x.com/thenanyu/status/2039820803722633589|AI as product marketer>


*Garry Tan* — Y Combinator President & CEO

Brief take: called Perplexity Computer "quite special."
- <https://x.com/garrytan/status/2039943351278190840|Tweet>


*PODCASTS*

*Training Data — "How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly"*

*The Takeaway:* AI reasoning models paired with robotic labs can already beat state-of-the-art benchmarks in experimental biology — and the implications for how we do science globally are enormous.

Jason Kelly, founder and CEO of Ginkgo Bioworks, has spent nearly two decades on a single premise: DNA is code (ATCGs, not zeros and ones), cells are programmable like computers, and if you can engineer biology the way you engineer software, you unlock an enormous market. Unlike computers that move information, cells move atoms — meaning if you can program them, you can build physical things. The challenge is that "our ability to program cells today is really bad," and improving it requires physical lab experiments, not just simulations.

That bottleneck is now cracking. Ginkgo partnered with OpenAI to run an AI reasoning model against their autonomous robotic lab on a real biochemistry challenge: optimizing cell-free protein synthesis, a technique used in drug development. The model designed experiments in batches, received raw data back, and iterated. After four rounds it surpassed the Stanford-set state of the art. After six rounds, it beat that benchmark by 40%.

The counterintuitive part: the model wasn't especially clever. It just did what scientists do — form a hypothesis, design an experiment, get data, interpret it, iterate — but it could do it continuously, at scale, without rest. "What really let it break through wasn't that it was so smart. It was that it could run experiments. The question was just, could it design them like a scientist could? And the answer was, hell yeah."

Kelly's bigger vision is a transformation of scientific collaboration itself. Today, dozens of labs work in parallel on the same disease, publishing distilled results every year or two. He imagines replacing this with 100 AI scientists inside one autonomous lab, each pursuing a different hypothesis, sharing raw experimental data with each other daily — not waiting for the filtered version in a paper. "Your failed result might be relevant to my hypothesis, and I would never see that normally." His contrarian note: humanoid robots are wrong for biology. Purpose-built track systems outperform bipedal walkers in a microscale discipline every time.

<https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8|Watch on YouTube>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
