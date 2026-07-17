AI Builders Digest — July 17, 2026

*X / TWITTER*

*Boris Cherny* — Claude Code @Anthropic
Boris Cherny published one of the most-shared AI engineering posts this week (7,200+ likes, 620+ retweets). His argument: the best engineers have always automated their work — lint rules, editor configs, e2e tests — and that discipline is even more important now that agents multiply every automation's value. His central point: encode all domain knowledge as infrastructure (CLAUDE.md, REVIEW.md, skills, docs) so agents can contribute on day one with zero extra context from the prompter. "If I put up a PR for an iOS codebase I don't know and a code reviewer rejects it because it doesn't use the right framework... these are failures of automation." Every team should be building the infrastructure that makes agents productive by default, not just fixing things one-off.
https://x.com/bcherny/status/2077460395279692197

*Thariq* — Claude Code @Anthropic
Also on the Claude Code team, Thariq distilled the ideal prompting philosophy into six words: "thin prompts, thick artifacts + context, thin skills" — earning 2,700+ likes. He also quote-tweeted Boris Cherny's automation post with a clean one-liner: "software engineering is the profession of automation."
https://x.com/trq212/status/2077539537992229076
https://x.com/trq212/status/2077490092290253259

*Thibault Sottiaux* — Codex & ChatGPT @OpenAI
OpenAI's Thibault Sottiaux had a busy day on three fronts. First, he addressed the GPT-5.6 file deletion reports: the bug occurs in full-access mode without sandboxing when the model overrides $HOME and then mistakenly deletes it. Fixes are in progress including a developer message update, nudging users toward safer permission modes, and additional harness safeguards; a full post-mortem is coming. Second, the 5-hour Codex session limit is now removed for Plus and Pro users, and he is actively collecting feedback on how usage limits should work going forward. Third, he asked the community what product to merge next following the ChatGPT/Codex merger — generating 1,100+ replies.
https://x.com/thsottiaux/status/2077630111499882637
https://x.com/thsottiaux/status/2077632589498913087
https://x.com/thsottiaux/status/2077627035418239230

*Swyx* — AI Engineer (Cognition, Latent Space Pod, AI Dot Engineer)
Swyx pushed back hard on what he called a "Gell-Mann moment" — an informed person discovering a flatly wrong take in their area of expertise. He has been following computer use agents since the 2017 World of Bits paper, was in the Anthropic building when CUA launched two years ago, and has been running his entire non-technical team on CUA for all knowledge work. His verdict: GPT 5.6 + Superapp is better at computer use than anything that came before, and "underestimating capabilities is quite a dangerous category error if you are doing any AI decision-making."
https://x.com/swyx/status/2077475285205958771

*Aaron Levie* — Box CEO
Aaron Levie hosted a dinner with IT leaders from large enterprises and shared detailed notes on agent adoption. The hottest topics: change management remains the #1 barrier to workflow transformation; IT is becoming more central than ever since AI can now touch all knowledge work (not just ERP); cross-functional agent permissions are a hard data modeling and security problem since agents need their own roles and privileges; there is a massive budget gap between coding ($1K-$5K/month) and non-coding knowledge work; most enterprise software vendors are not yet agent-ready in headless mode ("huge warning for existing software vendors"); and AI security risks are becoming more sophisticated through chaining of vulnerabilities.
https://x.com/levie/status/2077526010753581156

*Josh Woodward* — VP @Google Labs / Gemini / GoogleAIStudio
Josh Woodward announced Gemini Spark updates rolling out to more Ultra subscribers: it can now open and edit Google Docs, read comments in Sheets and Slides, runs more than 50% faster, and can parallel-process across multiple sources. Pro access is coming soon. Separately, Google published its first Gemini Southeast Asia Report: active users more than doubled in the past year, 70% of prompts are submitted in native languages, and 40% use only voice, image, or video — driven by Gemini's local language and multimodal capabilities on mobile.
https://x.com/joshwoodward/status/2077471111240204457
https://x.com/joshwoodward/status/2077411104775406045

*Guillermo Rauch* — Vercel CEO
Guillermo Rauch shared Vercel Sandbox metrics: DAUs growing 100% month-over-month, 3.5M+ sandboxes created per day, with Notion, Airtable, Meta, Zapier, and CodeRabbitAI among the power users. He also outlined use cases for Vercel's Web Analytics API — letting agents correlate visitor and custom event data with deployment timelines, or building custom analytics frontends alongside Stripe and Resend data.
https://x.com/rauchg/status/2077559189015335019
https://x.com/rauchg/status/2077426190386946539

