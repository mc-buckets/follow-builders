AI Builders Digest — August 22, 2026

*X / TWITTER*

*Swyx (latentspacepod, smol.ai)*
Two notable shares. Swyx promoted the latest Latent Space podcast with Eisok Kant — who NVIDIA just paid $6B for — on why his company is producing models that are "actually, not exaggeration" beating frontier benchmarks. He also highlighted AI Dot Engineer speaker Matt Pocock's new /wayfinder skill, designed for navigating early-stage research when you don't yet know what you don't know, pairing it with a course launch covered by Richard MacManus.

https://x.com/swyx/status/2090577677916807429
https://x.com/swyx/status/2090550020496040266

*Boris Cherny (Claude Code, Anthropic)*
Announced that Fable-class enterprise safeguards are coming this fall — letting enterprises run frontier models on their own infrastructure with full data control. Anthropic retains none of customer data under this model. The team has been co-developing it with ~100 companies. "Mythos-class models require additional safety measures and enterprises need to meet their own privacy and compliance rules."

https://x.com/bcherny/status/2090537902912815536

*Thibault Sottiaux (Codex & ChatGPT, OpenAI)*
Three updates. First, he clarified that Codex usage limits haven't been secretly changed — users seeing restrictions were mostly running sub2api (converting subscriptions into API traffic to re-serve across many users), which triggers fraud detection. Honest subscribers using Sign in With ChatGPT are unaffected. Second, GPT-Image-2 now supports transparent image generation in ChatGPT and via API. Third, ChatGPT Sites is live — create a shared site and build something collaboratively with others in real time.

https://x.com/thsottiaux/status/2090675027670978569
https://x.com/thsottiaux/status/2090631723302469995
https://x.com/thsottiaux/status/2090518287532916854

*Peter Yang (AI tutorials, YouTube)*
Hit 100K YouTube subscribers and teased upcoming interviews covering AI evals (with Hamel Husain and Shreya Shankar), vibe-coded businesses that became real (Replit Head of Product Engineering), ChatGPT Finance, and SpaceXAI's Grok Bot team. Also floated a simple but provocative agentic design: a "manager agent" that negs a worker agent — prompts like "Are you sure this is the best you can do?" or "I think you can do better, try again" — arguing this alone could meaningfully improve output quality.

https://x.com/petergyang/status/2090589731927282021
https://x.com/petergyang/status/2090564541499498919

*Madhu Guru (Sr Director, AI at Meta)*
Published part 4 of his "how to build great evals" series, arguing enterprises fail at AI because they lack a _laddered_ eval strategy. The four tiers he outlines: hill-climb evals (push the quality frontier, refresh continuously), regression evals (did we break what works today?), smoke test evals (safety basics that absolutely cannot go wrong), and launch evals (near-real traffic, most realistic). He notes that smoke tests aren't necessarily the hardest questions — just the ones that matter most to get right.

https://x.com/realmadhuguru/status/2090595384905113939

*Thariq (Claude Code, Anthropic)*
Echoed the Fable enterprise announcement (same news as Boris Cherny above, from the same team): enterprises get control over where data lives and who has access to it. Broader rollout expected this fall after ~100 pilot companies.

https://x.com/trq212/status/2090569474139439335

*Amjad Masad (CEO, Replit)*
Announced a long-awaited Replit + OpenAI partnership, sharing a story about PG asking Sam Altman to recruit Replit before they were even in YC. Also highlighted that Replit's new Free Mode is notably fast — "making coding interactive again" — and that you can build a substantial amount with it.

https://x.com/amasad/status/2090514571513708874
https://x.com/amasad/status/2090484698413740186

*Guillermo Rauch (CEO, Vercel)*
Teased a 0.0.5 release that's small enough to fit on two floppy disks (xz-compressed), shipping tomorrow with the most-requested feature. Also declared that Vercel is "building AWS for agents." Separately, congratulated Bun's Jarred Sumner on shipping — calling Bun's "simple, fast & open" ethos a perfect match for Vercel's worldview.

https://x.com/rauchg/status/2090600467592266240
https://x.com/rauchg/status/2090520415336845595
https://x.com/rauchg/status/2090470175674179695

*Aaron Levie (CEO, Box)*
Wrote a detailed take on post-training for applied AI: once you have deep enough vertical expertise and enough task volume, purpose-building domain-specific models makes real sense. He quoted the key insight from the post he shared: "In post-training, we incentivized efficient tool use and reasoning through reward shaping, preferring trajectories that would reduce tokens consumed at inference-time given equivalent performance. This allowed us to co-optimize for both cost and quality." He noted this won't make sense in every domain, but for companies with genuine vertical depth, it's a compelling path to winning.

https://x.com/levie/status/2090664811185205722

*Garry Tan (President & CEO, Y Combinator)*
Signaled strong sector conviction with two posts: "YC is the YC for AI Researchers" and "YC is the YC for consumer hardware." Also flagged what he called an "interesting violation of 'you should dogfood your own product'" — context unclear without the quoted tweet, but provocative enough to note.

https://x.com/garrytan/status/2090471408996659339
https://x.com/garrytan/status/2090469087722041567
https://x.com/garrytan/status/2090470082053050655

*Zara Zhang (Builder)*
Shared a reframe from a Claude conversation that stuck with her: "Motivation follows action more than it precedes it." Simple, but she says it completely changed how she thinks about getting unstuck.

