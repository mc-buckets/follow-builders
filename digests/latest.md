AI Builders Digest — May 25, 2026

*X / TWITTER*

*Thariq (Claude Code at Anthropic)*
Thariq ran Claude's "please save me money" prompt against the legacy codebase of his old startup OMMultiverse — and it actually worked. He noted that he occasionally remembers this capability exists and is surprised every time it delivers real cost savings on a codebase he hasn't had time to maintain.
- https://x.com/trq212/status/2058377974882210096
- https://x.com/trq212/status/2058380417716125966

*Amjad Masad (CEO at Replit)*
Masad amplified a user story that cuts to Replit's core pitch: a developer built their first mobile app MVP in a single weekend using Replit for Dial, and it passed Apple's App Store review on the very first submission — something that had never happened to them before, even using Cursor.
- https://x.com/amasad/status/2058418731840159953

*Guillermo Rauch (CEO at Vercel)*
Rauch ran a crowdsourced survey asking followers to share the AI-built product they're most proud of and which model they used — drawing 1,558 replies. After processing 1,400 of them, his takeaway: OpenAI is closing the mindshare gap with Anthropic; "Codex" got more tool mentions than "Claude Code." But ranked by underlying model, Anthropic's models are still dominant. The original prompt became its own signal — 2,195 likes suggests the builder community is eager to show what they're making.
- https://x.com/rauchg/status/2058245330836271263
- https://x.com/rauchg/status/2058353051073970416

*Aaron Levie (CEO at Box)*
Levie made a pointed argument against AI job-loss predictions: we keep confusing task completion with job elimination. When AI automates tasks within a job, the job doesn't disappear — it expands to do more of those tasks, at higher quality, or shifts to what hasn't been automated yet. A small business that couldn't afford a marketing agency can now hire one marketer who operates at agency-level output. "Don't fall into the trap of confusing tasks with jobs."
- https://x.com/levie/status/2058223867815227756

*Garry Tan (President & CEO at YCombinator)*
Tan dropped new benchmark results for his GBrain memory system: it beats MemPalace by 1% on LongMemEval and outperforms Vector RAG by 38% on retrieval success. He also fine-tuned his own Qwen3.5-397B model in a couple of hours using Thinking Machines, calling fast usable multimodal "mind-blowing" for personal AI. On the civic front, he's pledging $50K through Garry's List Action to fight political opposition to startups remaining in San Francisco, and is looking for 9 others to match him.
- https://x.com/garrytan/status/2058448209027141709
- https://x.com/garrytan/status/2058378310254793013
- https://x.com/garrytan/status/2058251537298980992

*Nikunj Kothari (Partner at FPV Ventures)*
Kothari flagged that a piece he wrote nearly a year ago — arguing that B2B companies need strong narrative and "vibes" to stand out — is finally landing. He's now seeing more companies wake up to the idea. His core thesis: in a world flooded with AI-generated sameness, distinctive brand storytelling is becoming a genuine competitive moat.
- https://x.com/nikunj/status/2058203594672021769

*Peter Steinberger (creator of OpenClaw)*
Steinberger built and released a public GitHub dashboard showing your repos, open Issues/PRs, last release version, and commits since last release. He also shared a practical Codex tip: tell it to maintain a scratch-log during bigger refactors — documenting decisions made, tradeoffs taken, and things you forgot to specify — so you can review the agent's reasoning after the fact.
- https://x.com/steipete/status/2058381186884411473
- https://x.com/steipete/status/2058308112134635528

*Aditya Agarwal (General Partner at South Park Commons)*
Agarwal captured the pace of the moment in one stark observation: six months ago in November 2025, the cutting edge was chatting with LLMs and being impressed by that alone. By May 2026, AI systems have produced more code in aggregate than all human-written code across history. A stark marker of how fast the baseline has shifted.
- https://x.com/adityaag/status/2058233900464238801


*PODCASTS*

*No Priors — "The Story Behind Cerebras' $63 Billion IPO with Founder and CEO Andrew Feldman"*

*The Takeaway:* Cerebras built the world's fastest AI inference hardware years before anyone cared — and survived long enough to be exactly right when the market finally caught up.

Andrew Feldman is the co-founder and CEO of Cerebras Systems, which recently went public at a $63 billion market cap. Cerebras builds "wafer-scale" chips — each one roughly the size of a dinner plate, compared to the postage-stamp-sized chips everyone else makes — delivering AI inference speeds 15 to 20x faster than GPUs, across big models, small models, US and Chinese models alike.

The core lesson from Feldman's story is about timing and patience. Being right early is indistinguishable from being wrong. Cerebras had a radically superior chip by 2019 but spent years selling almost nothing because AI models weren't yet useful enough for speed to matter. From 2023 to early 2025, people pointed at AI but didn't use it daily. The moment daily use became real — coding assistants, agents, integrated workflows — demand exploded and Cerebras was the only hardware company ready for it. "How big is the market for slow search? It's zero."

The architectural conviction matters too. Feldman's bet from the start: to be 15-20x better than a GPU, you can't make incremental improvements. "To be radically better, you can't build something that is a similar architecture... your design has to be different." Industry veterans called it impossible for years.

A sovereign wealth fund (G42 in the UAE) provided the critical bridge: a $1 billion order that let Cerebras scale manufacturing, battle-test at cluster size, and survive the gap between niche early adopters and mainstream demand. Without it, the $20B+ OpenAI deal and the AWS deployment agreement that followed couldn't have been fulfilled.

On AI-assisted coding inside Cerebras: Feldman sees a sharp split in his 850-person company. A small number of engineers running 8 to 10 parallel agents have gone from "10x to 100x" productivity — they've restructured their entire workflow around governing agents rather than writing code directly. Most others are still figuring out how to adapt.

His vision for what fast inference unlocks isn't incremental — it's structural. "Netflix used to deliver DVDs in envelopes. When the Internet got fast, they became a movie studio." Fast AI won't just make existing tasks faster. It will enable entirely new business models that don't exist yet.

https://www.youtube.com/watch?v=jeop9wfb9jU


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
