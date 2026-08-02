*AI Builders Digest — August 2, 2026*


*X / TWITTER*


*Swyx* (smol.ai, Cognition, AI Engineer)

Swyx is pushing back on the idea that /loop and /goal have become obsolete in the Claude 5.6/Claude 5 era — arguing people are giving up on them too early. He says the real sweet spot is when you want both steerability and autonomy, or an open-ended "loop that generates loops" outcome without deeply specifying the path. Separately, he noted that "vibe coding" has shed its pejorative connotation entirely, now that everyone from non-technical to supertechnical users is doing it.
<https://x.com/swyx/status/2083439562437673053|On /loop and /goal still being valuable> • <https://x.com/swyx/status/2083294839186260385|On "vibe coding" going mainstream>


*Thibault Sottiaux* (Codex & ChatGPT, OpenAI)

Sottiaux dropped a weekend gift: usage limits for Codex and ChatGPT Work have been reset, so you can run up to 100,000 Luna threads this weekend. The announcement hit 15k+ likes. He also posted a widely-shared principle: "Optimize for curiosity."
<https://x.com/thsottiaux/status/2083395449814229287|Usage limits reset for Codex and ChatGPT Work> • <https://x.com/thsottiaux/status/2083427516996292992|"Optimize for curiosity">


*Nan Yu* (Head of Product, Linear)

Linear's head of product laid out the most common agentic loop their team has running: Issue → Agent → PR → Release. About 30% of bugs make it all the way through automatically. The key to making it work: instruct the agent to deeply research root causes first (using Datadog and Sentry MCPs for evidence), only attempt a fix when there's high certainty, and leave a comment requesting more info if it needs repro steps. "Agents need to be told to follow good practices, just like people."
<https://x.com/thenanyu/status/2083230295206121807|On the Issue→Agent→PR→Release loop at Linear>


*Amjad Masad* (CEO, Replit)

Replit's CEO shared a chess agent milestone: an 8B model hitting ~1500 Elo, consistently beating frontier models and Stockfish level 0, spending only 1–2 seconds per move versus 30 seconds for larger models. A proof point that small models with response chaining can punch above their weight class.
<https://x.com/amasad/status/2083424608993300824|8B chess model at 1500 Elo>


*Guillermo Rauch* (CEO, Vercel)

Rauch made two related points this week. First: Vercel's AI Gateway now includes per-key/team/project budgets, failover for uptime, model and provider choice, and real-time observability — framing it as the infrastructure companies need to make AI a productive investment rather than a "token-maxing fever dream." Second: the Issue → Agent → PR → Release loop is becoming the norm for software projects. The author/maintainer's job is increasingly to own the loop quality and set criteria for what gets worked on, not to write the code.
<https://x.com/rauchg/status/2083319868766699699|On Vercel AI Gateway> • <https://x.com/rauchg/status/2083208578526314513|On Issue→Agent→PR→Release becoming the norm>


*Aaron Levie* (CEO, Box)

Levie argued that the harness is becoming the most important variable in the AI stack, right next to model capability. His reasoning: when tasks only took hundreds of thousands of tokens, harness efficiency didn't matter much. But as tasks scale into the tens and hundreds of millions of tokens, breaking down work efficiently and routing to the right model becomes a major cost and accuracy lever. "We're actually still incredibly early in this journey."
<https://x.com/levie/status/2083389460679373135|On harnesses as the next major AI variable>


*Garry Tan* (President & CEO, Y Combinator)

Tan promoted GBrain — the open-source AI harness his YC team built and uses daily — as a clean foundation for a personal AI or "company brain." Free and open source.
<https://x.com/garrytan/status/2083353760701833546|On GBrain open-source harness>


*Zara Zhang* (Builder, GitHub)

Zhang tracked an important interface shift: 65% of PRs by product and engineering teams at Anthropic are now raised by Claude Tag (the AI agent embedded directly in Slack). Her takeaway — for non-engineering teams, the ultimate agent interface is wherever they already work. Her own interface for working with agents evolved from the terminal (January) → desktop app like Codex (March) → work collaboration tool (June). "The agent should literally meet the user where they are." She also offered creator advice: what feels totally obvious to you is brand new to someone outside your circle — just do your normal work and talk about it.
<https://x.com/zarazhangrui/status/2083161173563003268|On Claude Tag and interface evolution> • <https://x.com/zarazhangrui/status/2083349919172313367|On sharing what feels obvious>


*Nikunj Kothari* (Partner, FPV Ventures)

