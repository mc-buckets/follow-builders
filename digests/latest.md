AI Builders Digest — April 4, 2026

*X / TWITTER*

*Andrej Karpathy* (AI researcher, formerly Director of AI at Tesla and founding team at OpenAI)

Karpathy dropped one of his most detailed posts in a while: a full breakdown of how he uses LLMs to build personal knowledge bases. The workflow: ingest raw source material (articles, papers, repos, images) into a directory, have an LLM "compile" a wiki of interconnected .md files — summaries, backlinks, concept articles. He uses Obsidian as the frontend viewer, rarely touches the wiki manually, and has the LLM handle all writes. Once the wiki grows large enough (~100 articles, ~400K words in his case), he runs complex Q&A against it without needing fancy RAG — the LLM auto-maintains index files and navigates the knowledge base on its own. Outputs get rendered as markdown, slideshows (Marp), or matplotlib images, all filed back into the wiki to keep compounding. His call: "I think there is room here for an incredible new product instead of a hacky collection of scripts."
- <https://x.com/karpathy/status/2039805659525644595|tweet>

He followed up with a natural extension: future frontier LLM queries could spawn entire ephemeral teams of LLMs — iteratively building wikis, linting them, looping, then producing full reports. "Way beyond a `.decode()`."
- <https://x.com/karpathy/status/2039808711452246261|tweet>

*Aaron Levie* (CEO at Box)

Levie shared a hard-won lesson from building Box Agent: be "brutally unsentimental" about your architecture. The rough loop he describes — build scaffolding → model improves → scaffolding becomes harmful → strip it out → new problems emerge → repeat — has already played out multiple times. Mitigations they built for context window limitations and retrieval accuracy actively hurt quality once models got better at those tasks. "Always make sure you're taking advantage of the frontier capabilities and don't become nostalgic around the tech you've already built."
- <https://x.com/levie/status/2039931799414194621|tweet>

*Ryo Lu* (Designer at Cursor)

On the day Cursor 3 launched, Ryo published a manifesto on what makes Cursor different: "glass vs. black box." The argument: AI tools have kept the opacity of terminals — type a wish, pull the lever, accept or reject. Cursor's bet is the opposite: every agent action visible, every diff inspectable, every plan editable. "As AI gets more powerful, glass gets more important. Not because you need to watch every move. But because the best work happens when you know you can." He also posted the official Cursor 3 launch: simpler interface that unfolds more tools when needed, works across local and cloud projects.
- <https://x.com/ryolu_/status/2039895634313187619|glass vs. black box>
- <https://x.com/ryolu_/status/2039780768847958359|Cursor 3 launch>

*Peter Steinberger* (builder, co-founder at OpenClaw)

Flagged a worrying signal from the Linux kernel security list: AI-generated bug reports have exploded from 2–3 per week two years ago to 5–10 per _day_ now. The reports are largely correct — which is creating a different kind of problem. Maintainers are getting overwhelmed with volume even when the quality is real. Steinberger's prediction: "This is gonna kill some OSS projects."
- <https://x.com/steipete/status/2039782190838686088|tweet>

*Amjad Masad* (CEO at Replit)

Replit is opening a sales office in Salt Lake City and is hiring there. Also shared a Replit-built agent that does SEO audits on your site.
- <https://x.com/amasad/status/2039777772701413396|Salt Lake City office>
- <https://x.com/amasad/status/2039838798671126728|SEO audit agent>

*Sam Altman* (CEO at OpenAI)

Called TBPN his favorite tech show and said OpenAI invested in them so they can keep doing what they do — and he's not expecting any softer treatment as a result. "I don't expect them to go any easier on us, am sure I'll do my part to help enable that with occasional stupid decisions."
- <https://x.com/sama/status/2039773740586918137|tweet>

*Dan Shipper* (CEO at Every)

Every has been beta testing Cursor 3.0 for a week and published a full "vibe check" review.
- <https://x.com/danshipper/status/2039770244361662920|tweet>

*Peter Yang* (Product at Roblox, newsletter author with 140K+ readers)

Tried Cursor 3 and found the new simplified interface a big improvement — the old UI had too many buttons and toggles that interrupted flow. Wonders why it isn't the default view since users currently have to hit `cmd+shift+p` to access it.
- <https://x.com/petergyang/status/2039850011044016291|tweet>

*Garry Tan* (President and CEO at Y Combinator)

Called Perplexity Computer "quite special actually" — brief but worth noting given the source.
- <https://x.com/garrytan/status/2039943351278190840|tweet>

*Claude AI* (Anthropic)

Computer use in Claude Cowork and Claude Code Desktop is now available on Windows.
- <https://x.com/claudeai/status/2039836891508261106|tweet>

*Swyx* (AI engineer; affiliated with Cognition, Temporal, AI Engineer community)

Reacted to TBPN announcing podcast sales with a question: time for a Dario Amodei × Dwarkesh Patel episode?
- <https://x.com/swyx/status/2039773480980480431|tweet>

*PODCASTS*

*Training Data — How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly*

_The Takeaway:_ Biology is about to undergo the disruption that software has promised for 30 years — and autonomous robotic labs are what finally make it real.

Jason Kelly founded Ginkgo Bioworks in 2008 on the idea that DNA is code and cells are programmable computers. Unlike digital computers that move information, cells move atoms — meaning you can, in theory, program them to synthesize anything. The problem has always been the lab: expensive, underutilized, physically tied to wherever scientists happen to be working.

Kelly's bet is that autonomous labs — where scientists submit experiment jobs via computer to a centralized robotic system — flip that equation entirely. Ginkgo already has 50 scientists submitting jobs into one centralized robotic setup in Boston. Traditional lab benches run below 20% utilization because humans cycle in and out; autonomous systems hit 70%+. Labs also get _smaller_, not bigger, because you no longer need to replicate equipment everywhere your scientists are located.

On humanoid robots in labs: Kelly is dismissive. "There are much better ways to do that than walk them bipedally among things. You just put them on a track." Biology is a microscopic discipline — humanoids solve the wrong problem.

The near-term applications Kelly is most excited about: AI-accelerated drug discovery, and longitudinal personal health monitoring via molecular blood testing (he thinks wearables are measuring the wrong things). The longer-term vision is more ambitious — Ginkgo just launched a Cloud Lab service where anyone can run experiments starting at $39 and receive data back. His analogy: in the 1960s, saying kids would program computers sounded insane. "I believe if you do manage to drop the cost of all this stuff, you may have kids and everybody else wanting to just ask original scientific questions."

"All of the previous revolutions in tech — Internet, social media, whatever — have been totally meaningless to biotechnology and biopharma. Not this. This is actually gonna change the fundamentals of how we do science."

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
