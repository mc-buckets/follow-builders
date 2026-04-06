*AI Builders Digest — April 6, 2026*

*X / Twitter*

*Andrej Karpathy* — AI researcher (formerly Director of AI @Tesla, founding team @OpenAI)

Karpathy laid out a detailed workflow for using LLMs to build personal knowledge bases: ingest raw documents (articles, papers, repos, datasets) into a directory, have an LLM "compile" a wiki of structured .md files with summaries, backlinks, and concept articles, then run Q&A agents against it. He uses Obsidian as the IDE frontend and vibe-coded a naive search engine as a CLI tool for the LLM. At ~100 articles and ~400K words, complex queries become tractable without fancy RAG. He also floated that every frontier LLM query could eventually spawn an entire ephemeral wiki-building team to produce full reports — "Way beyond a `.decode()`." His parting thought: this rough collection of scripts deserves an incredible product.

- <https://x.com/karpathy/status/2039805659525644595|Full thread: LLM knowledge bases>
- <https://x.com/karpathy/status/2039808711452246261|On ephemeral wiki query teams>

*Aaron Levie* — CEO @Box

Levie shared the core loop of building AI agents: build scaffolding for the LLM → models improve and make that scaffolding redundant → ruthlessly remove it to recapture gains → repeat. For Box Agent, architecture had to evolve multiple times between design and launch because early mitigations (chunking strategies, custom retrieval) became harmful constraints as models got better. His bottom line: "Always make sure you're taking advantage of frontier capabilities and don't become nostalgic around the tech you've already built."

- <https://x.com/levie/status/2039931799414194621|Full thread: building AI agents>

*Ryo Lu* — Designer @Cursor

Ryo published a manifesto on "glass vs. black box" as Cursor 3 launched. His argument: the terminal was a black box; AI kept the box and made it more addictive; Cursor breaks it open. In the glass model, the plan is editable, the diff is visible, the agents are watchable and stoppable. "As AI gets more powerful, glass gets more important — not because you need to watch every move, but because the best work happens when you know you can." Cursor 3 ships with a simplified default interface that unfolds more tools on demand.

- <https://x.com/ryolu_/status/2039895634313187619|Glass vs. black box manifesto>
- <https://x.com/ryolu_/status/2039780768847958359|Cursor 3 launch>

*Peter Steinberger* — Co-founder @OpenClaw

Steipete flagged an alarming surge: AI-generated security bug reports to the Linux kernel mailing list have exploded from 2–3/week two years ago, to ~10/week last year, to 5–10 per day in early 2026 — and most are reportedly valid, forcing the kernel team to bring in extra maintainers. His prediction: "This is gonna kill some OSS projects."

- <https://x.com/steipete/status/2039782190838686088|On the AI security report surge>

*Amjad Masad* — CEO @Replit

Masad announced two moves: a new no-setup enterprise-grade auth solution, and the opening of a sales office in Salt Lake City. He also surfaced an AI-powered SEO audit tool built on Replit.

- <https://x.com/amasad/status/2039777772701413396|SLC sales office>
- <https://x.com/amasad/status/2039774118443421887|Enterprise auth solution>
- <https://x.com/amasad/status/2039838798671126728|SEO audit tool>

*Sam Altman* — CEO @OpenAI

Altman went on record that TBPN is his favorite tech show, framing OpenAI's involvement as wanting to keep it going — and explicitly not expecting them to go easier on OpenAI for it.

- <https://x.com/sama/status/2039773740586918137|On TBPN>

*Dan Shipper* — CEO @Every

Shipper's team ran a week-long vibe check of Cursor 3.0 and published their findings. He also cheered on folks grinding through product work.

- <https://x.com/danshipper/status/2039770244361662920|Every's Cursor 3.0 vibe check>

*Peter Yang* — Product @Roblox, AI newsletter author (140K+ readers)

Yang tried Cursor 3 and called the new simplified interface "much better" — the old one had too many buttons and toggles getting in the way of just talking to the agent. He questioned why the new view isn't the default.

- <https://x.com/petergyang/status/2039850011044016291|On Cursor 3's new interface>

*Swyx* — AI Engineer community (@aidotengineer), @Latent Space pod

Swyx noted that TBPN was apparently sold/acquired, congratulating the team and half-seriously calling for a Dario × Dwarkesh episode.

- <https://x.com/swyx/status/2039773480980480431|On TBPN>

*Garry Tan* — President & CEO @Y Combinator

Tan flagged Perplexity Computer as "quite special" and shared a brief riff on loving your work.

- <https://x.com/garrytan/status/2039943351278190840|On Perplexity Computer>
- <https://x.com/garrytan/status/2039948180977316164|On loving your work>

*Claude AI* — @Anthropic

Computer use in Claude.ai and Claude Code Desktop is now available on Windows.

- <https://x.com/claudeai/status/2039836891508261106|Computer use now on Windows>

*Podcasts*

*Training Data*

_How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly_

The Takeaway: AI won't just accelerate biology research — it'll restructure the entire experimental loop, enabling continuous 24/7 autonomous lab operation and unlocking the vast store of unpublished scientific knowledge.

Jason Kelly bootstrapped Ginkgo Bioworks for six years straight out of grad school before raising VC in 2014. His thesis has always been programmable biology. His conviction now: "All of the previous revolutions in tech — the internet, social media — have been totally meaningless to biotechnology. Not this."

Ginkgo partnered with OpenAI on cell-free protein synthesis optimization and achieved a 40% improvement over state-of-the-art results using reasoning models. The critical shift isn't just using AI to design biology faster — it's using reasoning models to explore experimental design space that humans wouldn't think to try, running continuously instead of 9-to-5.

The deeper unlock Kelly sees is information sharing. Science is hobbled by how little gets published versus how much gets done. Autonomous labs generate more data; AI can surface the patterns buried in failed experiments that never make it into journals. The result isn't just faster science — it's a fundamentally different information economy for research.

<https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8|How Autonomous Labs Will Transform Scientific Research — Training Data podcast>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
