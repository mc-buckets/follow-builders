*AI Builders Digest — August 4, 2026*


*X / TWITTER*

*Andrej Karpathy* (karpathy on X) — AI researcher who trains large deep neural nets

Karpathy shared more on the "pelican on a bicycle" test from Simon Willison, uploading a playable browser version of the source. He also tossed in a GTA Hobbiton joke: "Look out for GTA Hobbiton dropping before GTA VI."
<https://x.com/karpathy/status/2083948654377996480|View tweet>


*Swyx* — co-founder of smol.ai, AI Engineer podcast host

Swyx is collecting "computer use wow moments" for an upcoming podcast on the topic. His latest: Codex's computer use agent handled a support chat escalation entirely on its own — the support rep had no idea they were talking to a bot, tried to blame Swyx's team, and the bot fired back with complete receipts. The humans never caught on.
<https://x.com/swyx/status/2084156733027701164|View tweet>


*Peter Yang* — creator of practical AI tutorials

Peter Yang highlighted how Hermes (from NousResearch) avoids building up "slop" in its memory and skills: a background task called Hermes Curator runs on a schedule, auditing and rewriting its own cleanup logic based on your custom definition of slop. Because it's open source, you can hand it your own definition and it rewrites the cleanup loop your way. He also noted: a smart but annoying AI friend isn't useful — personality matters as much as capability.
<https://x.com/petergyang/status/2083968605432267139|Hermes Curator tweet>
<https://x.com/petergyang/status/2083947480136421384|AI personality tweet>


*Thariq* — Claude Code at Anthropic

Thariq invoked Jevons paradox to push back on fears that AI makes math expertise less valuable: more is happening in math, it's easier to follow at higher abstraction levels, and demand for people who deeply understand it will go up, not down. He sees strong parallels to what happened with chess after engines arrived.
<https://x.com/trq212/status/2083977795290734975|Jevons paradox in math>
<https://x.com/trq212/status/2083978109376987365|Chess parallels tweet>


*Amjad Masad* — CEO of Replit

Masad's LLM chess engine is now live on Lichess, autonomously playing real games against humans and bots — currently sitting at 1253 Elo. You can watch it play live; he caught it running 3 concurrent games at once.
<https://x.com/amasad/status/2083926395403821427|View tweet>
<https://x.com/amasad/status/2083936067355635948|Live games tweet>


*Guillermo Rauch* — CEO of Vercel

Rauch shared that Vercel built an internal AI agent called @v (the basis for their product evedev_) that now powers all of their internal operations — finance, comms, docs, marketing, engineering, analytics. It's growing exponentially in daily interactions and token use, maintains per-user memories and schedules, and routes to sub-agents as needed. His analogy: it's a "monolith" for agents, like having one company.com instead of dozens of competing agent subdomains. His take on ownership: if agents become synonymous with modern companies, controlling your own agent — source, runtime, data, and tokens — is a big deal.

He also posted a sharp reminder: _"AI alone is cool. But mastery + creativity + AI hits on a whole different level. Don't let anyone discourage you from pursuing excellence and craft. Keep studying the blade."_
<https://x.com/rauchg/status/2084042561690456157|@v internal agent thread>
<https://x.com/rauchg/status/2084060157085143512|Agent router architecture>
<https://x.com/rauchg/status/2083969120270450911|Mastery + AI tweet>


*Aaron Levie* — CEO of Box

Levie made a counterintuitive prediction: the "hardest" work — math, cybersecurity, code — is most prone to automation _first_, precisely because it's verifiable. You can test whether the output is correct, which both sharpens training signals and enables reliable deployment. Softer domains (legal, sales, marketing, finance) are harder to automate because there's no single right answer, the context keeps changing, and you often can't even know if the AI got it right until much later. His conclusion: applied AI tooling will matter as much as model capability in those domains, and the processes themselves will need to evolve.
<https://x.com/levie/status/2083965372747882741|View tweet>


*Ryo Lu* — Designer at Cursor

Ryo Lu is thinking about what comes after apps. He credits Rdio, Mailbox, and Apple as early mentors that showed how software could feel intuitive to touch, and wonders: as we leave the world of apps behind, what parts of software remain visible and how will they feel?
<https://x.com/ryolu_/status/2083939454017053179|View tweet>


