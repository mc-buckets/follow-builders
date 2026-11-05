AI Builders Digest — November 5, 2026

*X / TWITTER*

*Cat Wu (claude code + cowork at Anthropic)*
Cat Wu announced her departure from Anthropic after two years, marking a milestone in Claude Code's evolution. In a heartfelt farewell, she described joining the team after using an early internal version to build an RL environment without writing a single line of code herself. Her post captures how much has changed: "When we first launched, most people approved every permission prompt by hand and mostly used Claude to answer questions and write tests. Today, the default is trusting Claude's judgment to auto-approve." She thanked the Claude Code, Cowork, and Tag teams and the user community whose feedback shaped so much of what shipped.
https://x.com/_catwu/status/2117731934340337676

*Thariq (formerly Claude Code at Anthropic)*
Thariq, also recently departed from Anthropic, amplified a point about AI scaling laws with a sharp take: the bitter lesson is at work again. Smarter models will need fewer and fewer tokens — they won't need to verify their work or check for bugs, they'll just be right.
https://x.com/trq212/status/2117670540148347273

*Boris Cherny (Claude at Anthropic)*
Boris Cherny announced a quality-of-life improvement for Claude Enterprise: auto-connect for plugins. Team and Enterprise admins can now configure plugins once, and teammates are connected automatically the first time they use them — no more signing in one by one.
https://x.com/bcherny/status/2117693181651542387

*Sam Altman (CEO at OpenAI)*
Sam Altman posted a pointed statement on AI governance: people should always be in control of the future. OpenAI opposes any scenario where humans are relegated to roles that "AI systems think makes sense to reward." His framing: human control over the future should ultimately constrain AI progress, even as capabilities advance.
https://x.com/sama/status/2117794005165748448

*Thibault Sottiaux (Codex & ChatGPT at OpenAI)*
Thibault Sottiaux reflected on the current state of agents with a candid take: "Things will change again and again and again. We're still very early and agents today are incredible, and yet so frustrating still." He's looking forward to cracking the flow state problem but acknowledges the long road ahead.
https://x.com/thsottiaux/status/2117746467058405665

*Aaron Levie (CEO at Box)*
Aaron Levie made a sharp observation about widening AI output divergence. Two years ago, the best productivity gains were 30–50% for highly capable users; now the ceiling has jumped to 5–10x depending on the field. He attributes this to longer agentic task windows, reduced need for human intervention, and better multi-agent support. His conclusion: the gap between frontier adopters and those not paying attention is becoming an order of magnitude — and recursive self-improvement will only widen it further.
https://x.com/levie/status/2117505799937577263

*Guillermo Rauch (CEO at Vercel)*
Guillermo Rauch shared three notable items this week. The biggest: Vercel is launching a Security Review product powered by an internal agent they call "@hacker" that audits every line of code automatically — and he says it catches things other agents miss. He positioned it as a way to "download a security team as software." He also highlighted a new `vercel doctor` CLI subcommand (recommending others ship doctor subcommands in their own CLIs), and pointed to new Vercel CI and Security Review capabilities.
https://x.com/rauchg/status/2117734833824948373
https://x.com/rauchg/status/2117802827519250568
https://x.com/rauchg/status/2117765475010822497

*Swyx (AI Engineer, smol.ai / Cognition / Temporal)*
Swyx announced the final track theme for the upcoming AI Engineer conference: "Raising Your Ambition," featuring speakers including jxnlco, Jarred Sumner, Mitsuhiko, and a keynote from someone who recently cloned the entire Adobe suite. The event gathers 1,000 agentic engineers in-person in SF and streams to 2M monthly viewers online. He also highlighted a talk from Addy Osmani on how Anthropic ships 30,000 code changes a day using a "dark factory" approach, with independent verification at every loop — calling it one of the top talks at AIE NYC.
https://x.com/swyx/status/2117679157035602065
https://x.com/swyx/status/2117558305891746212

