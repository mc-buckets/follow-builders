AI Builders Digest — April 14, 2026

*X / TWITTER*

*Andrej Karpathy* (researcher, formerly Director of AI at Tesla and founding team at OpenAI)

In a major thread, Karpathy laid out his system for using LLMs to build personal knowledge bases: raw sources (articles, papers, repos, images) are collected into a `raw/` directory, then an LLM "compiles" them into a structured wiki of markdown files — summaries, backlinks, concept articles, all maintained automatically. He uses Obsidian as the frontend to browse and view the data, a CLI search engine he vibe-coded as a tool for LLM queries, and runs "health check" passes to find inconsistencies and suggest new connections. Key insight: at ~100 articles and ~400K words, he finds no need for fancy RAG — the LLM handles it. He sees a major product opportunity here that's currently just a collection of hacky scripts. In a follow-up, he extrapolated further: future LLMs spawning entire ephemeral wiki-building teams to answer a single complex query — "way beyond a `.decode()`."

- https://x.com/karpathy/status/2039805659525644595
- https://x.com/karpathy/status/2039808711452246261

*Aaron Levie* (CEO at Box)

Shared one of the most useful practitioner lessons on building AI agents: be "brutally unsentimental" about your architecture. The loop he describes — build scaffolding → model improves → scaffolding becomes redundant or harmful → strip it out → new capabilities emerge → repeat — is now the default rhythm of agent development. From the Box Agent experience: mitigations they built for finding data and chunking text ended up _lowering_ quality once the models got better. "The main lesson is always make sure you're taking advantage of the frontier capabilities and don't become nostalgic around the tech you've already built."

- https://x.com/levie/status/2039931799414194621

*Ryo Lu* (Designer at Cursor)

Announced Cursor 3 and shared the design philosophy behind it: "glass vs. black box." The terminal was a black box; AI kept the black box and made it more addictive. Cursor 3 breaks it open — agents are visible, diffs are shown, plans are editable, state is clear. "As AI gets more powerful, glass gets more important. Not because you need to watch every move. But because the best work happens when you know you can." The new interface starts simple and unfolds tools as needed, works across local and cloud projects.

- https://x.com/ryolu_/status/2039895634313187619
- https://x.com/ryolu_/status/2039780768847958359

*Peter Steinberger* (founder at Openclaw, formerly PSPDFKit)

Flagged a dramatic and under-discussed development: AI-generated bug reports are flooding the Linux kernel security list — from 2–3 per week two years ago to 5–10 per _day_ now. The reports are mostly correct, forcing the project to bring in more maintainers. His prediction: "This is gonna kill some oss projects."

- https://x.com/steipete/status/2039782190838686088

*Sam Altman* (CEO at OpenAI)

Commented on the TBPN acquisition, calling it his favorite tech show and expressing genuine support for them continuing hard-nosed coverage — including of OpenAI. Notably self-deprecating: "I don't expect them to go any easier on us, am sure I'll do my part to help enable that with occasional stupid decisions."

- https://x.com/sama/status/2039773740586918137

*Amjad Masad* (CEO at Replit)

Three product moves: Replit now does SEO audits for your site, launched a no-setup enterprise-grade auth solution, and opened a new sales office in Salt Lake City, Utah (hiring).

- https://x.com/amasad/status/2039838798671126728
- https://x.com/amasad/status/2039774118443421887
- https://x.com/amasad/status/2039777772701413396

*Dan Shipper* (CEO at Every)

Shared a week-long Cursor 3.0 vibe check from the Every team.

- https://x.com/danshipper/status/2039770244361662920

*Peter Yang* (Product at Roblox, creator)

Tried Cursor 3 and found the new interface significantly cleaner — far fewer buttons and toggles getting in the way of the agent. Questioned why the simplified mode isn't the default view.

- https://x.com/petergyang/status/2039850011044016291

*Claude* (Anthropic)

Computer use in Claude Code Desktop and Claude Cowork is now available on Windows.

- https://x.com/claudeai/status/2039836891508261106

*Garry Tan* (President & CEO at Y Combinator)

Brief endorsement: "Perplexity Computer is quite special actually."

- https://x.com/garrytan/status/2039943351278190840

*PODCASTS*

*Training Data — How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly*

_The Takeaway:_ Ginkgo Bioworks already has an AI reasoning model running autonomous experiments in a robotic lab — and after six rounds, it beat the Stanford benchmark for cell-free protein synthesis by 40%. This isn't a demo. It's a preview of how all experimental science gets done.

Jason Kelly, founder and CEO of Ginkgo Bioworks, spent 15 years building toward one goal: remove humans from the lab bench so science can actually scale. He's now convinced AI makes that possible, and he's more aggressive about the timeline than most scientists.

The key insight is structural, not technical. Today, labs are like a city where every car is custom-built for one driver. Equipment isn't shared. Experiments run five days a week, not twenty-four hours a day. Less than 5% of a typical research budget goes to actual reagents — the stuff you burn doing science. The rest is overhead: people, lab space, regulation. Autonomous robotic labs flip that ratio. If 90% of cost becomes reagents, you get roughly 10x more data per dollar — before the AI even has to be smarter than the human scientist.

The 40% improvement over Stanford's benchmark came from something simpler than clever AI: the model could run experiments. It didn't need to simulate biology or model molecular dynamics. It just needed to design experiments logically, get the data back, and iterate. "What really let it break through wasn't that it was so smart. It was that it could run experiments."

His vision for the near future: 100 AI scientists running in parallel on the same robotic lab, each pursuing a different hypothesis — say, for Alzheimer's — and sharing all raw experimental data with each other daily. Not polished papers every two years. Daily. Failed results from one line of inquiry become useful signal for another.

Kelly draws a direct analogy to Waymo. Traditional lab automation is like a subway — high efficiency, zero flexibility. Human scientists are like cars — fully flexible, fully manual. AI-powered autonomous labs are the Waymo moment: the flexibility of a car, the efficiency of the subway. "Every part of our physical infrastructure, post-industrial revolution — everything has to get looked at again with that lens."

Near-term applications he's most excited about: GLP-1 style consumer wellness drugs (not disease treatment — enhancement), longitudinal molecular monitoring (weekly blood tests vs. yearly doctor visits), and eventually, democratizing science entirely — letting everyday people design and run experiments the way kids today write code.

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
