AI Builders Digest — June 9, 2026

*X / TWITTER*

*Boris Cherny* (Claude Code at Anthropic)

Boris Cherny shared five tips for running Claude Opus autonomously for hours or days: (1) enable auto mode for permissions so Claude doesn't ask for approval, (2) use dynamic workflows to orchestrate hundreds or thousands of agents, (3) use /goal or /loop to keep Claude working until done, (4) run Claude Code in the cloud so you can close your laptop, and (5) make sure Claude has a way to self-verify its work end to end — browser extension for web, iOS/Android simulator MCP for mobile, a full web server for backend.
<https://x.com/bcherny/status/2063792263067754658|View tweet>

*Thibault Sottiaux* (Codex & ChatGPT at OpenAI)

Thibault Sottiaux announced a 100-day Codex challenge: every day for the next 100 days, OpenAI will select one person doing impressive or incredibly useful work with Codex and give them 10x usage limits for a month. The first winner gets announced tomorrow.
<https://x.com/thsottiaux/status/2063748242681307611|View tweet>

*Madhu Guru* (former Product Leader at Google Gemini, Veo, Nano)

Madhu Guru pushed back on the assumption that AI training data is low-skill grunt work. The data required to advance the model frontier is the opposite: complex, domain-specific knowledge for high-economic-value tasks, most of which have little documentation. This is exactly why we have SWE agents but not knowledge-work agents yet. He argues companies producing this training data are doing "extremely high-leverage, high-skill work" that is "critical to moving AI forward — and deeply underappreciated."
<https://x.com/realmadhuguru/status/2063704354910347520|View tweet>

*Amjad Masad* (CEO at Replit)

Replit CEO Amjad Masad quote-tweeted a founder success story, summarizing Replit's core value proposition as "removing all distractions and having you focus on what matters — getting to market and getting the bag."
<https://x.com/amasad/status/2063744208587125142|View tweet>

*Guillermo Rauch* (CEO at Vercel)

Vercel CEO Guillermo Rauch shared that the Vercel AI Gateway recovers over 1 trillion tokens per month on average — analogous to how Stripe recovers revenue through smart retries on failed payments. The gateway adds redundancy, zero-data retention enforcement, observability, usage APIs, and caps, all with zero markup over the AI labs.
<https://x.com/rauchg/status/2063714700618334260|View tweet>

*Aaron Levie* (CEO at Box)

Box CEO Aaron Levie had three substantive posts.

He argued AI hasn't reduced GTM costs in enterprise software — if anything it's increased them. Cheaper software development shifts the hard problem to discoverability and market differentiation: "If you make one thing cheaper and more abundant (development of software) then the new problem of discoverability and market differentiation (GTM) becomes the hardest part."
<https://x.com/levie/status/2063756386572681606|View tweet>

On model routing, Levie predicted a split between frontier intelligence for high-end tasks and cheaper models for high-volume workloads — and argued "the layer that can efficiently route the workload to the right model will become increasingly valuable — agent orchestration that can cost-optimize while still performing the task successfully will be in a strong position."
<https://x.com/levie/status/2063835799096090749|View tweet>

He also announced Box now has a markdown editor on the web with full CLI support, commenting, and version history. Box Drive can be mounted as a local drive so files are instantly accessible in Claude Cowork, Codex, Obsidian, Cursor, or any other app.
<https://x.com/levie/status/2063649508681224367|View tweet>

*Garry Tan* (President & CEO at Y Combinator)

Y Combinator CEO Garry Tan flagged that "educating people on how to use the AI tools has become a serious bottleneck" — pointing to a shift where the tools are no longer the limiting factor; adoption and change management are.
<https://x.com/garrytan/status/2063786111588323780|View tweet>

He also shared a GBrain product update: version 0.42.30 can now give you a detailed summary of how your thinking has changed over time.
<https://x.com/garrytan/status/2063785286367392095|View tweet>

*Zara Zhang* (independent AI builder)

Zara Zhang reflected on why her Frontend Slides skill grew so organically: "slides are inherently social." People see HTML-based decks and ask how they were made, and creators of those slides are perceived as "more AI-native and AI-savvy." The format has a viral loop built right into it.
<https://x.com/zarazhangrui/status/2063638307586662539|View tweet>

*Nikunj Kothari* (Partner at FPV Ventures)

FPV Ventures partner Nikunj Kothari offered a contrarian take on the token anxiety trend: companies should still give employees copious token budgets to stay at the frontier and explore the edges. Cutting back makes it "way too easy to fall back to doing the things how they have always been done."
<https://x.com/nikunj/status/2063630238123483195|View tweet>