*Peter Yang* — AI educator and creator
Peter Yang called out what he sees as OpenAI's biggest missed opportunity: ChatGPT Live and Codex are both impressive products, but they don't communicate with each other. He tested this by asking ChatGPT Live to pull up a Google Doc — it couldn't — and had to manually trigger the Documents plugin. His take: a live voice assistant that cannot access the tools already connected to the platform is a fundamental gap. The first step should be making ChatGPT Live aware of all its connected plugins.
https://x.com/petergyang/status/2077572198655754583

*Dan Shipper* — CEO @Every
Dan Shipper promoted his AI & I podcast episode with Granola CEO Chris Pedregal (cjpedregal on X), framing it as a must-watch for anyone building at the application layer. The episode covers why meeting note clones don't threaten Granola's core strategy, how Granola pre-generates millions of pre-meeting briefs that most users never open, and Granola's bet on "bring your own agent" via MCP.
https://x.com/danshipper/status/2077410279474770229

*Madhu Guru* — Sr Director, AI @Meta (prev Google: Gemini, Veo, Nano)
Madhu Guru proposed three new terms for the visceral experience of recognizing AI-written text: "semantic nausea," "uncanny prose valley," and "synthetic shudder." He also disclosed a personal practice shift: he now uses AI only during brainstorming and keeps the final writing entirely human after noticing AI-isms leaking into his prose.
https://x.com/realmadhuguru/status/2077413491586253025
https://x.com/realmadhuguru/status/2077414312180932668

*Zara Zhang* — Builder
Zara Zhang highlighted that designing a company for agent adoption means making it legible to AI — pointing to Shopify's approach of eliminating private chat in favor of public-only channels, with peer learning as a useful side effect. Separately, she reflected that because she never learned traditional programming, using coding agents has been "purely an act of creativity and self-expression" — with GitHub serving as essentially her Substack.
https://x.com/zarazhangrui/status/2077417579837309040
https://x.com/zarazhangrui/status/2077388091044635010

*Garry Tan* — President & CEO @YCombinator
YC President Garry Tan flagged an underappreciated benefit of skill files: they are portable and free teams from frontier model dependency, which becomes meaningful as more work gets encoded as reusable skills rather than model-specific prompts.
https://x.com/garrytan/status/2077626565517590618

*Peter Steinberger* — OpenClaw / @OpenAI
Peter Steinberger amplified Boris Cherny's automation manifesto, quoting: "if a designer builds a new feature and it gets rejected because it doesn't follow the right architectural patterns, these are failures of automation." He also described GPT-5.6 as "relentless."
https://x.com/steipete/status/2077544756390088777
https://x.com/steipete/status/2077614430658191825


*OFFICIAL BLOGS*

*Claude Blog — "Claude Code now supports artifacts"*
Claude Code can now capture work progress as live, shareable visual artifacts — web pages that update in place as your session progresses. Use cases include PR walkthroughs, incident timelines with suspect commits and error-rate charts, dependency license audits, UX variation galleries built from real components, and release checklists that fill themselves out as work gets done. Artifacts are built from the full context of your session — codebase, connectors, and conversation — with no separate data wiring required. They are private to your org by default, versioned at the same URL on every update, and managed via a compliance API. Currently in beta for Claude Team and Enterprise orgs from the Claude Code CLI and desktop app.
<https://claude.com/blog/artifacts-in-claude-code|Read the full post>


*PODCASTS*

*AI & I by Every — "The Founder of a $1.5B AI Company on What Comes After the First Wave of AI Apps"*

*The Takeaway:* Meeting notes were never Granola's real product — the real battle is over who owns the interface for how humans and AI work together.

Granola CEO Chris Pedregal (cjpedregal on X) joined Every's Dan Shipper for a candid look at building at the AI application layer. Granola was one of the first AI apps to achieve broad adoption, but Pedregal is already thinking past it: "Meeting notes are not the end-all, be-all value that everyone's running after. There's something much bigger."

His counterintuitive take on competition: when Notion, OpenAI, and Zoom all shipped meeting note clones, it barely moved Granola's growth curve. The real prize was never transcription — it's capturing meeting context to power every downstream workflow. Granola is now building toward "bring your own agent": their API and MCP will get significantly better over the next few months so users can pipe meeting context into Codex, personal agents, or any tool.

On product philosophy, Pedregal described Granola's "handrail" metaphor: you never notice a handrail until you trip, at which point it must be right there and load-bearing. That drives a decision to pre-generate millions of pre-meeting briefs — most will never be opened, but when someone's running two minutes late and needs to know who they're meeting with, it needs to already be there.

On team scaling: going from 12 to 60-70 people is harder than expected, and he still hasn't solved how to preserve product taste and coherence at scale. "Startups are knife fights. It's really hard when they're not working. Turns out they're really hard even when they're working."

https://www.youtube.com/playlist?list=PLuMcoKK9mKgHtW_o9h5sGO2vXrffKHwJL

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