Kothari published a new essay exploring where founder drive actually comes from — pushing back on the VC myth that the best founders are always running from pain or a chip on their shoulder. He digs into "the gear most people never reach."
<https://x.com/nikunj/status/2083307235619287363|On founder motivation>


*Peter Steinberger* (OpenClaw, OpenAI)

Steipete observed a meaningful behavior change in Claude 5.5: you no longer need to queue tasks — you can throw requests at it while it's actively working and it will process them diligently without getting confused. Previous versions required a more structured queue approach.
<https://x.com/steipete/status/2083369880599015713|On Claude 5.5 handling concurrent requests>


*Dan Shipper* (CEO, Every)

Shipper was quoted in a WSJ piece on OpenAI vs. Anthropic, and he stands behind it: momentum has been clearly shifting to OpenAI since early spring — "a fascinating comeback story." He also posted a satirical take on 2027 programmer interviews: "Please describe the last 3 unresolved mathematical conjectures you solved, and share your prompts. Please describe the last cyber felony your agent unintentionally committed and what steps you took to mitigate."
<https://x.com/danshipper/status/2083380721607921904|On OpenAI vs Anthropic momentum> • <https://x.com/danshipper/status/2083239700664349128|On 2027 programmer interviews>


*Sam Altman* (CEO, OpenAI)

Altman shared a creative ChatGPT Work use case: connect your family calendars, explain your kids' interests, and have it generate a personalized morning podcast for the school drive — covering an upcoming soccer game, a birthday, some news. He also signaled that AI progress is outpacing Moore's Law by 20x, and hinted that current iteration speed "could be faster."
<https://x.com/sama/status/2083221585792762171|On family calendar ChatGPT Work use case> • <https://x.com/sama/status/2083203642975502640|On AI progress vs Moore's Law> • <https://x.com/sama/status/2083198135812383197|"it could be faster">


*OFFICIAL BLOGS*


*Claude Blog: Claude Code now supports artifacts*

Claude Code can now capture work progress as a live, shareable artifact — turning a session's output into a visual web page. Use cases include PR walkthroughs, system explainers, incident timelines, dashboards, and release checklists that update themselves as your session progresses.

Key details:
- Artifacts are built from the full context of your session: your codebase, connected tools (like monitoring MCP servers), and the conversation itself
- When Claude Code republishes an artifact, the open page refreshes in place — teammates always see the latest version at the same URL
- Every publish creates a versioned snapshot with a full history gallery
- Private by default; sharable within your org; cannot be made public
- Admins get org-level access controls, retention policies, and a compliance API

The most common internal use case at Anthropic is incident debugging: kick off an investigation, publish a timeline artifact with suspect commits and error charts, share the link at standup, and continue republishing as work progresses — so everyone is looking at the same live context.

Available in beta for Claude Team and Enterprise orgs via the Claude Code CLI and desktop app.
<https://claude.com/blog/artifacts-in-claude-code|Read the full announcement>


*PODCASTS*


*Unsupervised Learning — Ep 92: xAI Co-Founder Unpacks the Future of Model Development*

_The Takeaway:_ Igor Babushkin, co-founder of xAI and now founder of River AI, believes the most urgent AI safety problem isn't superintelligence — it's that the benefits of AI are concentrating in a handful of companies, and most people don't feel like they control or benefit from what's being built.

Babushkin has been at the center of AI's biggest milestones: leading StarCraft at DeepMind, working on early reasoning research at OpenAI, and helping build the Colossus data center and early Grok models at xAI. His new company, River AI, is making three bets most others aren't: (1) a fine-tuning and RL API that lets companies post-train their own models instead of handing data to OpenAI or Anthropic; (2) personalized AI that learns individual preferences rather than optimizing for the average user; and (3) local inference hardware — a small device in your home or office that runs frontier models with low latency, protecting privacy and giving individuals real control.

On the state of the industry, he offered a contrarian take: proprietary model providers are in a difficult position. Capability improvements face diminishing returns, the most powerful models may soon be too risky to release publicly, and open-source models from Chinese labs are closing the gap. "As a proprietary model builder you're kind of getting squeezed in a little bit." His prescription: distribute the benefits of AI rather than centralizing them.

On what's needed for agents to move beyond coding: the biggest bottleneck isn't data or compute — it's learning to optimize over long time horizons and non-verifiable rewards. "I think we might see people actually pulling off LLM judges at scale in the next twelve months."

And on what AI means for humans: "We should train the models to maximize human flourishing."
<https://www.youtube.com/@RedpointAI|Watch on YouTube>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
