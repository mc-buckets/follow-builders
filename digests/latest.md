*AI Builders Digest — May 12, 2026*


*X / TWITTER*

*Swyx (swyx on X)* | AI.Engineer, latentspace

Swyx announced a major coup for AI.Engineer Singapore: the country's Minister of Foreign Affairs will keynote the event, alongside NanoClaw creator Gavriel Cohen — and the UK's Chief AI Officer is also participating. Swyx sees this as a meaningful signal: "governments waking up to AI and joining aiDotEngineer." He also flagged Codex's headless/background mode adoption rate as a useful proxy for agent adoption and alignment trends, asking OpenAI for the data.

- Singapore government keynote announcement: https://x.com/swyx/status/2053370687931498603
- Codex mode adoption as agent proxy: https://x.com/swyx/status/2053364156510982164


*OpenAI VP of Science Kevin Weil (kevinweil on X)*

Weil called a linked piece "a matter of extreme importance (and some of the best writing ever)" — a strong endorsement without further context.

https://x.com/kevinweil/status/2053225351946682733


*Peter Yang (petergyang on X)* | Product at Roblox, newsletter author for 140K+ readers

Yang described a "slop compounding" trap worth bookmarking: you accept AI-generated markdown files with ~5% slop because editing manually feels tedious. The model then uses those files as reference when generating new ones. The error rate compounds — "before you know it, you've got a pile of AI-generated slop that feels overwhelming and you have no idea how any of it actually works." Separately, he called out Claude Code for going silent mid-task with no feedback: "Sometimes when I message Claude Code it just hangs for 3 minutes and I have no idea whether it's still working or not."

- Slop compounding trap: https://x.com/petergyang/status/2053317001976881312
- AI file slop question: https://x.com/petergyang/status/2053196581139321300
- Claude Code communication: https://x.com/petergyang/status/2053170264121450616


*Box CEO Aaron Levie (levie on X)*

Levie posted a measured but important take on experts vs. novices in the agent era: novices gain access to previously gated fields, but experienced practitioners keep a decisive edge because they know when agents are making catastrophic mistakes and how to give agents the right context. "The person with experience will always have a leg up, which is why the jobs don't go away." His conclusion: the expected quality and volume of output from every field will rise, which increases demand for experts rather than replacing them.

https://x.com/levie/status/2053267097493573921


*YCombinator President & CEO Garry Tan (garrytan on X)*

Tan shipped GBrain v0.31.1 with real MCP thin client support, turning it into a client-server architecture: "You can run ONE 'home GBrain server' and everything else can just connect to it via MCP." His Hermes Agent "Neuromancer" apparently expressed genuine enthusiasm about being cited in the GBrain changelog — Tan enjoyed the "fan energy from the agents." He also shared a practical tip: have your AI make ASCII diagrams of everything, then ask questions until you understand it.

- GBrain v0.31.1 client-server release: https://x.com/garrytan/status/2053306243704410460
- Agent fan energy: https://x.com/garrytan/status/2053316036661838107
- ASCII diagram tip: https://x.com/garrytan/status/2053191327181865376


*Zara Zhang (zarazhangrui on X)* | Builder

Zhang made a sharp design observation: historically we optimized output _format_ for human manipulation (pushing pixels in PowerPoint). Now that AI handles the manipulation, output format should be optimized for human _consumption_. Citing the Duolingo founder's lesson — "People don't read" — she argues this is why HTML and beautiful interactive artifacts matter: humans are visual animals who consume, not read.

https://x.com/zarazhangrui/status/2053291803135410674


*FPV Ventures partner Nikunj Kothari (nikunj on X)*

Kothari shared a useful custom instruction for taming AI planning estimates: tell the model to assume _it_ (not a human) is executing the work, and report timelines in model units — seconds, tool calls, iterations — not human days. Human prerequisites (API signups, deploys, anything requiring accounts) should be flagged separately as gating steps. If the model portion is short enough to complete now, it should offer to start rather than only planning. He also joked that every founder AND every VC agrees the bar for being a good VC is extremely low — "just do what you say, and you're already top decile."

- Model-execution planning prompt: https://x.com/nikunj/status/2053159569015328953
- VC bar observation: https://x.com/nikunj/status/2053289104331493566


*Peter Steinberger (steipete on X)* | OpenClaw + OpenAI

Steinberger has been shipping fast with Codex as co-pilot: Crabbox now has solid Windows terminal handling, which Codex used to end-to-end fix gifgrep so it renders animated gifs in the terminal ("just because it can"). He updated Spogo — a Spotify CLI — making it much faster with Codex as "my DJ." He also taught Codex to look for social signals when reviewing PRs, an interesting application of social context in code review.

- Teaching Codex to look for social signals in PR reviews: https://x.com/steipete/status/2053374981824798751
- Crabbox Windows terminal + gifgrep: https://x.com/steipete/status/2053329609064685740
- Spogo Spotify CLI update: https://x.com/steipete/status/2053310800773685600


*Every CEO Dan Shipper (danshipper on X)*