*Peter Steinberger* (OpenClaw co-creator, collaborates with OpenAI)

The most viral post of the day: Peter Steinberger's blunt reminder that "you shouldn't be prompting coding agents anymore — you should be designing loops that prompt your agents." The tweet hit 13,700+ likes and 870 retweets, sparking widespread discussion about how the mental model for AI-assisted development needs to shift.
<https://x.com/steipete/status/2063697162748260627|View tweet>

*Aditya Agarwal* (General Partner at South Park Commons, former CTO at Dropbox)

South Park Commons GP Aditya Agarwal — who went through both the Meta and Dropbox IPOs — noted that "fabulous wealth tends to amplify deeper desires, not create new ones." With a wave of liquidity expected in the coming months, he predicts many of those people will start new things, fund new things, and keep the Silicon Valley flywheel spinning.
<https://x.com/adityaag/status/2063731771284619521|View tweet>

*Sam Altman* (CEO at OpenAI)

OpenAI CEO Sam Altman quote-tweeted Thibault Sottiaux's Codex 100-day challenge with a one-liner: "interesting recursive loop here maybe" — pointing at the meta irony of using Codex to find and reward the best Codex power users.
<https://x.com/sama/status/2063779477419901071|View tweet>


*OFFICIAL BLOGS*

*Claude Blog — New in Claude Managed Agents: dreaming, outcomes, and multiagent orchestration*
<https://claude.com/blog/new-in-claude-managed-agents|Read the full post>

Anthropic launched three new capabilities for Claude Managed Agents. _Dreaming_ is a scheduled background process that reviews past agent sessions and memory stores, extracts patterns, and curates memories so agents improve over time — it can update memory automatically or hold changes for human review. Harvey (legal AI) tested it and saw completion rates go up ~6x. _Outcomes_ lets developers write a success rubric; a separate grader evaluates the agent's output in its own context window and sends the agent back for another pass when something isn't right. In testing, outcomes improved task success by up to 10 points, with the largest gains on the hardest problems, and improved file generation quality by +8.4% on docx and +10.1% on pptx. _Multiagent orchestration_ lets a lead agent break complex jobs into pieces and delegate each to a specialist agent with its own model, prompt, and tools, all running in parallel on a shared filesystem, with full trace visibility in the Claude Console. Netflix and Spiral by Every are among the early teams using these capabilities.


*PODCASTS*

*The MAD Podcast with Matt Turck — State of Enterprise AI 2026: Aaron Levie on Tokenmaxxing, Rise of Headless, and AI-Proofing Your Job*
https://www.youtube.com/watch?v=Gs2styCcwro

_The Takeaway:_ Enterprise AI deployment is taking longer than expected — not because the technology isn't good enough, but because it's advancing faster than companies can build stable architectures around it.

Box CEO Aaron Levie, who speaks with hundreds of CIOs every year, offers a uniquely grounded view on how AI is actually landing inside the world's largest companies. The mood is cautiously optimistic: CIOs are seeing real productivity gains in engineering and are being pulled by their business teams to extend those gains everywhere else. The challenge isn't enthusiasm — it's execution.

The token cost conversation is real but often misframed. The deeper issue is that AI agents consume compute in a fundamentally different way than chatbots: one coding session can cost $1,000. "We've just gone from a pricing model of a chatbot to that pricing model no longer working when one coding agent could be consuming $1,000 of compute on a single task." As token budgets escape the IT department and move into line-of-business budgets, companies will need entirely new FinOps muscle — there's no "FinOps for the marketing team" yet.

On why coding is ahead of the rest of knowledge work: coding is uniquely suited for AI agents because work is verifiable, users are technical, and the codebase provides rich context. Most knowledge work lacks all three. The blockers are access controls, unstructured data scattered across dozens of systems, and the absence of technical users who can catch and correct agent mistakes.

Levie is bullish on the "internal FDE" role — a technical person embedded within a business team who understands workflows and wires up agents to get real work done. This is a sustaining job, not a transitional one: every model upgrade creates new work.

On headless software: a dual model emerges — agents doing high-volume headless work at massive scale, humans using the interface for complex or judgment-intensive tasks. Enterprise software companies will run both a seat business and a consumption business. And on jobs: Levie is a committed Jevons paradox believer — productivity gains don't shrink the demand for roles, they expand the total amount of work worth doing.


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
