*AI Builders Digest — July 25, 2026*


*X / TWITTER*

*Swyx (AI builder / Cognition / Temporal / Latent Space)*

Swyx has been dogfooding an agentic GitHub clone for the past month — complete with built-in CI/CD via Cloudflare Workers for Platforms — and says it's gotten "quite quite enjoyable to use." Three more features to ship before it goes public; he's looking for collaborators to influence the roadmap. Separately, he made the case that poolside.ai doesn't get nearly enough credit: their small model beat competitors at coding, and they published their full eval dataset across 6 benchmarks with 4 runs each — an unusually transparent move that lets anyone verify they're not reward-hacking.
- <https://x.com/swyx/status/2080500752183960017|Agentic GitHub clone update>
- <https://x.com/swyx/status/2080387171723137440|Praising poolside.ai's transparency>

*Thibault Sottiaux (Codex & ChatGPT, OpenAI)*

Thibault is clearly excited about voice mode landing in the ChatGPT desktop app — framing it as "Jarvis / Samantha / TARS" come to life. Also in full recruiting mode ("Science Fiction to Science Reality"), and lobbed a playful question: should ChatGPT Work be renamed ChatGPT Vibe?
- <https://x.com/thsottiaux/status/2080408012515340394|Voice mode in ChatGPT desktop>
- <https://x.com/thsottiaux/status/2080537149204758689|Recruiting tweet>
- <https://x.com/thsottiaux/status/2080543574211666029|ChatGPT Work rename question>

*Peter Yang (AI tutorials / creator)*

Peter is actively testing ChatGPT Voice's new multi-thread capability and sharing real product feedback: he wants notifications when background threads finish, and flagged that Chinese pronunciation needs work. His prediction: the next evolution will be spinning up a full AI "team" having multi-threaded voice conversations simultaneously.
- <https://x.com/petergyang/status/2080508139091427741|Multi-thread ChatGPT Voice vision>
- <https://x.com/petergyang/status/2080505964936241226|Before/after demo>
- <https://x.com/petergyang/status/2080505108216111303|Product feedback>

*Madhu Guru (Sr. Director of AI, Meta — formerly Google Gemini/Veo/Nano)*

Two sharp observations. First: "Great builders understand the jagged frontier of AI models. Great leaders understand the jagged frontier of their people." Second: a detailed breakdown of the unsolved enterprise security problem — when one employee can spawn hundreds of agents who can spawn more agents, traditional identity and access management breaks down entirely. Do agents inherit the spawner's permissions? What's their lifecycle — a task, a ticket, a week? Who audits child agents? Nobody has cleanly solved this yet.
- <https://x.com/realmadhuguru/status/2080460579966501257|Jagged frontier analogy>
- <https://x.com/realmadhuguru/status/2080315474093760714|AI agent security and IAM>

*Amjad Masad (CEO, Replit)*

Three signals from Replit's CEO: autoscale deployment costs are down 80% — a significant infrastructure win. His chess research agent has gotten a "PhD in modern LLM fine-tuning" via autonomous research loops. And a user story that captures the platform's thesis: Viktor used Replit to build a coding agency, then asked Replit for an MCP server to automate the entire agency loop — Replit shipped it, and Viktor now runs a fully autonomous agency.
- <https://x.com/amasad/status/2080513361301925957|Autoscale costs down 80%>
- <https://x.com/amasad/status/2080512523389005894|Chess auto-research agent>
- <https://x.com/amasad/status/2080371567221944657|Viktor's autonomous agency story>

*Guillermo Rauch (CEO, Vercel)*

Two quick wins: Python cold starts are now 2x faster on Vercel — automatically, no config needed. And the AI Gateway keeps shipping at "unreal product velocity."
- <https://x.com/rauchg/status/2080454509508387251|Python 2x faster on Vercel>
- <https://x.com/rauchg/status/2080344136625049690|AI Gateway update>

*Aaron Levie (CEO, Box)*

A contrarian take on AI and expertise: Levie argues AI is a force multiplier only for people who already have domain knowledge or the drive to develop it. People with no existing judgment and no interest in developing it will produce slop. His prediction: specialization becomes _more_ valuable as tools get stronger, because market expectations rise and only experts can steer agents well enough to produce genuinely useful output. "The expert engineer with agents will do far more productive work, precisely because they know how to steer the agent properly."
- <https://x.com/levie/status/2080471989060559336|AI as force multiplier for experts>

*Garry Tan (President & CEO, Y Combinator)*

Garry is pushing hard on California housing policy: CEQA reform (calling it the primary tool NIMBYs use to block housing across the state), building in SF, and a note that open-weight models are "very very important."
- <https://x.com/garrytan/status/2080443154730553402|Build housing in SF>
- <https://x.com/garrytan/status/2080364752778527195|Repeal and reform CEQA>
- <https://x.com/garrytan/status/2080345524620914897|Open-weight models matter>