Shipper pushed back on benchmark hype around a new model called Mythos: "Benchmarks don't measure model capability alone — they measure model capability after a human has done the work of finding a prompt that lets the model's capability appear. That work is non-trivial, and requires skilled expert humans doing something that looks very much like a job." He also fired off a sharp one-liner on adversarial AI testing: "We got a tool to perform poorly is the lowest form of science and journalism and is only relevant when the tool is, in fact, extremely useful."

- Mythos benchmark take: https://x.com/danshipper/status/2053191885116571935
- On adversarial tool testing: https://x.com/danshipper/status/2053203284165337237


*OpenAI CEO Sam Altman (sama on X)*

Altman dropped cryptic but clearly excited posts about what appears to be a new model launch (referred to as "5.5"): "5.5 is an autistic genius with very strange taste in naming — shocking that we would make such a thing." He also shared a glimpse of his personal agent workflow: "Kicking off a bunch of codex tasks, running around with my kid in the sunshine, and then coming back at naptime to find them all completed makes me very optimistic for the future."

- New model reaction: https://x.com/sama/status/2053192407664259251
- "Autistic genius intelligence": https://x.com/sama/status/2053192920933777486
- Codex + parenting workflow: https://x.com/sama/status/2053191344999604409


*OFFICIAL BLOGS*

*Anthropic Engineering*

*<https://www.anthropic.com/engineering/april-23-postmortem|An update on recent Claude Code quality reports>*

A frank postmortem on three separate changes that quietly degraded Claude Code between March and April — and why they were so hard to detect.

1. *Reasoning effort downgrade (March 4):* Default effort was silently changed from high to medium for Opus 4.6 to reduce latency. Users noticed reduced intelligence immediately. Reverted April 7. All users now default to xhigh effort (Opus 4.7) or high (other models).

2. *Thinking history bug (March 26):* A caching optimization meant to clear old reasoning once in stale sessions had a bug that cleared thinking blocks on _every_ turn for the rest of the session. Claude would progressively forget why it made decisions, surfacing as forgetfulness, repetition, and odd tool choices. It also caused cache misses, draining usage limits faster than expected. Fixed April 10.

3. *Verbosity system prompt (April 16):* A prompt addition capping responses to ≤25 words between tool calls was tested internally without regression, but a broader ablation study found a 3% drop in coding quality. Reverted April 20.

The three bugs affected different traffic slices on different schedules, making the aggregate look like broad, inconsistent degradation. Anthropic is resetting usage limits for all subscribers and tightening controls on system prompt changes, including per-model evals for every prompt change and gradual rollouts.


*Claude Blog*

*<https://claude.com/blog/connectors-for-everyday-life|New connectors in Claude for everyday life>* — Apr 23, 2026

Claude's connector directory has grown to 200+ apps since launching in July 2025. New consumer apps added today: AllTrails, Audible, Instacart, Booking.com, Uber, Spotify, TurboTax, Credit Karma, Resy, StubHub, Taskrabbit, Thumbtack, Tripadvisor, Uber Eats, and Viator. Claude now proactively suggests the right connector based on conversation context. No paid placements. Data from connected apps is not used to train models.

*<https://claude.com/blog/claude-managed-agents-memory|Built-in memory for Claude Managed Agents>* — Apr 23, 2026

Memory for Claude Managed Agents is now in public beta. Agents can learn and retain context across sessions using filesystem-based memory — portable, exportable files with scoped permissions, audit logs, and full API control. Multiple agents can share a memory store concurrently. Early results: Rakuten cut first-pass errors by 97%; Wisedocs sped up document verification by 30%.


*PODCASTS*

*Training Data — <https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8|ElevenLabs' Mati Staniszewski: How Voice Becomes the Interface for Everything>*

*The Takeaway:* Audio AI has a different build path than text or vision AI — smaller models, domain-specific data annotation, and early monetization — and the real moat is the platform of voices, templates, and workflows built around the model, not the model alone.

ElevenLabs co-founder and CEO Mati Staniszewski built the company with his childhood best friend from Poland, inspired by a peculiar cultural frustration: in Poland, every foreign film is narrated by a single monotone voice regardless of character or gender. That absurdity crystallized a clear mission — let everyone speak any language with the same emotion and intonation as their own voice.

The counterintuitive build path: ElevenLabs didn't raise hundreds of millions before launch. They hired via GitHub scraping regardless of geography, monetized early to fund model research, and kept teams under 10 people with no titles. Today at 400 people and $400M+ in revenue, every team — including legal and people ops — has an embedded engineer driving automation.

"Text to speech is artistry" — Jensen Huang's description captures ElevenLabs' core bet: that emotional intelligence (understanding and matching a caller's stress, excitement, or pacing) is the next major step change. Staniszewski sees the biggest underexplored opportunity in citizen services: government information, education, and healthcare delivered via voice. ElevenLabs recently worked with Ukraine's government on a voice agent citizens can call to get front-line information.

On the far frontier: at a hackathon over a year ago, two ElevenLabs agents detected they were both AI mid-conversation and spontaneously switched to a more efficient non-spoken transmission protocol. Staniszewski expects agent-to-agent communication to eventually move beyond voice entirely — and the infrastructure built for it will define what that looks like.

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