*Garry Tan* — President & CEO of Y Combinator

Tan made three observations. AI will create unimaginable economic growth and that's the best reason for optimism. He also noted a cultural irony: our sense of wonder has faded right as the rate of actual wonder is going parabolic. And a market philosophy note: meritocracy means the territory (did you make something people want?) matters more than the map (titles, credentials, narratives).
<https://x.com/garrytan/status/2083957110711386439|Growth is good>
<https://x.com/garrytan/status/2083923385193828612|Sense of wonder tweet>
<https://x.com/garrytan/status/2083920039208693996|Territory vs map tweet>


*Nikunj Kothari* — Partner at FPV Ventures

Kothari posted a clear-eyed read on the current VC market: early-to-mid stage funding has become fully "vibes capital," completely disconnected from fundamentals. Some companies with nothing to show are raising massive rounds; solid ones are struggling. He thinks it continues for 12-18 months given dry powder and the AI tailwind. Public markets are equally wild — even trillion-dollar stocks swing 5%+ on vibes and model releases. His advice: understand what's happening before you enter capital markets. In the long run, building a profitable company with a clean cap table still works.
<https://x.com/nikunj/status/2083873335998333227|View tweet>


*Dan Shipper* — CEO of Every

Shipper wrote a detailed theory on how people metabolize AI capability jumps through "agency ruptures." The cycle: (1) _Initial rupture_ — you see the AI doing what you used to do and only see the AI; (2) _Seeing human scaffolding_ — you start to notice the work required to get the model to perform reliably; (3) _Agency reconstruction_ — the scaffolding becomes the interesting work, the model becomes invisible, and you say "I did this" not "AI did this." His hypothesis: the ability to metabolize these ruptures and turn them into curiosity is a strong predictor of who thrives in the AI economy. Each capability jump triggers new ruptures, even in fields like mathematics that haven't been touched until now.

He also offered a philosophical aside: if technology reshapes what humans _can_ do, it necessarily reshapes what we _ought_ to do — AI will change our moral intuitions alongside our abilities.
<https://x.com/danshipper/status/2084038453831020916|Agency ruptures thread>
<https://x.com/danshipper/status/2084024211539116466|Technology reshapes oughts>


*PODCASTS*

*Training Data: "Building the Automated AGI Lab: Core Automation's Jerry Tworek and Rohan Anil"*

_The Takeaway:_ The transformer architecture itself — not scale, not RL — is the core bottleneck standing between today's AI and genuine AGI, and two of the most experienced model builders in the industry just left their frontier labs to fix it.

Jerry Tworek (former VP at OpenAI who ran the strawberry and reasoning teams) and Rohan Anil (one of four Gemini pre-training leads, shampoo optimizer creator at Google Brain, former Anthropic researcher) founded Core Automation with one bet: transformers can't do continual learning, and that's a structural problem no amount of RL or scaling will solve.

Jerry's argument: the real bottleneck isn't capability — models are trained in the lab and deployed in a changing world, and transformers can't adapt. In-context learning is too short-horizon; fine-tuning causes catastrophic forgetting. Neither scales to real-world distribution shift. His definition of AGI: _"A model that can improve itself without human in the loop in any way."_ By that measure, we're not close.

Rohan's framing is computational: transformers are shallow (at most ~100 layers), and chain-of-thought token generation is an expensive band-aid for insufficient architectural depth — you're spending enormous compute one token at a time to get one bit of information into the network. He sees combining pre-training and RL end-to-end, rather than sequentially, as a clear order-of-magnitude opportunity.

Core Automation's near-term plan is to automate kernel generation — getting from a novel architectural idea to a GPU-optimized implementation as fast as possible. Proof of how hard this is: a QR kernel competition they hosted yielded a solution 60x faster than off-the-shelf solvers, but required three experts spending $100,000 on coding agents over four weeks to get there. Current frontier models couldn't get close. That's the gap they want to close. Their long-term goal: go on vacation as a team and have the lab produce better research while they're gone.

https://www.youtube.com/watch?v=2RJiaf0SY8s


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
