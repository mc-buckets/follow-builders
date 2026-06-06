AI Builders Digest — June 6, 2026

*X / TWITTER*

*Alex Albert — Research at Anthropic*
Shared a milestone: over 80% of all code merged into Anthropic's codebase is now written by Claude, with the typical engineer shipping 8x as much code as they did in 2024. On the most open-ended tasks, Claude's success rate jumped from ~26% to 76% in just six months. The kicker: when research sessions went off-track, Claude proposed a better next step than the human took 64% of the time. "We're not at recursive self-improvement yet, but it could come sooner than most expect."
<https://x.com/alexalbert__/status/2062580571214389510|View tweet>

*Thibault Sottiaux — Codex & ChatGPT at OpenAI*
Announced that Codex is now usable within your own programs via the Python SDK (`pip install openai-codex`). <https://x.com/thsottiaux/status/2062734215494664697|View tweet>

Also disclosed a bug being fixed that was causing tokens served to some Codex Pro and Plus accounts to be undercounted — affecting less than 15% of accounts. "Not the kind of bug you want us to fix, but didn't want to do this silently." <https://x.com/thsottiaux/status/2062648326332539015|View tweet>

*Sam Altman — CEO of OpenAI*
Announced a big upgrade to ChatGPT memory rolling out today. <https://x.com/sama/status/2062660086787613116|View tweet> Also teased ChatGPT's new ability to build and publish web apps directly, saying he missed HyperCard and wished he'd had this as a kid — right before nostalgia-posting "man the early days of the internet were so special." <https://x.com/sama/status/2062661071761211561|View tweet>

