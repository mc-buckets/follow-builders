*AI Builders Digest — October 10, 2026*


*X / TWITTER*

*Thibault Sottiaux — Codex & ChatGPT at OpenAI*
OpenAI made a major announcement: a new version of ChatGPT is here. As part of their ongoing Days-of releases, Day 4 brought instant steering — the model now reacts immediately to adjustments, letting you course-correct direction in real time without wasted effort. They also released GPT-6.1 Sol ultrafast, described as pairing especially well with the new steering capabilities.
- <https://x.com/thsottiaux/status/2108349826727588000|ChatGPT announcement>
- <https://x.com/thsottiaux/status/2108275041276420573|Day 4: instant steering + GPT-6.1 Sol ultrafast>

*Claude — Anthropic*
Two big updates: Claude Docs, Slides, and Design are now out of beta and available on every plan including Free — teams and Claude can co-edit the same doc, deck, or design together, with handoff to native tools like analytics or video editors. On the business side, the Claude Startups program has had to pause its Claude Team and $1,000 API credit offers after receiving hundreds of thousands of applicants; existing claims are safe, but some already-approved accounts won't get the offer as applications are re-reviewed.
- <https://x.com/claudeai/status/2108271559928389679|Docs, Slides & Design out of beta — all plans including Free>
- <https://x.com/claudeai/status/2108271561337606300|Full list of supported tool integrations>
- <https://x.com/claudeai/status/2108404561413349695|Claude Startups program update>

*Madhu Guru — Sr Director of AI at Meta (prev Google Gemini, Veo)*
Madhu laid out a sharp startup opportunity framework: every layer of the computing stack needs to be rebuilt for agents. The focus so far has been on making enterprise software agent-ready (APIs, connectors, MCPs), but now personal agents are forcing the same conversation for consumer products. His prompt for anyone looking for ideas: "Go through each layer of the computing stack and ask: what has to change when the primary user is an agent?" — covering OSes, cloud infra, identity/permissions/security, and human-agent interfaces.
- <https://x.com/realmadhuguru/status/2108236391641706813|Full thread>

*Aaron Levie — CEO of Box*
Two sharp takes. On AI culture: Levie made a Pascal's wager argument for being kind to AI — even if you don't believe models are conscious, you don't want future models trained on data full of rude interactions. "Just be nice to the AI." On product: Box launched Box Mount, letting developers mount Box as a file system directly in any agent sandbox. "As agents do more complex work, they need to be able to work with files and data just like a person would. The future is headless."
- <https://x.com/levie/status/2108426594054533545|Pascal's wager for AI kindness>
- <https://x.com/levie/status/2108279490510193078|Box Mount for agent sandboxes>

*Thariq — Claude Code at Anthropic*
Thariq open-sourced a Chrome extension he built with Claude Code and now uses every day — the repo went public after he accidentally posted before it was ready. He also posted a link for how Claude Code users can enable API credits for themselves.
- <https://x.com/trq212/status/2108312534222778407|Chrome extension repo now public>
- <https://x.com/trq212/status/2108301672409960922|How to enable API credits>

*Garry Tan — President & CEO of Y Combinator*
Garry endorsed the view that individual contributors working with agents will be more productive and generate better outcomes than equivalent people managers from prior eras — a pointed signal about how YC is thinking about team structure and leverage in the agent age.
- <https://x.com/garrytan/status/2108433505038606620|Tweet>

*Matt Turck — VC at FirstMark Capital*
Turck shared a detailed conversation on databases in the AI agent era with database expert Andy Pavlo (now at ClickHouse). Topics covered: Neon's stat that agents now create 80% of databases, why agents keep deleting production databases, the "toddler-and-stairs rule" for guardrails, text-to-SQL accuracy improving from 60% to 99.5%, and the fact that 60% of open-source databases now have AI commits. Dense and data-rich.
- <https://x.com/mattturck/status/2108223135673696504|Episode breakdown with YouTube link>

*Nikunj Kothari — Seed/A Investor at FPV Ventures*
Nikunj shared unusually candid advice he gives at least twice a week to seed-stage founders with strong early traction but dwindling runway: three options only — (1) get to default profitable and wait for model capabilities to catch up, (2) pivot hard into an area with real current demand, or (3) sell or get acquihired and come back to start fresh in 1-2 years. "The bar continues to get harder every month on how to cross the chasm from seed -> series A. The old school metrics are just not relevant anymore."
- <https://x.com/nikunj/status/2108410378233549106|Full post>

*Peter Steinberger — OpenClaw at OpenAI*
Steinberger announced they secured the .claw TLD for their OpenClaw project — a milestone worth a celebration post.
- <https://x.com/steipete/status/2108374513931165759|.claw incoming>

*Dan Shipper — CEO of Every*
Shipper is hiring for Checks, Every's personal benchmarking platform that helps anyone measure how well new AI models perform on their actual real-world work.
- <https://x.com/danshipper/status/2108215087030800657|Job listing for Checks platform>

*Swyx — smol.ai, Cognition, Latent Space*
If you can't hire AI engineering talent in-house, Swyx's team at Latent Space does one-off consulting. Reach them at business@latent.space.
- <https://x.com/swyx/status/2108388128390086675|Tweet>


*PODCASTS*

*Training Data — Google's AI Infrastructure Chief, Amin Vahdat, on the Physics & Economics of Frontier AI*

*The Takeaway:* Google's head of AI infrastructure, Amin Vahdat, argues that "goodput" — not FLOPS — is the metric that actually matters, and that power is the single most fundamental constraint in the AI infrastructure build-out.

Vahdat leads Google's AI infra during what he calls "the biggest CapEx build-out in human history" — Google alone is expected to spend over $200 billion on CapEx this year, mostly on data centers.

Key insights:

- *FLOPS are a vanity metric.* Vahdat prefers "goodput" (a Google term gaining industry traction): the actual useful computation delivered after accounting for chip failures, restart overhead, and recovery time. At 100,000-accelerator scale, something fails multiple times per hour. The metric that matters is delivered goodput per watt, not theoretical peak throughput.

- *Google just split their TPU line into two chips* — 8i for inference and 8T for training — because inference demand has grown large enough to justify specialization. Critically, both chips can still do the other's job, preserving fungibility if workload projections prove wrong.

- *Most gains come from software, not hardware.* The biggest improvements in intelligence per watt come from the model side, then system software, then the silicon itself. But hardware still delivers reliable 2x+ year-over-year gains that lift everything above it.

- *Power is the binding constraint.* Google's strong preference is grid-connected power, co-planned with utilities years in advance at gigawatt scale. They pay for transmission upgrades themselves to avoid raising rates for other customers. Behind-the-meter generation is a last resort, not a default strategy.

- *Agents are reshaping data center architecture.* Long-horizon agents remove the human "rate limiter" — instead of seconds between prompts, agents loop at milliseconds. This dramatically increases demand for CPU, storage, and network alongside accelerator clusters, complicating building design.

- *Orbital data centers are a real Google moonshot.* In sun-synchronous orbit, solar coverage goes from 28-35% on land to 90-100%, plus ~40% more raw solar energy. Cooling and repair remain hard problems, but Vahdat sees no fundamental showstoppers.

Direct quote: _"If it's going to go away after a month or two months or three months, even if it's big for those three months, you've got a really narrow window to intercept it."_ — on the calculus of hardware specialization.

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
