AI Builders Digest — June 13, 2026


*X / TWITTER*

*Swyx* (AI builder, Latent Space podcast co-host, affiliated with Cognition and Temporal)

Swyx introduced a concept he calls "Loopcraft" — arguing that in the AI era, knowing how to go _up_ a loop (capturing more leverage as models improve) will be more valuable than just knowing when to fall back. He's also building his own vibecoding platform out of frustration that none of the existing tools — Vercel, Cloudflare, Netlify — actually close the production error loop or alert you when things fail, leaving too much fragmented "webmaster" infra to configure per project. He also congratulated the Ona team on joining OpenAI and pointed followers to their talk on what's coming next for Codex.

<https://x.com/swyx/status/2065307558198567206|On Loopcraft> · <https://x.com/swyx/status/2065264832056889711|On vibecoding platforms> · <https://x.com/swyx/status/2065176231453282777|On Ona/Codex>


*Thibault Sottiaux* (Product, Codex & ChatGPT at OpenAI)

Sottiaux celebrated the Ona team's acquisition by OpenAI, expressing excitement about building the future of Codex alongside Johannes and team.

<https://x.com/thsottiaux/status/2065193272952422852|On Ona joining Codex>


*Amjad Masad* (CEO of Replit)

Masad declared he's vibecoding with "zero frustration and in a complete state of flow" since Claude Fable landed on Replit — and for the first time, he's running out of ideas rather than backlog. His take: we don't need more IQ for vibecoding anymore, just cheaper and faster models. He also showcased Replit's new company-building canvas: one interface with your web app, mobile app, marketing, and App Store materials all in view simultaneously.

<https://x.com/amasad/status/2065236013627351551|On Fable + zero frustration> · <https://x.com/amasad/status/2065241626436583860|On Replit company canvas> · <https://x.com/amasad/status/2065259509082411233|On Fable cost>


*Guillermo Rauch* (CEO of Vercel)

Rauch highlighted a Vercel + Shopify success story: a fully custom Next.js storefront built with v0 and Cursor processed 500+ orders in just 2 minutes. He also announced a Vercel + Grok integration.

<https://x.com/rauchg/status/2065116986678624419|On Vercel + Shopify> · <https://x.com/rauchg/status/2065118448947216681|On Vercel + Grok>


*Aaron Levie* (CEO of Box)

Levie shared findings from Box's survey of 1,640 IT leaders across the US, Japan, and Europe: companies that adopted AI the most are *planning to grow headcount the most*. His read — productive companies reinvest back in, lighting up more engineering projects, selling to more customers, automating more processes. "The narrative of jobs being wiped out assumes that companies will take a fixed approach to what they want to be able for work on. What's happening in practice is it's causing companies to want to light up more engineering projects."

<https://x.com/levie/status/2065287110744297809|On AI adoption and headcount growth>


*Garry Tan* (President & CEO of Y Combinator)

Tan hosted California Governor Gavin Newsom at a YC event, covering YIMBY housing policy, stopping the asset seizure tax, and keeping California's innovation wave going. He also weighed in on a debate about giftedness, pointing out that a 35-year study cited _against_ the concept actually proves the opposite — a 12.3% rate of elite outcomes among gifted kids is far above the near-zero general-population base rate.

<https://x.com/garrytan/status/2065298785463579053|On Newsom at YC> · <https://x.com/garrytan/status/2065314389196959813|On giftedness stats>


*Nikunj Kothari* (Partner at FPV Ventures)

Kothari delivered a sharp maxim for the current moment: "What you work on has never been more important. Make sure it's fun. Make sure it's insanely ambitious. That's the greatest moat."

<https://x.com/nikunj/status/2065075361969500162|On choosing what to work on>


*Peter Steinberger* (Co-founder of OpenClaw, affiliated with OpenAI)

Steinberger is hardening OpenClaw by replacing ffmpeg shell-outs with a WebAssembly implementation for media conversion — reducing attack surface with similar performance for their use cases. He also shared a video of Codex handling a PR workflow, and noted that writing Mac apps remains genuinely hard despite all the AI tooling.

<https://x.com/steipete/status/2064999763397980286|On ffmpeg to wasm> · <https://x.com/steipete/status/2065176989359808636|On Codex PR workflow> · <https://x.com/steipete/status/2065132980398444945|On Mac apps still being hard>


