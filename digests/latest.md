*AI Builders Digest — May 6, 2026*

*X / TWITTER*

*Swyx* — AI builder & podcaster (dxtipshq, Cognition, Temporal, AI Dot Engineer, Latent Space)

Swyx shared a reconstructed WSJ chart comparing OpenAI (~$850B valuation, ~$30B ARR) to Anthropic (~$900B valuation, ~$44B ARR) — noting that Anthropic's revenue may be $8–10B lower under OpenAI's accounting methodology. He also promoted a talk version of a recent piece co-created with steveruizok, and highlighted a popular post featuring DevOps pioneer Patrick Debois as a track keynote he gave a "blank check" to based on early support.
• <https://x.com/swyx/status/2051440392722391180|OAI vs. Anthropic valuation comparison>
• <https://x.com/swyx/status/2051329419860758932|Talk version post>
• <https://x.com/swyx/status/2051329252344369626|Patrick Debois keynote highlight>

*Peter Yang* — Product at Roblox, AI tutorial creator for 140K+ readers

Peter Yang laid out a clean three-wave framing for AI's progression: "Coding is the first frontier. Knowledge work is the second one. Personal agents are the third." He also crowdsourced ideas for getting his 8-year-old started building with agents — something shareable with her class, maybe earning her first dollar online.
• <https://x.com/petergyang/status/2051508988936937764|Coding → Knowledge → Personal agents>
• <https://x.com/petergyang/status/2051459299860533483|Getting an 8-year-old to build with agents>

*Amjad Masad* — CEO of Replit

Replit CEO Amjad Masad shared two user success stories: an entrepreneur who used Replit to find investors and land meetings, and a multi-modal learning platform built for deaf students — which he called "great use of AI for education." Both highlight Replit expanding beyond developer tooling into real-world impact.
• <https://x.com/amasad/status/2051511694040744139|Replit helps entrepreneur find investors>
• <https://x.com/amasad/status/2051406536443035922|Multi-modal learning platform for deaf students>

*Guillermo Rauch* — CEO of Vercel

Vercel CEO Guillermo Rauch announced `npx deepsec`, an open-source agent orchestrator for deep security reviews. Built for internal use and tested against major OSS projects, it can find critical vulnerabilities in minutes that would take human teams months. It runs thousands of agents scrutinizing a codebase in parallel via Vercel Sandbox. He's offering to sponsor runs for OSS projects — DMs open.
• <https://x.com/rauchg/status/2051386798899888539|Announcing npx deepsec>

*Aaron Levie* — CEO of Box

Box CEO Aaron Levie argues that enterprise AI agent deployment is in early innings but about to move fast. With both Anthropic and OpenAI launching enterprise agent initiatives, the real work is just starting: upgrading IT systems, giving agents the right context, redesigning workflows, and managing the human-agent relationship. "While AI models have an incredible amount of capability packed into them, there's no shortcut to getting that intelligence applied to a business process in a stable way." He sees this creating major new job and firm opportunities across the market.
• <https://x.com/levie/status/2051344780328858040|Enterprise AI agents: early but getting very big fast>

*Garry Tan* — President & CEO of Y Combinator

YC's Garry Tan is shipping fast on GBrain, his personal AI tool. v0.27 adds support for non-Anthropic and non-OpenAI embeddings and LLMs, with multi-modal embeddings and deep photo OCR on deck. He positions GBrain as uniquely differentiated: "It's not a memory layer OR a code tool OR a search engine. It's all three unified under one graph with one query interface. Nobody else has that." He uses it all day with a 100K markdown file setup.
• <https://x.com/garrytan/status/2051517574589116510|GBrain v0.27 release>
• <https://x.com/garrytan/status/2051525161380364315|What makes GBrain different>

*Nikunj Kothari* — Partner at FPV Ventures

FPV Ventures partner Nikunj Kothari called Gemini Flash "criminal how cheap and how good" — praising its 1M context windows, structured outputs, and new live voice model as his most-used model in production workloads. He also dropped a hot take: startup cohort 2023–2025 focused too heavily on launch videos and distribution at the expense of retention, and seed-to-Series-A conversion rates are now starting to show it. He predicts a wave of acquihires coming.
• <https://x.com/nikunj/status/2051321911741972900|Gemini Flash is criminally cheap and good>
• <https://x.com/nikunj/status/2051349526171287930|Distribution vs. retention: the reckoning>

