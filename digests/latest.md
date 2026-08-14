*AI Builders Digest — August 14, 2026*

*X / TWITTER*

*Swyx* (swyx on X) — AI researcher affiliated with smol.ai, AI Engineer, and Latent Space Pod
Called a recent paper "already one of the most important papers of this year," sharing notes with a further distillation of the methodology. Also marked the one-year anniversary of Perplexity's offer to buy Chrome with a scheduled throwback tweet.
- https://x.com/swyx/status/2087437017840046156
- https://x.com/swyx/status/2087691099691475285

*Josh Woodward* (joshwoodward on X) — VP at Google Labs, Gemini App, and Google AI Studio
Announced a new wave of Gemini integrations rolling out today: Angi, Fever, GetYourGuide, Granola, iHeartRadio, Localiza, OpenTable, Otter, Pandora, Thumbtack, Ticketmaster, Wix, Zocdoc, and Zoho. Invited partners to DM him.
- https://x.com/joshwoodward/status/2087751559606407615

*Thibault Sottiaux* (thsottiaux on X) — Codex & ChatGPT at OpenAI
Two notable signals: crossed the 15M milestone and announced a usage limit reset landing "in the next hour" with a nudge to use `/fast`. Also dropped a one-liner that got traction: "Also don't say Linux, we just shipped that" — implying Codex just added Linux support.
- https://x.com/thsottiaux/status/2087706104814023111
- https://x.com/thsottiaux/status/2087439859493617908

*Peter Yang* (petergyang on X) — AI tutorials and interviews creator
Shared a new free essay arguing the way we use computers is about to change fundamentally: voice becomes the orchestration layer, personal computing moves to the cloud, and trust becomes the key differentiator between AI products. Worth a read for anyone thinking about the next UI paradigm.
- https://x.com/petergyang/status/2087547168764862495

*Madhu Guru* (realmadhuguru on X) — Sr. Director of AI at Meta, formerly led Gemini, Veo, and Nano at Google
Made a sharp prediction: the biggest alpha in AI products over the next few years is in the application layer, not model infrastructure. Models will keep getting cheaper and more local, so differentiation will come from deeply understanding user workflows and redesigning experiences around them. "The denominator of people who can build AI products is about to get enormous. So being in the top 0.1% of builders will matter more than ever."
- https://x.com/realmadhuguru/status/2087553833098723547

*Amanda Askell* (AmandaAskell on X) — Philosopher and ethicist at Anthropic
Light day — two gaming-adjacent posts: one on the ethical bar in Bioshock (not murdering children), and one on playing Skyrim as "that challenging fantasy philanthropy game" by focusing on adopting orphans and skipping the plot.
- https://x.com/AmandaAskell/status/2087606022961865148
- https://x.com/AmandaAskell/status/2087597131800674495

*Guillermo Rauch* (rauchg on X) — Vercel CEO
Shared that the Vercel Sandbox (`npx sandbox@latest sh`) now ships with a reasonable default set of pre-installed tools and full customization — calling it "faster than your local machine." Also highlighted Seedance 2.5 running on the Vercel AI Gateway. Capped with his current mood: "Endless opportunity everywhere you look."
- https://x.com/rauchg/status/2087698195120116064
- https://x.com/rauchg/status/2087631388359242050
- https://x.com/rauchg/status/2087736311885218160

*Aaron Levie* (levie on X) — Box CEO
Enthusiastic take on new Deepseek and Grok releases: "huge jumps in capability at insanely low costs." Framed it as Jevons paradox for AI — cheaper compute unlocks entirely new enterprise use cases (security code scans, document review, workflow automation) that couldn't previously be budgeted. Bullish on the applied AI layer that routes and optimizes across models.
- https://x.com/levie/status/2087719356763672917

*Garry Tan* (garrytan on X) — President & CEO of Y Combinator
Launched GBrain v0.45.6.0 with 17 new brain skills hardened through his personal OpenClaw agent across hundreds of thousands of markdown files. Clarified the intended use: GBrain should run as a _separate_ agent alongside Codex or Claude Code, not inside your main coding agent — think of it as a personal AI with its own git repo for memory and custom skills. Now works with both Codex and Claude Code.
- https://x.com/garrytan/status/2087594114372259890
- https://x.com/garrytan/status/2087597829065945249

*Matt Turck* (mattturck on X) — VC at FirstMark Capital, MAD Podcast host
Offered a dry summary of AI engineering's evolving vocabulary: "Graph engineering is the new loop engineering which is the new harness engineering which is the new context engineering which is the new prompt engineering." A useful (and funny) reminder that the underlying challenge stays the same even as the terminology cycles.
- https://x.com/mattturck/status/2087528600849252696

*Zara Zhang* (zarazhangrui on X) — Builder, Harvard '17
Flagged a Stanford lecture series as "pure gold" — calling out that such high-quality knowledge is freely available on YouTube.
- https://x.com/zarazhangrui/status/2087547174662136273

*Peter Steinberger* (steipete on X) — Co-founder of OpenClaw, working with OpenAI
Made a sharp observation on the arc of AI coding tools: "CLI was a year ago. Apps maybe 6 months. Now it's services, web, cloud sessions." Captures how quickly the paradigm is shifting from local tooling to cloud-native agent infrastructure.
- https://x.com/steipete/status/2087568620465607078