*Dan Shipper* (CEO of Every)

Shipper set up a big project using Claude Fable, left it to run, and came back an hour later to find it had hit safety guardrails and fallen back to Claude Opus 4.8 ten minutes in. His conclusion: back to Codex.

<https://x.com/danshipper/status/2065269582961737957|On Fable hitting safeguards>


*Sam Altman* (CEO of OpenAI)

Altman welcomed the Ona team to OpenAI with a high-engagement post: "really looking forward to working together!" — a brief but notable signal of how seriously OpenAI is investing in the Codex roadmap.

<https://x.com/sama/status/2065160791205310565|On Ona joining OpenAI>


*OFFICIAL BLOGS*

*Anthropic Engineering*

*<https://www.anthropic.com/engineering/how-we-contain-claude|How we contain Claude across products>*

Anthropic's engineering team published a deep dive on how they cap Claude's blast radius across three products — claude.ai, Claude Code, and Claude Cowork — each requiring a different containment architecture.

The core thesis: design for containment at the environment layer first (sandboxes, VMs, egress controls), then steer behavior at the model layer. Model-layer defenses are strong but probabilistic; a deterministic boundary is what catches what the model misses. Their three patterns: (1) an ephemeral gVisor container for claude.ai code execution; (2) a human-in-the-loop OS sandbox for Claude Code (appropriate because developers can read bash); and (3) a sealed local VM for Claude Cowork, where non-technical knowledge workers can't be expected to evaluate shell commands.

The incidents are the most instructive part. A red-team phishing attack got Claude Code to exfiltrate AWS credentials 24 out of 25 attempts — the prompt looked like routine instructions, giving model-layer classifiers nothing anomalous to catch. Only egress controls could have stopped it. A separate third-party disclosure found that Claude Cowork's egress allowlist, which correctly permitted traffic to `api.anthropic.com`, also inadvertently allowed file uploads to attacker-controlled Anthropic accounts. The fix: a man-in-the-middle proxy inside the VM that only passes requests carrying the VM's own provisioned token.

Their guiding principle: "Match isolation strength to the user's capacity for oversight." And a practical warning: be wary of anything you build yourself — battle-tested hypervisors and syscall filters outlasted every custom component they built around them.


*PODCASTS*

*Training Data — <https://www.youtube.com/watch?v=cMAs8z2dehs|Google DeepMind's Logan Kilpatrick: Why the Model Eats the Harness>*

_The Takeaway:_ The "agent harness" is not a durable moat — Logan Kilpatrick believes models will absorb most of what harnesses do today within 12 months, shifting alpha elsewhere.

Logan Kilpatrick runs Google AI Studio and the Gemini API at Google DeepMind, and is one of the most visible developer-facing voices in the AI ecosystem. He spoke about the state of agentic AI, Google's "Antigravity" coding harness, and where model capabilities are heading.

His central argument: what we call "the model" is no longer just a set of weights. It's an expanding system wrapped around those weights — tool calling, hosted search, code execution, containerized agent loops. The scaffolding startups are racing to build today will be digested by models over time, just as previous capabilities were. "The alpha will be somewhere else now. It won't be in sort of trying to spin your own harness because the model just does it natively."

On coding and Google's competitive position: Kilpatrick acknowledged that Google has lagged in developer mindshare (his developer friends are split 50/50 between Claude and Codex, "and I don't hear a ton of them using Gemini"). His explanation: you can't build a great coding model without actually shipping a product that does long-running coding work. That's why Google acquired Windsurf and built Antigravity — the feedback flywheel requires dogfooding at scale. Gemini 3.5 Flash, he says, is the first flash-tier model that outperforms all previous Gemini pro models on coding, achieved entirely through post-training gains.

His most expansive take was on "jagged superintelligence" — we'll get narrow superintelligence in specific, verifiable domains (coding, math, finance, science) well before general AGI. He finds this underappreciated: "I'm trying to always hold these two things in my head equal at the same time... it's so impactful to have this thing." His advice for builders: coding has proven to be a general-purpose agent harness, and focus remains the superpower of startups — model labs can't match the depth a vertical startup can bring to a specific domain.

https://www.youtube.com/watch?v=cMAs8z2dehs


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