*Swyx — affiliated with Cognition (Devin), Temporal, and AI Engineer community*
Highlighted the first eval release from Cognition: real-world enterprise code evals capped at 100 hours (versus METR's 16-hour cap), with a financial guarantee on the results. Their dataset covers Java/TypeScript/Python/C# feature dev, bugfixes, and migrations — 258 sessions from 126 users across diverse enterprise customers. "This is pioneering real world evals work."
<https://x.com/swyx/status/2062611218196771017|View tweet>

Also commented that Singapore investors are finally taking Neon (a leading database company born in Singapore) seriously. <https://x.com/swyx/status/2062627150885450065|View tweet>

*Thariq — Claude Code at Anthropic*
Reflected on the "An App Can Be a Home-Cooked Meal" essay: "personal software was a bit early in 2020 but in 2026, it really can be as personal as a home cooked meal, or a handwritten letter." <https://x.com/trq212/status/2062605395101884916|View tweet>

Also shared a post on how dynamic workflows allow Claude Code to handle whole new types of tasks. <https://x.com/trq212/status/2062556889171517499|View tweet>

*Cat Wu — Claude Code at Anthropic*
Hiring a PM for Claude Code focused on model performance. Looking for someone with experience writing agentic evals who wants to integrate research ideas into the core product.
<https://x.com/_catwu/status/2062659533047259212|View tweet>

*Aaron Levie — CEO of Box*
Responding to Anthropic's post on Claude's growing role in internal development, highlighted the key insight: AI creates far more ideas than any organization can pursue, and the bottleneck shifts to execution. "The rate at which organizations can spot and fix these bottlenecks may be a skill that improves over time, and it may become the most important skill for any organization." AI doesn't eliminate the need for people to manage — it multiplies the scope of what needs to be managed.
<https://x.com/levie/status/2062728257359790292|View tweet>

*Peter Yang — Product at Roblox, AI tutorials newsletter*
Spent a full day setting up integrations and skills in Codex for his top creator workflows, concluding you can save at least 50% of your time on knowledge work by investing in the system upfront. His 3-step process: reflect on your most painful manual workflow, list every step in detail, then ask Codex or Claude Code what integrations to build. "AI will guide you the rest of the way."
<https://x.com/petergyang/status/2062740262338929110|View tweet>

Also noted Codex still has a weak frontend design compared to Claude: "Claude can one-shot great looking HTML slides." He argues the UI is often a novice's first impression and Codex needs to improve it. <https://x.com/petergyang/status/2062743491365544361|View tweet>

*Dan Shipper — CEO of Every*
Launched Spiral 4.0, a writing partner powered by a new Style Engine built on stylometry principles — it extracts your brand voice from examples of past work. Now supports MCP and CLI so agents like Codex and Claude Code can invoke it automatically. Every uses it internally for landing pages, tweets, podcasts, and marketing emails across the full 30-person team.
<https://x.com/danshipper/status/2062628079869005876|View tweet>

*Nikunj Kothari — Partner at FPV Ventures*
Built a personal Claude Code skill called "Nock" trained on 200+ founder pitch meeting notes captured by Granola, distilled to ~53 sessions with substantive debate. The result is a question bank grounded in real VC conversations that evaluates decks in his voice. He iterated against 5-10 actual decks until it felt accurate. Founders can try it at nikunjk.com/nock; VCs can build their own version at nikunjk.com/buildnock.
<https://x.com/nikunj/status/2062659649732825549|View tweet>

*Guillermo Rauch — CEO of Vercel*
Congratulated the Void team and reaffirmed Vercel's collaboration on an open web platform, with investment in Nitro.js and native support for Vite-based frameworks including Nuxt, Svelte, and TanStack Start.
<https://x.com/rauchg/status/2062535454130676193|View tweet>

*Garry Tan — President & CEO of Y Combinator*
Celebrated two YC decacorns in one day, including Polaris — a commercial fusion company that hit 150 million degrees Celsius, the first privately funded machine to do it. "This is the abundance future, built by people who actually ship."
<https://x.com/garrytan/status/2062763109849411834|View tweet>

Also a reminder to founders: "So close to product market fit is still not product market fit."
<https://x.com/garrytan/status/2062761266083754088|View tweet>

*Claude — Anthropic's official AI account*
Featured Anton Osika, co-founder and CEO of Lovable: "His working thesis: the most underrated moat in AI is trust, and earning it takes craft, care, and obsession."
<https://x.com/claudeai/status/2062558332695556378|View tweet>

*Aditya Agarwal — General Partner at South Park Commons*
Noted that many roles will have engineering infused into them going forward, citing Marketing Engineer as a prime example of the trend.
<https://x.com/adityaag/status/2062655784127971565|View tweet>

*Josh Woodward — VP at Google Labs, Gemini*
Expressed enthusiasm for a new Gemini feature on the macOS app.
<https://x.com/joshwoodward/status/2062667951485108354|View tweet>


*OFFICIAL BLOGS*

*Anthropic Engineering*

_An update on recent Claude Code quality reports_
A candid postmortem on three separate bugs that degraded Claude Code quality between March and April. Issue 1: default reasoning effort was quietly downgraded from high to medium to reduce latency, but users immediately noticed reduced intelligence — reverted April 7. Issue 2: a caching bug caused Claude to continuously drop its prior thinking blocks after sessions idle for over an hour, making it appear forgetful and repetitive — fixed April 10. Issue 3: a system prompt instruction limiting responses to 25 words between tool calls hurt coding quality — reverted April 20. Because each bug affected different traffic slices on different schedules, the aggregate looked like broad, inconsistent degradation. Anthropic is resetting usage limits for all subscribers and committing to broader eval suites, soak periods, and tighter controls on system prompt changes.
<https://www.anthropic.com/engineering/april-23-postmortem|Read the full post>

_Scaling Managed Agents: Decoupling the brain from the hands_
Anthropic explains the architecture behind Managed Agents, their hosted service for long-horizon agent tasks. The key design move: decoupling Claude (the "brain") from execution sandboxes (the "hands") and from the session log, so each component can fail or be replaced independently. Credentials never enter the sandbox where generated code runs. Result: p50 time-to-first-token dropped ~60% and p95 dropped over 90%. The system is a "meta-harness" — opinionated about interfaces, not about what runs behind them — so it can accommodate future harness implementations without breaking existing integrations.
<https://www.anthropic.com/engineering/managed-agents|Read the full post>

*Claude Blog*

_New in Claude Managed Agents: self-hosted sandboxes and MCP tunnels_
Claude Managed Agents now supports running agent execution inside your own infrastructure or with managed providers including Cloudflare, Daytona, Modal, and Vercel — keeping sensitive files and code within your security perimeter while Anthropic handles orchestration. MCP tunnels (in research preview) let agents reach private MCP servers inside your network without exposing them to the public internet — a lightweight gateway you deploy makes a single outbound connection, no inbound firewall rules required.
<https://claude.com/blog/claude-managed-agents-updates|Read the full post>

_New connectors in Claude for everyday life_
Claude now connects to AllTrails, Audible, Booking.com, Instacart, Intuit Credit Karma, Intuit TurboTax, Resy, Spotify, StubHub, Taskrabbit, Thumbtack, Tripadvisor, Uber, Uber Eats, and Viator — joining 200+ connectors already in the directory. Claude now dynamically suggests the right connector mid-conversation based on what you're doing. Connected service data is not used for model training, Claude remains ad-free with no paid placements, and you can disconnect any service at any time.
<https://claude.com/blog/connectors-for-everyday-life|Read the full post>


*PODCASTS*

*The MAD Podcast with Matt Turck — OpenAI's Dan Roberts: Why AI Can Now Make Discoveries*

*The Takeaway:* Reinforcement learning is no longer the cherry on top of pre-training — it's increasingly the cake — and AI has already crossed into genuine original scientific discovery.

Dan Roberts leads the Foundations of Reinforcement Learning team at OpenAI, arriving via a PhD in theoretical physics at MIT (quantum gravity and black hole information theory), a postdoc at the Institute for Advanced Study, time at FAIR, a startup, and a stint at Sequoia Capital as entrepreneur-in-residence. He joined OpenAI two years ago to work at what he sees as a convergence between physics and intelligence research.

His core argument: RL started working not because of a new algorithm, but because pre-trained models became powerful enough to build on. "If you have a powerful enough pre-trained model, then it can start to do well at RL." From there, RL teaches models to actually _use_ test-time compute — to generate a running thought process before committing to an answer.

On the OpenAI Erdős problem result, Roberts framed it as fundamentally an act of exploration: the model assumed the conjecture was false (against mathematical consensus), then persevered down an extremely long calculation path drawing on algebraic number theory. "When you go against the grain and do something contrarian like that, you really have to have strong conviction in what you're doing in order to persevere down a really long calculation path."

His physics-trained instinct applied to AI: when a model "grokks" or shows unexpected emergent behavior, that's not magic — it means you didn't understand what you were scaling up. The fix is to find a simpler toy system that still contains the phenomenon, understand it there, then scale with intent. "If you can figure out what to put into the small thing, then you understand the thing."

<https://www.youtube.com/watch?v=oWOz2htozfI|Watch on YouTube>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
