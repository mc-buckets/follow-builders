*AI Builders Digest — April 13, 2026*


*X / TWITTER*

*Andrej Karpathy* (former Director of AI at Tesla, founding team at OpenAI)

Karpathy shared a detailed breakdown of how he's using LLMs to build personal knowledge bases — raw documents get ingested into a directory, an LLM "compiles" them into an interconnected Markdown wiki, and then further LLM agents run Q&A and health checks over the whole thing. He uses Obsidian as the frontend and vibe-coded a small search engine to hand off to the LLM as a tool. His conclusion: "I think there is room here for an incredible new product instead of a hacky collection of scripts." He followed up noting that the natural next step is spawning entire ephemeral teams of LLMs to build a full wiki, lint it, and produce a report — going way beyond a simple text decode.

- https://x.com/karpathy/status/2039805659525644595
- https://x.com/karpathy/status/2039808711452246261

*Aaron Levie* (CEO, Box)

Levie posted a sharp lesson from building Box Agent: be brutally unsentimental about your architecture. As models improve, the scaffolding you built to compensate for earlier limitations becomes a drag on performance — and you have to ruthlessly tear it out. The loop: build scaffolding → models improve and make it redundant → remove scaffolding → new harder problems emerge → repeat. "Always make sure you're taking advantage of the frontier capabilities and don't become nostalgic around the tech you've already built."

- https://x.com/levie/status/2039931799414194621

*Ryo Lu* (Design, Cursor)

Lu wrote a manifesto on Cursor's design philosophy around what he calls "glass" — making AI tools transparent and inspectable rather than a black box. His argument: as AI gets more capable, giving users full visibility into agents, diffs, and state becomes _more_ important, not less. "Give away the wheel and you get mediocre. Keep it and you get to build something great." He also announced Cursor 3, which launches with a simpler interface that unfolds more tools as needed, works across local and cloud projects.

- https://x.com/ryolu_/status/2039895634313187619
- https://x.com/ryolu_/status/2039780768847958359

*Peter Yang* (Product at Roblox, newsletter author)

Yang tried out Cursor 3 and likes the cleaner interface — the old version had too many buttons and toggles cluttering the experience. He thinks the new agent-first view should just be the default. He also posted a practical thread of hard-won tips for surviving Disneyland with kids: get early access, sprint to the most popular ride, buy premier passes for the next two, nap at the hotel during peak hours, and head back to the park at 5pm when lines thin out.

- https://x.com/petergyang/status/2039850011044016291
- https://x.com/petergyang/status/2039898958814974021

*Amjad Masad* (CEO, Replit)

Masad shared that Replit is opening a sales office in Salt Lake City, Utah and encouraged locals to consider joining the team. He also highlighted a no-setup enterprise-grade auth solution and amplified an agent that can SEO-audit your site.

- https://x.com/amasad/status/2039777772701413396
- https://x.com/amasad/status/2039774118443421887
- https://x.com/amasad/status/2039838798671126728

*Sam Altman* (CEO, OpenAI)

Altman gave a shoutout to TBPN, calling it his favorite tech show. OpenAI appears to have acquired or backed the podcast. "I don't expect them to go any easier on us, am sure I'll do my part to help enable that with occasional stupid decisions." The post drew 5,000+ likes.

- https://x.com/sama/status/2039773740586918137

*Garry Tan* (President & CEO, Y Combinator)

Tan flagged Perplexity Computer as "quite special actually" — a short but pointed endorsement. Also reposted a quote on loving your work.

- https://x.com/garrytan/status/2039943351278190840
- https://x.com/garrytan/status/2039948180977316164

*Peter Steinberger* (co-founder, OpenClaw)

Steinberger flagged a concerning data point for open source maintainers: the Linux kernel security list has gone from 2-3 vulnerability reports per week two years ago, to 10 per week last year, to now 5-10 _per day_ — with AI-generated reports being the sole driver. He predicts this pace could kill some OSS projects. He also reacted with humor to a post asking whether AI-generated content counts as "hot people or slop cannon."

- https://x.com/steipete/status/2039782190838686088
- https://x.com/steipete/status/2039948914112209390

*Dan Shipper* (CEO, Every)

Shipper shared that Every has been beta-testing Cursor 3.0 for a week and published a full vibe check. He also posted two brief reactions to things shipping at Every, expressing genuine excitement as the product icons fill in.

- https://x.com/danshipper/status/2039770244361662920
- https://x.com/danshipper/status/2039876581015933226
- https://x.com/danshipper/status/2039855704714985969

*Claude / Anthropic*

Computer use in Claude for Work and Claude Code Desktop is now available on Windows.

- https://x.com/claudeai/status/2039836891508261106

*Nan Yu* (Head of Product, Linear)

Yu posted a series of brief quote tweets riffing on the idea that AI can flex into different roles — PM, product marketer, collaborator — depending on what you need. He also half-jokingly proposed "TBPN for sports."

- https://x.com/thenanyu/status/2039832290490994970
- https://x.com/thenanyu/status/2039823494398001448
- https://x.com/thenanyu/status/2039820803722633589


*PODCASTS*

*Training Data — "How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly"*

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8

_The Takeaway:_ AI reasoning models paired with robotic labs can already beat human scientists at experimental design — not because they're smarter, but because they never sleep, share data in real time, and cost a fraction as much to run.

Jason Kelly founded Ginkgo Bioworks in 2008 straight out of grad school with no funding and a singular goal: make biology programmable. He bootstrapped for six years before Y Combinator (Sam Altman personally recruited him) unlocked their first real capital. Today Ginkgo operates what Kelly calls an "autonomous lab" — a robotic facility where AI agents design and run wet-lab experiments end to end, without a human touching the bench.

The proof point: Ginkgo and OpenAI ran a reasoning model against a classic biochemistry optimization problem (cell-free protein synthesis). Over four rounds of 30,000 experiments each, the model beat the Stanford-published state of the art. After six rounds, it beat it by *40%*. Kelly's explanation: "What really let it break through wasn't that it was so smart. It was that it could run experiments."

His broader argument is structural, not hype. Science today is brutally inefficient — labs run at low equipment utilization five days a week, every lab duplicates the same equipment, and researchers share conclusions once a year via published papers rather than sharing raw data daily. Kelly's vision: 100 AI scientists running in parallel on the same autonomous lab, each pursuing a different hypothesis, pooling raw experimental data _every day_, and publishing a weekly lab notebook. Right now, less than 5% of research budgets go to actual reagents (the real cost of doing experiments); the rest is overhead. Flip that ratio and you get 10x more data per dollar — without the AI even needing to be smarter than the scientists.

"All of the previous revolutions in tech — Internet, social media, whatever — have been totally meaningless to biotechnology and biopharma. Not this. This is actually gonna change the fundamentals of how we do science."

Kelly is candid that scientists will push back on creativity claims. His response: creativity isn't the point. The advantage is scale, speed, and frictionless information sharing — things that are simply socially and organizationally impossible for humans working in separate labs under separate budgets.


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