*Peter Steinberger* — Co-creator of OpenClaw, partnered with OpenAI

Peter Steinberger shipped Crabbox 0.5.0 — remote CI boxes with desktop/browser leases, VNC + authenticated WebVNC, AWS Windows + WSL2, screenshots, and app launch. He's also using ephemeral crabboxes with WebVNC so agents can reproduce issues directly, set up the exact state to test and fix, and post videos on the PR. A meaningful step up for agent-powered QA.
• <https://x.com/steipete/status/2051485798613111116|Crabbox 0.5.0 release>
• <https://x.com/steipete/status/2051557150040711425|Agents reproducing issues in ephemeral crabboxes>

*Aditya Agarwal* — General Partner at South Park Commons

South Park Commons GP Aditya Agarwal drew a clear line between speed and direction: "We have never desired to be an accelerator. Velocity is not interesting without a grounding towards true north."
• <https://x.com/adityaag/status/2051330205902581842|Velocity vs. true north>

*Sam Altman* — CEO of OpenAI

OpenAI CEO Sam Altman expressed genuine excitement about voice models improving, observing that people are already changing how they interface with AI. He also teased that OpenAI will "do something nice" for everyone who applied to the GPT-5.5 party but didn't get a spot.
• <https://x.com/sama/status/2051464865634742334|Excited about voice models>
• <https://x.com/sama/status/2051318922805436896|GPT-5.5 party makeup announcement>

*OFFICIAL BLOGS*

*Anthropic Engineering — Claude Code auto mode: a safer way to skip permissions*
<https://www.anthropic.com/engineering/claude-code-auto-mode>

Claude Code's new _auto mode_ offers a middle ground between manually approving every action and the all-or-nothing `--dangerously-skip-permissions` flag. It uses two defense layers: a server-side prompt-injection probe that scans tool outputs before they reach the agent, and a two-stage transcript classifier (running on Sonnet 4.6) that evaluates each action before it executes. Stage 1 is a fast single-token yes/no filter tuned to block aggressively; only flagged actions escalate to Stage 2 with chain-of-thought reasoning. On real internal traffic (n=10,000), the full pipeline hits just 0.4% false-positive rate while catching real overeager actions at 83% recall. The post is candid about the tradeoff: auto mode is designed to replace `--dangerously-skip-permissions`, not careful human review on high-stakes infrastructure. Notable design choice: the classifier strips assistant text and tool results entirely — so the agent can't rationalize or injection-steer its way past the guardrail.

*PODCASTS*

*Training Data — Waymo's Dmitri Dolgov: 20 Million Rides and the Road to Full Autonomy*
<https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8>

_The Takeaway:_ Building toward full autonomy isn't a sprint — it's a twenty-year mission that only rewards those who internalize the real depth of the problem before the first hype cycle ends.

Waymo co-CEO Dmitri Dolgov has been building self-driving cars since the 2005 DARPA Challenge, joining what became the Google Self-Driving Car Project in 2009. Two decades in, Waymo has surpassed 20 million fully autonomous rides — with 10 million of those happening in the last seven months alone, a pace that let them launch four new cities in a single day.

The most counterintuitive insight from Dolgov: early progress in autonomous driving is deceptively easy, which is exactly what triggers hype cycles and mass investment. But that early ease masks a very hard long tail. "The problem has always had this property that it's very easy to get started, but it's very difficult to take it all the way to a real product, full autonomy, and superhuman performance."

On the tech side, Waymo's approach isn't vanilla end-to-end AI. Their Waymo Foundation Model runs a driver + simulator + critic architecture — a multimodal world-action-language model — and deliberately augments learned representations with structured intermediate outputs. This enables closed-loop evaluation, richer reinforcement learning rewards, and run-time validation that a basic end-to-end system can't provide at production scale.

The safety numbers are striking: across 170 million fully autonomous miles, the Waymo driver is more than 13x safer than a human in serious-injury-causing collisions — translating to preventing a serious injury every eight days at current scale. One emergent capability that surprised even Dolgov: the LiDAR detecting footsteps beneath a bus, letting the system predict and react to a hidden pedestrian before they were visible to any sensor.

Waymo is now operating in 11 cities, with London and Tokyo announced for later this year. The sixth-generation hardware platform is already running fully autonomous rides for employees, with a cabin Dolgov describes as feeling like "a living room."

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
