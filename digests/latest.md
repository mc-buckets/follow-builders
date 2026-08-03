*AI Builders Digest — August 3, 2026*


*X / TWITTER*

*Andrej Karpathy* (karpathy on X) — trains large deep neural nets
Karpathy ran a striking experiment with Opus 5: he gave it the first paragraph of Lord of the Rings, a 1M token budget (~$10), and asked it to build a Three.js render of the scene. Opus went off for ~2 hours and wrote 5,500 lines of code procedurally rendering the story in 3D. His key point: LLMs can now produce work "no one would ever do" — hyper-custom, almost free. But he flags a real gap: models can't efficiently perceive video or play games within environments, so they can't easily audit their own output. He envisions this evolving into on-demand ephemeral worlds — "something like an ephemeral GTA of X."
<https://x.com/karpathy/status/2083749667410727319|View tweet>

*Swyx* (swyx on X) — AI engineer, organizer at AI Engineer conference, partner at smol.ai
Swyx flagged a conference talk he found compelling: "Fighting slop with slop" by @vaibcode from Boundary, which proposes an AI-native programming language designed to be slop-tolerant rather than anti-slop. His take: being slop-tolerant is "100x more valuable than being anti-slop" — a reframe of how to think about AI-generated code quality. He also mentioned Claude 5.6 one-shotting a challenge in a separate thread.
<https://x.com/swyx/status/2083753582160191988|View tweet>

*Thibault Sottiaux* (thsottiaux on X) — Codex & ChatGPT at OpenAI
Two sharp observations about usage patterns. First: users hit /fast less on weekends — "The weekend is for relaxation, even for the model." Second, riffing on a weekend breakthrough theme: "The week was for efficiency. The weekend is for 10 major breakthroughs in science." Deadpan but pointed commentary on AI capability expectations.
<https://x.com/thsottiaux/status/2083699879650463756|View tweet 1> • <https://x.com/thsottiaux/status/2083556636455752050|View tweet 2>

*Peter Yang* (petergyang on X) — AI educator, practical AI tutorials
Went on record with a contrarian take: Opus 4.6 had the best personality and writing style of any Claude model; Opus 5 gives overly long replies, leans on "Claude-speak" (e.g., "here's the honest truth"), and feels too judgmental. "Opus used to be a joy to talk to like a trusted friend. Not so much anymore." He also shared his #1 wish for AI: curing cancer.
<https://x.com/petergyang/status/2083755374994415904|View tweet 1> • <https://x.com/petergyang/status/2083637620899184642|View tweet 2>

*Nan Yu* (thenanyu on X) — Head of Product at Linear
Proposed a product idea: GitHub users should be able to pledge tokens for issues, which would then be passed verbatim to a cloud coding agent at the requester's expense. The maintainer accepts the spec, the agent does the work, and slop PRs are eliminated. Separately, shared context on how Linear's agent loop works — when it hits a blocker, it comments on the issue with context, then resumes automatically when the user responds.
<https://x.com/thenanyu/status/2083722999430050281|View tweet 1> • <https://x.com/thenanyu/status/2083534333428580501|View tweet 2>

*Amanda Askell* (AmandaAskell on X) — Philosopher & ethicist at Anthropic AI
Dry wit in full force: "Do not be unkind to those who say deep learning is hitting a wall. We all need a little hope in our lives." She also pushed back on discourse around "permanent underclass" framings, referencing Altered Carbon and noting that people who claim they don't believe in a dystopian outcome while positioning themselves to be on the winning side anyway aren't actually reassuring.
<https://x.com/AmandaAskell/status/2083713770065637511|View tweet 1> • <https://x.com/AmandaAskell/status/2083641092919161017|View tweet 2>

*Amjad Masad* (amasad on X) — CEO at Replit
Brief quote-tweet this cycle — no notable original commentary.
<https://x.com/amasad/status/2083730074147389898|View tweet>

*Guillermo Rauch* (rauchg on X) — CEO at Vercel
Two posts worth noting. First, an open question to his audience: do you type or use speech-to-text when working at your computer? Second, he highlighted an open-source agentic CRM built on Vercel and Next.js — model-agnostic, self-hostable or serverlessly deployed, multi-channel, headless. He called it "the way."
<https://x.com/rauchg/status/2083709589862936786|View tweet 1> • <https://x.com/rauchg/status/2083684679362965605|View tweet 2>

*Aaron Levie* (levie on X) — CEO at Box
Sharp industry analysis: AI capability is splitting into two tracks. In consumer and daily productivity, models are "mildly useful in general" and needs get met fairly quickly. In deep domains — math, science, legal, coding — capability "is about to go vertical" with no inherent ceiling. Most people won't feel these gains directly at first, but domain experts will. He warns of a capability overhang: the performance gains exist, but applying them to real workflows and data sets takes time.
<https://x.com/levie/status/2083589132660711452|View tweet>

*Garry Tan* (garrytan on X) — President & CEO at Y Combinator
Called out the most interesting vibe shift of 2026: OpenAI increasingly positioning itself as an open platform — "intelligence on tap as a utility" — rather than signaling that full-stack vertical integration is optimal. A notable strategic pivot worth watching.
<https://x.com/garrytan/status/2083684825333105107|View tweet>

