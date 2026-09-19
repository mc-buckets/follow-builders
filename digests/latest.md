*AI Builders Digest — September 19, 2026*

*X / TWITTER*

*Claude Projects — The Big Launch of the Day*

Anthropic rolled out a sweeping overhaul of how Claude handles work. The new Projects experience gives Claude persistent memory across sessions, multi-threaded task management, and a shared file library — all coordinated by a single project-level agent.

*Boris Cherny (Claude Code @ Anthropic)* described how it changed his workflow: "I stopped managing sessions. I just send thoughts as they come, Claude splits them into threads, and the project remembers how I work. It's where I do a ton of my coding now." 2,352 likes — clearly resonating.
<https://x.com/bcherny/status/2100669598995816511|tweet 1> / <https://x.com/bcherny/status/2100639991244427490|tweet 2>

*Cat Wu (Claude Code + Cowork @ Anthropic)* on the workflow shift: "I fire off a batch of tasks and move on. Claude has context on everything I'm working on and can give me an aggregated status update whenever I ask. It also has long-lived memory that evolves as I use it."
<https://x.com/_catwu/status/2100641163120423057|tweet>

*Thariq (Claude Code @ Anthropic)* explained the architecture: Projects brings the structure of Claude Tag to Claude Code — one agent per project, manages memory, spins off subagents for tasks. You can ask it to be proactive or do things on a schedule.
<https://x.com/trq212/status/2100638355872706571|tweet>

The Claude account shared key details: project memory is shared across threads, a file library keeps what you add and what Claude creates, threads run in the cloud (offline-friendly), and local file/tool support is coming soon. Pro and Max plans are rolling out now.
<https://x.com/claudeai/status/2100632684074549309|tweet 1> / <https://x.com/claudeai/status/2100632687316730327|tweet 2> / <https://x.com/claudeai/status/2100632688625348890|tweet 3>

- - -

*Josh Woodward (VP, Google Labs / Gemini)*

Two product pushes from Google's AI arm. Google Labs launched *CC for Families* — an AI agent that syncs up to 5 family members via shared Google Calendar, Chat, and Tasks. It handles paperwork, maintains shared context (grocery lists, favorite restaurants) and individual context (dietary restrictions, timezones), and sends a "Your Day Ahead" brief each morning. Waitlist open for US users 18+.
<https://x.com/GoogleLabs/status/2100653821907366366|Google Labs tweet>

Woodward also flagged Gemini Notebook on mobile: "If you're not using Gemini_Notebook on your phone yet, you're missing out."
<https://x.com/joshwoodward/status/2100616682431807860|tweet>

- - -

*Guillermo Rauch (Vercel CEO)*

Three posts worth noting. On deployment scale: it took Vercel 10 years to hit 1 billion deployments, then added 1.4 billion more in the last 10 months alone — driven by AI-generated software including "tiny, personal and even disposable" artifacts. Vercel has now brought full global CDN deployment (with firewall, immutable deploys, domain assignment, observability) down to under 1 second.
<https://x.com/rauchg/status/2100698591417499972|tweet>

New feature: `vercel --turbo --prod` — a flag that uses the fastest available build machine when agents need to ship a hotfix fast.
<https://x.com/rauchg/status/2100682030170489160|tweet>

A wry aside: "Vercel is the Vercel for Java."
<https://x.com/rauchg/status/2100745015362552312|tweet>

- - -

*Aaron Levie (Box CEO)*

A sweeping prediction on the agent-first future: "Agents already make up the majority of inference. This will quickly trend toward nearly all inference over the next year or two." Levie sketches the scope — agents reading every code commit for security, processing data workflows, handling recruiting and customer research, reviewing every event stream and log, executing personal tasks 24/7. "Just in the past week I've introduced multiple completely new workflows that would not have been possible technically even a month ago."
<https://x.com/levie/status/2100799668573946191|tweet>

- - -

*Garry Tan (YC President & CEO)*

Flagged Memorable, a startup that optimizes AI memory using *embeddings* rather than burning more tokens — a more efficient path to persistent model context.
<https://x.com/garrytan/status/2100668489178456268|tweet>

Also sounded a warning on alignment: "Be careful what you wish for — this is why we need alignment to humankind vs any other goal."
<https://x.com/garrytan/status/2100636443127210112|tweet>

And an optimistic note: "The future is already here. We just have to choose it and spread it faster."
<https://x.com/garrytan/status/2100612808568172830|tweet>

- - -

*Nikunj Kothari (FPV Ventures partner)*

Shared a solo build: nosugarforkids.com — a healthy snack catalog for kids, powered by a Claude agent that wakes up daily to: check for new products, prune dead listings, find SEO content ideas, check Google Search Console, write and edit posts, and reach out for backlinks. Zero paid promotion, no backlinks at launch — still grown to ~6k impressions/day organically. An MCP (and WebMCP) is available so agents can query the catalog directly.
<https://x.com/nikunj/status/2100714665571737885|tweet> / <https://x.com/nikunj/status/2100718806004064730|tweet with MCP link>

- - -

*Thibault Sottiaux (Codex & ChatGPT @ OpenAI)*

An intriguing prompt from the OpenAI side: "Has anyone yet tried to get Astra and Fable to agree on the perfect styleguide? And then host it somewhere with a web MCP?" The tweet (5,500+ likes, 1,800 replies) landed as a compelling experiment idea — get competing AI agents from different labs to collaborate on shared standards, then serve the result via a web MCP.
<https://x.com/thsottiaux/status/2100645454245720513|tweet>

- - -

*Aditya Agarwal (SPC General Partner)*

Highlighted GoodfireAI as "the leading non-frontier-lab company working on alignment and safety," calling the work "generationally important."
<https://x.com/adityaag/status/2100746235426836708|tweet>

- - -

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