*Dan Shipper* (danshipper on X) — CEO at Every
In a playful riff on a colleague's single-word posting strategy, announced a fake content agency "One Word" — and then said they're rebranding to "Word" because it's cleaner. Teased "something analog dropping tomorrow."
- https://x.com/danshipper/status/2087555423893065872
- https://x.com/danshipper/status/2087678775517442399

*Aditya Agarwal* (adityaag on X) — General Partner at SPC, former CTO of Dropbox
Shared that SPC India is the fund's first bet outside the US — and expressed conviction that "some of the most ambitious projects of the decade will be built there." Linked to an ETtech interview.
- https://x.com/adityaag/status/2087563716350902530

*Claude* (claudeai on X) — Anthropic's official AI account
Three product updates: (1) Claude in Chrome sessions now carry over to desktop, web, and mobile — conversations saved, skills and connectors work in the browser. Available on Max and Team now, rolling out to Pro soon. (2) The side panel runs the same Cowork session as all other Claude surfaces — sessions live with your account, not on a single device. (3) A reminder that browser agents can be tricked by prompt injection hidden in pages, with tips for staying safe.
- https://x.com/claudeai/status/2087635262390026525
- https://x.com/claudeai/status/2087635263774232617
- https://x.com/claudeai/status/2087635265066004694


*OFFICIAL BLOGS*

*Anthropic Engineering: An update on recent Claude Code quality reports*
<https://www.anthropic.com/engineering/april-23-postmortem|Read the post>

A thorough postmortem on three separate bugs that caused the degradation reports over the past month — none of which affected the API. First: in March, the default reasoning effort for Claude Code was quietly downgraded from high to medium to reduce latency, which hurt intelligence. Reverted April 7. Second: a caching optimization introduced March 26 had a bug that dropped prior reasoning context on every turn after a session went idle — making Claude seem forgetful and causing unexpected usage limit drain. Fixed April 10. Third: a system prompt change on April 16 capped response length (≤25 words between tool calls, ≤100 words for final responses), which hurt coding quality and was reverted April 20. Because each bug hit a different slice of traffic on a different schedule, the aggregate looked like broad, inconsistent degradation. Anthropic is resetting usage limits for all subscribers today, tightening controls on system prompt changes, and expanding the eval suite. They're also launching @ClaudeDevs on X for more transparent product communication.

*Anthropic Engineering: Scaling Managed Agents — Decoupling the brain from the hands*
<https://www.anthropic.com/engineering/managed-agents|Read the post>

A deep technical post on how Anthropic rearchitected Managed Agents by separating Claude (the "brain") from execution environments (the "hands") and durable session logs. The old coupled-container design was fragile — a container failure meant losing session state, and debugging required engineers to open shells inside containers that also held user data. The fix: the harness now calls sandboxes the same way it calls any tool (`execute(name, input) → string`), so containers are cattle, not pets. If one dies, a new one is provisioned. The session log lives outside both, so a crashed harness can be rebooted and resume from the last event. Payoffs: p50 time-to-first-token dropped ~60%, p95 dropped over 90%. Security also improved — credentials are never reachable from the sandbox where generated code runs.

*Claude Blog: New in Claude Managed Agents — self-hosted sandboxes and MCP tunnels*
<https://claude.com/blog/claude-managed-agents-updates|Read the post>

Two new capabilities for Claude Managed Agents now in public beta/research preview. Self-hosted sandboxes let a Claude agent execute tools on infrastructure you control — code execution, files, and services stay within your enterprise perimeter. Supported providers include Cloudflare, Daytona, Modal, and Vercel. MCP tunnels let Managed Agents connect to private MCP servers inside your network without exposing them to the public internet — a lightweight gateway makes a single outbound connection, no inbound firewall rules, traffic encrypted end to end. Both are managed from the Claude Console.


*PODCASTS*

*AI & I by Every: "Microsoft's Vision for an Internet Made for Agents With CTO Kevin Scott"*
<https://www.youtube.com/playlist?list=PLuMcoKK9mKgHtW_o9h5sGO2vXrffKHwJL|Watch the episode>

_The Takeaway:_ The bottleneck for AI isn't model capability anymore — it's the ecosystem plumbing needed for agents to actually act in the world.

Microsoft CTO Kevin Scott has been programming for 41 years and is also a woodworker and ceramic maker — someone who cares deeply about craft. His view on agents-for-coding: the craft debate ("are you a real programmer if you use AI?") is just the latest version of "are you a real woodworker if you use power tools?" His advice: be curious, try things, use what works.

On the bigger picture, Scott argues the AI industry is entering a "capability overhang" — models are now more capable than the products built on top of them. The urgent work is closing that gap, not scaling further. The agentic web is the answer: open protocols like MCP serve the same role for agents that HTTP does for the internet. NL Web is doing what HTML did. Scott says Microsoft is pushing internally for all its systems to speak a standard agent protocol to avoid "shipping the org chart" through Conway's Law.

On security: he doesn't claim to know the right model, but argues agents need identities so entitlement systems can say "this agent is acting on behalf of this person." The rest, he believes, is relatively straightforward to build on top of MCP.

His prediction for next year: the shift from synchronous to asynchronous agent interaction — instead of waiting for a response, you hand off a task and the agent iterates on its own before surfacing a result. *"Be curious. Try. And if it works for you, use it. And if it doesn't, don't."*


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