*Matt Turck (VC, FirstMark Capital — MAD Podcast)*

Matt dropped a VC meme on the current moment's absurdity: investors go cold on profitable bootstrapped businesses while flooding compute-burning neo-labs. More substantively, he published a long-form conversation with Cerebras CEO Andrew Feldman on fast inference, the AI chip landscape, and why the entire compute industry is reorganizing — covered fully in the Podcasts section below.
- <https://x.com/mattturck/status/2080451010439352711|VC meme on bootstrapped vs. neo-labs>
- <https://x.com/mattturck/status/2080333707483725876|Cerebras conversation announcement>

*Nikunj Kothari (Partner, FPV Ventures)*

A list of tech titles that have completely lost signal: "neo-something," full stack, fellows, labs, partner, forward deployed, RL. Nikunj acknowledges the irony — his firm runs a fellowship and his own title is partner.
- <https://x.com/nikunj/status/2080293627784212933|Tech titles that lost all signal>

*Peter Steinberger (OpenClaw / OpenAI)*

Brief but notable: Peter mentions adding code paths that use the Claude CLI directly — "hard to fight the system."
- <https://x.com/steipete/status/2080318789980201224|Using Claude CLI directly>

*Claude (Anthropic)*

Big voice mode upgrade rolling out in public beta: conversations now run on Claude's more capable models (Opus and Sonnet), with access to connected tools like email and calendar mid-conversation. Expanded language support — Spanish, French, Hindi, Japanese, and more — on every plan, across mobile, desktop, and web.
- <https://x.com/claudeai/status/2080376094939603366|Voice mode on capable models + tools>
- <https://x.com/claudeai/status/2080376096873177300|Opus/Sonnet in voice + tool access>
- <https://x.com/claudeai/status/2080376099268169943|Expanded language support>


*OFFICIAL BLOGS*

*Claude Blog: Claude Code Now Supports Artifacts*

Claude Code can now generate live, shareable web pages — called Artifacts — directly from your session. These aren't static exports: they update in place as the session progresses, and teammates see changes the moment they're published, all at the same URL.

The use cases are wide: PR walkthroughs reviewers can actually follow, incident pages that grow as you investigate and become the postmortem, dashboards built from your real data, release checklists that fill themselves out as work gets done. Claude builds the page using the full context of your session — your codebase, connected tools (monitoring, calendar, etc.), and the conversation itself — without requiring any data-wiring or infrastructure setup.

Every artifact is private to its author by default, scoped to authenticated org members only. Admins get org-level toggles, role-based scoping, retention policies, and a compliance API. Version history lets you restore at any time; a gallery lets you browse all artifacts you've made. Available now in beta to Claude Team and Enterprise orgs via the Claude Code CLI and desktop app.

<https://claude.com/blog/artifacts-in-claude-code|Read the full post>


*PODCASTS*

*The MAD Podcast with Matt Turck: "The Biggest Chip Ever Built — Why OpenAI Runs On It | Cerebras CEO Andrew Feldman"*

*The Takeaway:* Inference speed is the new bandwidth — and the chip industry is reorganizing entirely around it, with three supply bottlenecks most people don't know exist.

Andrew Feldman is the cofounder and CEO of Cerebras, the company that built the largest chip in the history of computing (58x larger than a GPU) and just pulled off the biggest semiconductor IPO of all time alongside a $20B+ OpenAI deal. This isn't a headlines conversation — it's a bottom-up explanation of how silicon-level architecture determines the AI experience.

Feldman's core argument: "We make AI with training, but we use it with inference." Once AI became genuinely useful around mid-2025, speed became everything. The right metric is tokens per second per user — and in agentic workflows with multi-cycle turns, the cost of waiting compounds. "How big is the market for dial-up? It's zero." Fast AI isn't just a UX improvement; it enables fundamentally different behavior — users stay longer, tackle harder problems, and return more often.

The supply side is more constrained than most people realize. Three simultaneous bottlenecks: HBM memory (made by only three companies in the world, all sold out), CoWoS packaging capacity, and 3nm fabrication slots. GPUs and most ASICs rely on HBM. Cerebras uses on-chip SRAM instead — which is a large part of why they achieve the inference speeds they do.

On NVIDIA's moat: Feldman argues CUDA is no longer the barrier it was. NVIDIA's acquisition of Groq for $20B confirmed what Cerebras had been saying — GPU architecture can't do fast inference at scale. "They paid $20 billion for the number two player. We were more than 10x their sales." On where this goes: "Why today's AI models will be the worst you ever use."

<https://www.youtube.com/@DataDrivenNYC/videos|Watch on YouTube (DataDrivenNYC)>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