https://x.com/zarazhangrui/status/2090399357145317837

*Nikunj Kothari (Partner, FPV Ventures)*
Wrote a detailed thread on why ambition matters so much in VC right now. The core math: with Anthropic becoming the fastest company to reach $1T valuation, Cursor going from $0 to $60B in four years, and fund sizes exploding accordingly, every deal needs to be underwritten to a trillion-dollar outcome. At that scale, the error of omission — missing the next Anthropic — is far worse than the error of admission. Price barely matters when you're swinging for that outcome. "The error of omission is way, way worse than the error of admission. And then power law kind of takes care of itself."

https://x.com/nikunj/status/2090585553947517298

*Aditya Agarwal (General Partner, South Park Commons)*
Shared a new Minus One episode with Snowflake CEO Sridhar Ramaswamy — the person who scaled Google Ads from $1B to $100B — on navigating Snowflake through the AI shift. Aditya's framing: the best founders are reductionists with the clarity to cut through fog of war. Topics covered include lessons from Google's founders, what went wrong at Neeva, and Snowflake's enduring value in the AI era.

https://x.com/adityaag/status/2090478527313252494
https://x.com/adityaag/status/2090501112927223889


*OFFICIAL BLOGS*

*Anthropic Engineering — <https://www.anthropic.com/engineering/april-23-postmortem|An update on recent Claude Code quality reports>*
Anthropic disclosed and post-mortemed three separate bugs that degraded Claude Code quality over the past month. (1) In March, default reasoning effort was changed from high to medium to reduce latency — users said they'd prefer higher intelligence and opt into lower effort, so it was reverted April 7; all users now default to xhigh effort for Opus 4.7 and high for other models. (2) A caching optimization had a bug that continuously dropped prior reasoning from sessions, making Claude seem forgetful and draining usage limits faster than expected — fixed April 10. (3) A system prompt instruction capping response length ("≤25 words between tool calls") hurt coding quality — reverted April 20. All issues are resolved as of April 20 (v2.1.116). Anthropic is resetting usage limits for all subscribers and adding tighter controls on system prompt changes, including per-model evals for every prompt change.

*Anthropic Engineering — <https://www.anthropic.com/engineering/managed-agents|Scaling Managed Agents: Decoupling the brain from the hands>*
Deep technical post on the Managed Agents architecture. The core design move: decouple the "brain" (Claude + harness) from the "hands" (sandbox) and session log. Each component becomes cattle instead of pets — if a container dies, the harness catches it as a tool error; if the harness fails, a new one resumes from the durable session log. Security benefit: agent-generated code never runs in the same environment as credentials. Performance result: p50 time-to-first-token dropped ~60%, p95 dropped over 90%. The principle echoes how operating systems virtualized hardware — stable interfaces outlasting the implementations underneath.

*Claude Blog — <https://claude.com/blog/claude-managed-agents-updates|New in Claude Managed Agents: self-hosted sandboxes and MCP tunnels>*
Two new Managed Agents capabilities are now available. Self-hosted sandboxes let enterprises run agent tool execution on infrastructure they control — or via Cloudflare, Daytona, Modal, or Vercel — keeping sensitive code, files, and data within their security perimeter. The agent orchestration stays on Anthropic's infrastructure while tool execution moves inside the enterprise boundary. MCP tunnels connect agents to private-network MCP servers via a lightweight outbound-only gateway, no inbound firewall rules or public endpoints required. Self-hosted sandboxes are in public beta; MCP tunnels in research preview (request access on the Claude Platform).


*PODCASTS*

*No Priors — From Restoring Sight to Reimagining the Brain, with Max Hodak*

_The Takeaway:_ Treating the brain as a computer — not a biological mystery to solve with drugs — produces faster, more reliable results, and Max Hodak's Science is already selling the first commercially approved device to prove it.

Max Hodak, founder and CEO of Science (formerly a co-founder of Neuralink), just received CE marking in Europe for Prima — a retinal prosthesis that restores functional vision to blind patients. The device implants a chip under the retina; the patient wears laser-projecting glasses that stimulate the chip directly, bypassing dead photoreceptors. It's the first device to generate a coherent visual image — not just flashes of light — in the mind's eye of a blind patient. Commercial sales begin in the coming weeks.

The contrarian core: Hodak thinks the AI-to-brain BCI hype cycle (thought-controlled cursors, silent speech) is misdirected. Writing and speaking, he argues, are already as fast as thought — the brain has a deeply evolved ~10-bit-per-second cognitive bottleneck, and BCI won't break that. The more interesting frontier is generating sensory experience: vision, hearing, balance. "If you can get the visual signal, auditory signal, balance, motor, in and out of the brain, that is an end in itself. That is the central object."

On AI and neuroscience: Hodak is a proponent of the platonic representation hypothesis — that large AI models and biological brains develop similar internal geometry for representing concepts. Science uses AI model internals to understand neural representations in practice, and for Hodak, those empirical alignments were an early signal that modern AI was "on the right track" rather than heading toward a wall.

On medicine broadly: The brain is the only organ you can't even in principle transplant, Hodak argues — everything else is support infrastructure for keeping the brain running. His long-term goal: make humans dramatically less fragile by improving the brain's I/O rather than fighting the underlying biology. "I'm going to be ultimately fairly disappointed if I'm murdered by my pancreas."

https://www.youtube.com/watch?v=7HXqMepjvy8

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