*Peter Yang (AI educator and content creator)*
Peter Yang observed a shifting norm in AI: very talented people are leaving AI-native companies after 1–2 years, far shorter than the traditional 2–3 year tenure expectation. He also covered Grok's new phone call feature, walking through five practical use cases — negotiating bills, canceling subscriptions, waiting on hold, making reservations, and gathering contractor quotes — noting it currently works with US numbers only.
https://x.com/petergyang/status/2117825980115067035
https://x.com/petergyang/status/2117783921748558185

*Amjad Masad (CEO at Replit)*
Amjad Masad pointed to what he sees as a chaotic but defining phase: enterprise adoption of agents and vibe coding is messy right now, but that's how every major platform shift looks at inflection points.
https://x.com/amasad/status/2117761721750475146

*Nikunj Kothari (Partner at FPV Ventures)*
Nikunj Kothari shared two underused Claude Code default skills worth trying: `/insights` (he runs it on a biweekly cron job paired with X bookmarks to continuously upgrade his AI dev setup) and `/playground` (which he uses to visualize workflow architecture, run learning loops, and find dead code and latency improvements — especially when pairing Codex and Claude Code together). He also reflected on living in a golden moment: he's reaching for Claude desktop, ChatGPT Codex, Grok Bot, and Muse regularly, each pushing the frontier in their own way.
https://x.com/nikunj/status/2117773647868018897
https://x.com/nikunj/status/2117650163066183769

*Matt Turck (VC at FirstMark Capital)*
Matt Turck spotlighted SurrealDB 4, calling it a major milestone for a database that's survived the unglamorous years of open-source grind. The new version is multi-model (vector, graph, document), ACID-compliant, with a rebuilt engine, native Postgres/MySQL support, and massive scalability via Cloudflare handling 10B+ peak rows/second.
https://x.com/mattturck/status/2117741948609949932

*Google Labs*
Google Labs announced Dreambeans — their AI-powered dream journaling or exploration tool — is rolling out to users in India, with more regions to follow.
https://x.com/GoogleLabs/status/2117689420744991161

*Garry Tan (CEO at Y Combinator)*
Garry Tan mourned the shuttering of Popular Mechanics, a cultural loss for science and engineering journalism.
https://x.com/garrytan/status/2117721182049046735

*PODCASTS*

*Unsupervised Learning — Ep 96: Nebius CTO on Racing the Hyperscalers Before AWS Wakes Up*

_The Takeaway:_ The real bottleneck in AI infrastructure isn't GPUs, power, or talent — it's execution ability, and the companies winning are the ones who can navigate every constraint at once.

Nebius CTO Danila (the company spun out of Yandex's international assets in 2024) makes a compelling case that the AI cloud market is fundamentally a software story, not a hardware one. When Nebius launched, their hardware team was 40–50 people; software was already 200. That ratio was intentional.

On why hyperscalers didn't dominate early: "If NVIDIA could have produced 10x the chips, this whole market would have been shaped differently." AWS and Google faced a chip allocation squeeze — most went to internal training needs, leaving little for the broader market. Worse, retrofitting decades of legacy cloud infrastructure for GPU workloads requires massive investment that's hard to justify when the AI cloud revenue is still a rounding error on their total revenue. That window gave independents like Nebius room to grow.

The most surprising insight: storage became a bigger bottleneck than expected. Customers routinely pull 500–700 GB/sec from a single shared file system — numbers that would have been unimaginable four years ago. "I underestimated the scale that a single client operates at nowadays. 30 megawatts used to be a serious data center. Now it's sometimes not enough for a single client."

On AI coding and agent adoption inside Nebius itself, he's notably conservative: "Whatever you've done with the agent, it's still your result. It's your responsibility. It's your pull request. It's you who is on call." Fully autonomous agents don't touch core services — yet.

His forward bet: the next wave of optimization isn't about bigger models, it's about outcome reliability in agentic workflows. He's watching how companies tune the harnesses, tools, and orchestration layers around models — not the models themselves.

https://www.youtube.com/@RedpointAI

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