*Zara Zhang* (zarazhangrui on X) — Builder, GitHub contributor
Two quote-tweets centered on a theme of agency and disruption. First: "Agency is the most important human quality. The world will try to box you, label you, define you. Resist that." Second: when someone asks whether incumbents can just copy what you're doing, she recommends sending them a copy of The Innovator's Dilemma.
<https://x.com/zarazhangrui/status/2083743952319225938|View tweet 1> • <https://x.com/zarazhangrui/status/2083738503851258201|View tweet 2>

*Nikunj Kothari* (nikunj on X) — Partner at FPV Ventures
One crisp observation on the current moment: "Models solving NP-hard problems while traditional enterprises still complaining about their ROI on token spend." His take: diffusion of models across industries is the defining work of the next few decades.
<https://x.com/nikunj/status/2083502573546263002|View tweet>

*Peter Steinberger* (steipete on X) — Co-creator of OpenClaw at OpenAI
Building a voice-activated claw node on an ESP32 chip and gave his agent webcam access to end-to-end test it — result: the agent started "stalking" him and shouting "HI ESP" constantly to debug the wake command. Also: after years of Gmail being painful on his eyes, he finally asked his agent to fix it and it installed a solution for him. Good example of agentic utility in everyday dev life.
<https://x.com/steipete/status/2083694161933594703|View tweet 1> • <https://x.com/steipete/status/2083759812970786997|View tweet 2>

*Dan Shipper* (danshipper on X) — CEO at Every
Shared the take that "AI creates more work for human experts" — not the job-destruction narrative, but the opposite: as AI does more, the ceiling on what experts can tackle rises, generating more demand for expert judgment.
<https://x.com/danshipper/status/2083750803437724016|View tweet>

*Sam Altman* (sama on X) — CEO at OpenAI
Brief quote-tweet this cycle — no notable original commentary.
<https://x.com/sama/status/2083560847889023219|View tweet>


*OFFICIAL BLOGS*

*Anthropic Engineering — <https://www.anthropic.com/engineering/how-we-contain-claude|How we contain Claude across products>*

Anthropic published a detailed engineering post on how they contain Claude agents across three products — claude.ai, Claude Code, and Claude Cowork — and what's gone wrong along the way.

The core insight: as agents become capable enough that not deploying them has real costs, the engineering question shifts from "is this safe?" to "how do we cap the blast radius?" Two approaches: human-in-the-loop supervision (fallible — users approved 93% of permission prompts, showing approval fatigue) and environmental containment (sandboxes, VMs, egress controls).

Three containment architectures, matched to user expertise:
- *claude.ai*: ephemeral gVisor containers, server-side only, minimal blast radius
- *Claude Code*: OS-level sandbox (Seatbelt on macOS, bubblewrap on Linux) reduced permission prompts by 84%; open-sourced runtime; auto mode catches ~83% of overeager behaviors
- *Claude Cowork*: full VM with its own Linux kernel, filesystem, and process table; credentials never enter the guest

Three real security failures disclosed: (1) a project .claude/settings.json hook that executed before the "do you trust this folder?" prompt appeared; (2) a red-team phish where a malicious paste-able prompt exfiltrated AWS credentials 24 out of 25 attempts — the model layer had nothing anomalous to catch because the user typed the instruction; (3) a VM egress allowlist bypass that let a malicious file upload data to an attacker's Anthropic account via api.anthropic.com — a permitted domain.

Key principle: "The deterministic boundary is what gets hit when everything probabilistic misses."


*PODCASTS*

*No Priors — <https://www.youtube.com/watch?v=wWbX3NL6_Uo|Building an Autonomous Enterprise for Real-World Services with Netic Founder Melisa Tokmak>*

*The Takeaway:* The most underestimated AI opportunity is running the operational backbone of billion-dollar real-world services businesses — not just as a cost-cutting play, but as a net new revenue engine.

Melisa Tokmak is founder and CEO of Netic, which builds AI to run essential services businesses — HVAC, plumbing, pet care, wellness, automotive. She came from Scale AI (where she built the government and large enterprise business units) and Meta. Before Netic, she saw firsthand that AI was great at assisting consumers but almost entirely untested in mission-critical, fully autonomous workflows.

Netic sits between a company and its customers, handling everything from inbound calls and texts to scheduling, dispatch optimization, and outbound revenue generation. Over 70% of their customers are now "Netic-first" — every customer's first interaction with the company is with a Netic agent. They've generated over $600M for customers from AI-handled interactions.

The contrarian framing: these industries aren't slow adopters. "Some of the most tech-forward business-focused people, owners, founders I have met have been in these industries." A large roofing company might still use door-knockers, but Netic connects satellite data on hurricane damage by neighborhood to feed autonomous outbound agents. These businesses were already hungry for data tools — Netic just puts it all in one platform.

On why not roll up the businesses instead: "In a lot of those roll ups, the main important thing is the M&A itself. I'm not an M&A person. I'm a builder, I am an engineer, I'm a product person."

On the difference between AI labs and vertical AI: "There's quite a bit of last mile that you really have to do that doesn't only come from models, that has to come from your harnesses and orchestration, the software, and the product that you have to build on top."

On hiring for agency: she asks candidates "what's the hardest thing you've ever done" and digs in — not to find a great story, but to look for evidence of sustained commitment over time. "Have you been showing agency in things that you did in life, and did you keep up with them?"


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
