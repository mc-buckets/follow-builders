*AI Builders Digest — June 7, 2026*


*X / TWITTER*

*Swyx* (AI & Engineer — Latent Space, Cognition, Temporal)
Swyx shared a sharp prompting tip: instead of defaulting to plan mode, frame your task as a question so the model is invited to push back and suggest alternatives rather than blindly executing what you said (which is often not precisely what you meant). "Literally just appending '?' to the end of your prompt often does it."
<https://x.com/swyx/status/2063082950317486133|tweet>

*Boris Cherny* (Claude Code @ Anthropic)
Boris announced that Claude Cowork's usage limits have been doubled for the next month. He described Cowork as best for work "too big for a chat" — research across dozens of accounts, recurring reports, and inbox triage. If you've been saving a big messy project, now's the time.
<https://x.com/bcherny/status/2063028954546733462|limits announcement> · <https://x.com/bcherny/status/2063028956211867837|use cases>

*Thibault Sottiaux* (Codex & ChatGPT @ OpenAI)
Thibault dropped a tight equation: "Better memory = Shorter prompts = More utility per token." He also noted that Codex papercuts are falling as adoption climbs — a healthy product signal.
<https://x.com/thsottiaux/status/2062966625733861752|memory tweet> · <https://x.com/thsottiaux/status/2062997768470474765|Codex adoption tweet>

*Peter Yang* (Product @ Roblox, 140K+ reader AI newsletter)
Peter shared a 5-step framework for building self-improving AI skills: (1) give it examples of good output so it knows what good looks like, (2) write a clear trigger description, (3) add pass/fail evals for common errors, (4) add a memory file to capture one-sentence learnings from past runs, and (5) build a skill that cleans up other skills by removing stale or duplicate instructions.
<https://x.com/petergyang/status/2062899832965255443|framework tweet>
He also interviewed a builder who contributes to Python and Go repos despite no CS degree, crediting Every's Compound Engineering workflow.
<https://x.com/petergyang/status/2062959766314582064|interview tweet>

*Madhu Guru* (ex-Product Leader @ Google — Gemini, Veo)
Madhu called out a common enterprise AI mistake: building for today's model capabilities and price points. His advice — think 6 months out, scaffold around current model weaknesses, and bet that the next generation will natively solve those gaps. "Over time, that ability to repeatedly identify and bridge model gaps becomes a moat of its own."
<https://x.com/realmadhuguru/status/2063024953721827329|tweet>

*Amjad Masad* (CEO @ Replit)
Amjad teased a Replit x Shopify partnership.
<https://x.com/amasad/status/2063065480878063694|tweet>

*Guillermo Rauch* (CEO @ Vercel)
Vercel announced that agent filesystem state can now be read, written, and mounted independently of Sandbox lifecycle — storage decoupled from compute, attachable to Builds, Functions, and Sandboxes. Rauch also promoted Vercel's Skills API, describing it as "the npm registry for agent capabilities and extensibility. Free and open."
<https://x.com/rauchg/status/2063009510503932181|filesystem tweet> · <https://x.com/rauchg/status/2062951924677128455|Skills API tweet>

*Aaron Levie* (CEO @ Box)
Aaron made a counterintuitive case against AI displacement fears: if coding agents — which have every structural advantage (verifiable output, digitized context, technical users, massive training data) — still require human engineers to be effective, then the risk in other knowledge work is lower than perceived. "Agents will let people do far more than they did before, but the people don't go away."
<https://x.com/levie/status/2063055332545540096|tweet>

*Ryo Lu* (Design @ Cursor)
Cursor's Ryo Lu showed off a new design-in-code workflow: click to select an element, chat to edit it, shift-click to multi-select. Works best with Composer 2.5.
<https://x.com/ryolu_/status/2063038983408615435|tweet>

*Garry Tan* (President & CEO @ YCombinator)
Garry teased a project he's been quietly building for months — something aimed at helping people learn better techniques to build software faster.
<https://x.com/garrytan/status/2063146456106795457|tweet>

*Aditya Agarwal* (General Partner @ South Park Commons, ex-CTO @ Dropbox)
Aditya offered a sharp reminder: "Sometimes speed is just impatience disguised as ambition."
<https://x.com/adityaag/status/2062917027103130013|tweet>

*Claude / Anthropic*
Claude's official account confirmed that doubled Cowork usage limits are live on all paid plans through July 5. Download the Claude desktop app to try it.
<https://x.com/claudeai/status/2063018337567670285|announcement> · <https://x.com/claudeai/status/2063018339710992794|desktop app link>


*PODCASTS*

*AI & I by Every — "The SaaS Apocalypse Is a Goldmine With Figma's Matt Colyer"*

*The Takeaway:* The "SaaS apocalypse" narrative misunderstands what software companies actually provide — and if you're in that space, the explosion of builders isn't a threat, it's a gold mine.

Matt Colyer is Director of Product Management for Developers at Figma. He's spent years in developer tools, built his own AI agents long before it became trendy, and now leads Figma's response to the agent era — including Figma's native agent for the Infinite Canvas and the Figma MCP server.

His core argument: the number of developers worldwide is moving from ~30 million toward potentially a billion. More builders means more software, which means more demand for the tools that make software good. "If you're in that space, it means it's a gold mine."

A few specific insights worth knowing:

- *Vibe-coding doesn't eliminate maintenance.* Colyer built his own email agent two years ago — a Python script that grabbed school PTO emails for his three kids and summarized them into bullet points. He's found the ongoing cost of running your own agent is real, and he now buys more software than before: "That tool seems cool. I'm just gonna pay somebody else to run my agent for me."

- *Figma's MCP strategy is bidirectional.* The Figma MCP server supports two flows: code → design (pull your live app into Figma canvas and edit with direct manipulation tools), and design → code (wrap your design system and push back to the codebase via an agent-generated PR with screenshots attached).

- *Canvas beats chat boxes for design thinking.* Current chat interfaces are too linear for creative work. On Figma's Infinite Canvas, divergent agents explore multiple directions simultaneously while convergent agents cluster and evaluate options — closer to how good design actually works.

- *Personalization is the unlock.* The gap between an okay agent and one people love is whether it understands your context. For Figma, that means your design system. Without it, the output isn't usable.

- *The next hard problem is reviewing, not generating.* Agents can produce faster than humans can evaluate. Building trust systems — evals, convergent review agents, consistency checks — is what Colyer sees dominating the next year.

On career advice for PMs and designers: the fundamentals still matter, and the most valuable people are the curious ones who push tools to their limits rather than just accepting the output. "You can't have been the one who's like, answer this problem for me. You have to be that curious person."

<https://www.youtube.com/watch?v=kYKebKB3-d0>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
