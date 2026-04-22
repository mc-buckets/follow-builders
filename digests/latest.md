*AI Builders Digest — April 22, 2026*


*X / Twitter*

*Andrej Karpathy* — former Tesla AI Director, OpenAI founding team

Karpathy shared a detailed workflow for using LLMs to build personal knowledge bases. The system works by indexing raw documents (articles, papers, repos, images) into a directory, then having an LLM "compile" a wiki of .md files — complete with summaries, backlinks, and concept articles — viewable in Obsidian. Once the wiki grows large enough (~400K words in his case), he queries it with LLM agents for complex Q&A, outputs as rendered markdown, slides, or matplotlib images, and loops outputs back into the wiki. He also runs "health checks" to find inconsistencies, impute missing data, and surface new article candidates. His conclusion: "I think there is room here for an incredible new product instead of a hacky collection of scripts."
<https://x.com/karpathy/status/2039805659525644595|Full thread>

He followed up suggesting the natural extrapolation: every question to a frontier LLM could spawn a team of LLMs to construct an entire ephemeral wiki, lint it, loop a few times, then write a full report — well beyond a simple `.decode()`.
<https://x.com/karpathy/status/2039808711452246261|Tweet>


*Aaron Levie* — Box CEO

Levie shared the sharpest architectural lesson from building Box's AI agent: you must be "brutally unsentimental" about your own tech. As models improve, previously built scaffolding becomes redundant or actively harmful — you need to ruthlessly jettison it to unlock new performance gains. He described the cycle: build scaffolding → models improve, rendering it redundant → remove it → new capabilities emerge → repeat. In Box Agent specifically, components they designed into the original architecture had to be ripped out before launch because they were creating unnecessary constraints as models got better at reasoning, search, and context handling. "Always make sure you're taking advantage of the frontier capabilities and don't become nostalgic around the tech you've already built."
<https://x.com/levie/status/2039931799414194621|Tweet>


*Ryo Lu* — Design at Cursor

Ryo announced Cursor 3 — a redesign built around the idea that simplicity and power aren't opposites. It works across local and cloud projects, starts minimal, and reveals more tools as you need them.
<https://x.com/ryolu_/status/2039780768847958359|Tweet>

He also published a philosophy essay on "glass vs. black box." His argument: AI tools made the black box more addictive (you type a wish, pull a lever, accept or reject the whole thing), and you see less and think less as models got better. Cursor bets the other way — visible agents, editable plans, stoppable diffs, nothing hidden. "As AI gets more powerful, glass gets more important. Not because you need to watch every move. But because the best work happens when you know you can." His closing line: "Give away the wheel and you get mediocre. Keep it and you get to build something great."
<https://x.com/ryolu_/status/2039895634313187619|Full essay>


*Peter Steinberger* — AI builder, openclaw

Steinberger flagged a signal worth watching: Linux kernel security maintainers report that AI-generated bug reports have surged from 2-3 per week two years ago, to ~10 per week last year, to 5-10 per day now. Crucially, most of these reports are correct — meaning maintainers have had to bring in extra reviewers just to process the volume. His prediction: this sustained AI-driven load will kill some open-source projects that can't absorb the overhead.
<https://x.com/steipete/status/2039782190838686088|Tweet>


*Peter Yang* — Roblox product manager, 140K newsletter readers

Yang tried Cursor 3 and found the new interface a meaningful improvement — the old UI had too many buttons and toggles that got in the way of just talking to the agent. He thinks the simplified new view should just be the default.
<https://x.com/petergyang/status/2039850011044016291|Tweet>


*Amjad Masad* — Replit CEO

Masad announced three things: an SEO audit tool for your site built on Replit, a new no-setup enterprise-grade auth solution for everyone, and a new sales office opening in Salt Lake City, Utah.
<https://x.com/amasad/status/2039838798671126728|SEO audit tweet> • <https://x.com/amasad/status/2039774118443421887|Auth tweet> • <https://x.com/amasad/status/2039777772701413396|SLC office tweet>


*Dan Shipper* — Every CEO

Shipper's team spent a week testing Cursor 3.0 before launch and published their full vibe check on Every's publication.
<https://x.com/danshipper/status/2039770244361662920|Tweet>


*Sam Altman* — OpenAI CEO

Altman declared TBPN his favorite tech show and said OpenAI wants them to keep doing what they do well — including holding OpenAI accountable. He joked he'll keep supplying material with "occasional stupid decisions."
<https://x.com/sama/status/2039773740586918137|Tweet>


*Claude* — Anthropic AI

Computer use in Claude Cowork and Claude Code Desktop is now available on Windows.
<https://x.com/claudeai/status/2039836891508261106|Tweet>


*Swyx* — AI engineer, Latent Space podcast

Swyx reacted to news that TBPN is selling their podcast with a tongue-in-cheek question: "time for dario x dwarkesh?" He also posted what reads as a reaction to a major AI pricing drop, repeating "HOW LOW IS LOW / HOW LOW / IS LOW."
<https://x.com/swyx/status/2039773480980480431|TBPN tweet> • <https://x.com/swyx/status/2039812100206604787|Pricing tweet>


*Nan Yu* — Linear Head of Product

Nan posted a series of brief observations framing AI as a flexible collaborator — sometimes a PM, sometimes a product marketer — depending on what you need. He also floated a half-joke concept: TBPN for sports.
<https://x.com/thenanyu/status/2039832290490994970|Tweet> • <https://x.com/thenanyu/status/2039823494398001448|Tweet> • <https://x.com/thenanyu/status/2039820803722633589|Tweet>


*Podcasts*

*Training Data: "How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly"*

*The Takeaway:* Biology is finally getting its computing moment — and the lab bench is about to become as obsolete as the mainframe.

Jason Kelly co-founded Ginkgo Bioworks in 2008 with a simple premise: DNA is code, cells are programmable, and if you can engineer biology the way you engineer software, you unlock a massive market. He bootstrapped for six years (with government grants and service work) before doing YC in 2014 after Sam Altman wrote a blog post saying Silicon Valley's model could work for deep tech.

His core argument is refreshingly blunt: "All of the previous revolutions in tech — Internet, social media, whatever — have been totally meaningless to biotechnology and biopharma. It's just some back office IT crap. Not this. This is actually gonna change the fundamentals of how we do science."

The vehicle for that change is the autonomous lab. Instead of human scientists walking around underutilized bench equipment in million-square-foot campuses, Kelly envisions centralized, robot-run labs where experiments are ordered through a computer and executed on a high-precision track system. Utilization jumps from under 20% to around 70%, space requirements drop dramatically, and the physical constraint of "you need a lab wherever your scientists are" disappears. Ginkgo already sold 97 robots to the Department of Energy for what he calls the "Genesis mission."

The contrarian take: humanoid robots in labs are a bad idea. Biology is a microscopic discipline — purpose-built track systems beat bipedal walking robots every time.

His long-term vision is to democratize science the way computing was democratized. Ginkgo launched a Cloud Lab service where experiments start at $39 — you don't get a sample back, you get data. Kelly's bet is that if you drop the cost of running a real experiment low enough, millions of ordinary people will want to be scientists. "If you rewind the clock to the 1960s when it was IBM and mainframes and you told people that kids would program computers, they would say you're fucking insane. And so I believe if you do manage to drop the cost of all this stuff, you may have kids and everybody else wanting to just ask original scientific questions and being able to do it."

<https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8|Watch on YouTube>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
