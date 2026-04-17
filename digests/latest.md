AI Builders Digest — April 17, 2026

*X / TWITTER*

*Andrej Karpathy* (karpathy on X) — ex-OpenAI founding team, ex-Tesla Director of AI

Karpathy published a detailed breakdown of how he's using LLMs to build personal knowledge bases. The workflow: index raw source documents into a `raw/` directory, then have an LLM incrementally "compile" a Markdown wiki — complete with article summaries, backlinks, and concept pages — viewable in Obsidian. The LLM owns the wiki; Karpathy rarely edits it directly. "I thought I had to reach for fancy RAG, but the LLM has been pretty good about auto-maintaining index files and brief summaries of all the documents." Once the wiki grows large enough, you can run complex Q&A against it, file outputs back in, and run "health check" passes to find inconsistencies and surface new connections. He teased the natural extrapolation: a single frontier LLM query spawning a whole team of LLMs to build an ephemeral wiki, lint it, and write a full report.

- <https://x.com/karpathy/status/2039805659525644595|LLM Knowledge Bases>
- <https://x.com/karpathy/status/2039808711452246261|The ephemeral wiki team extrapolation>


*Aaron Levie* (levie on X) — CEO of Box

Levie shared what he calls the defining loop of building AI agents: scaffold heavily around the LLM to solve specific tasks well, then as models improve, ruthlessly strip that scaffolding away. "You have to be brutally unsentimental in your architecture." He traced Box Agent's evolution — components built to handle chunking, context windows, and search that eventually became constraints as newer models made them redundant. "Many of the mitigations we put in place... eventually meant we got lower quality results or meant we were overfitting for specific use-cases, as soon as the models got better." The main lesson: always take advantage of frontier capabilities and don't become nostalgic about tech you've already built.

- <https://x.com/levie/status/2039931799414194621|The AI agent architecture loop>


*Ryo Lu* (ryolu_ on X) — Designer at Cursor

Cursor 3 launched, and Lu published a design manifesto to go with it. The framing: "glass vs. black box." Most AI tools kept the terminal's opacity and made it more addictive — you type a wish, pull the lever, accept or reject the whole thing. Cursor's bet is the opposite: make everything visible and controllable. "Give away the wheel and you get mediocre. Keep it and you get to build something great." In Cursor 3, agents are visible, diffs are there, plans are editable, state is clear. The same tool adapts to different users — PMs, designers, engineers, beginners — at their own depth. "As AI gets more powerful, glass gets more important."

- <https://x.com/ryolu_/status/2039780768847958359|Cursor 3 launch>
- <https://x.com/ryolu_/status/2039895634313187619|Glass vs. black box manifesto>


*Amjad Masad* (amasad on X) — CEO of Replit

Masad was in product mode this week. He highlighted a no-setup enterprise-grade auth solution now available on Replit, demoed an SEO audit agent, and announced that Replit is opening a sales office in Salt Lake City, Utah.

- <https://x.com/amasad/status/2039774118443421887|Enterprise auth>
- <https://x.com/amasad/status/2039838798671126728|SEO audit agent>
- <https://x.com/amasad/status/2039777772701413396|SLC sales office>


*Peter Steinberger* (steipete on X) — AI builder, OpenClaw

Steinberger flagged a worrying signal about AI-generated noise overwhelming open-source maintainers. He quoted from the Linux kernel security list: volume of vulnerability reports has spiked from 2–3 per week two years ago to 5–10 per _day_ now, and maintainers attribute the entire increase to AI-generated submissions. "Prediction: This is gonna kill some oss projects."

- <https://x.com/steipete/status/2039782190838686088|AI slop overwhelming kernel security maintainers>


*Peter Yang* (petergyang on X) — Product at Roblox, AI newsletter author

Yang tried Cursor 3 and endorsed the simplified interface: "The old one had far too many buttons and toggles that got in the way of just talking to the agent." He argued the new streamlined view should be the default, not something you need a keyboard shortcut to reach.

- <https://x.com/petergyang/status/2039850011044016291|Cursor 3 review>


*Dan Shipper* (danshipper on X) — CEO of Every

Shipper's team spent a week testing Cursor 3.0 and published their full vibe check.

- <https://x.com/danshipper/status/2039770244361662920|Every's Cursor 3.0 vibe check>


*Sam Altman* (sama on X) — CEO of OpenAI

Altman announced OpenAI is supporting TBPN (the tech podcast) to keep it running, calling it his favorite tech show. "I don't expect them to go any easier on us, am sure I'll do my part to help enable that with occasional stupid decisions."

- <https://x.com/sama/status/2039773740586918137|OpenAI backing TBPN>


*Nan Yu* (thenanyu on X) — Head of Product at Linear

Yu posted what appears to be a thread teasing AI agent capabilities — noting that the subject "can be a product marketer when you need" and "or a PM you collaborate with."

- <https://x.com/thenanyu/status/2039820803722633589|Thread post 1>
- <https://x.com/thenanyu/status/2039823494398001448|Thread post 2>


*Garry Tan* (garrytan on X) — President & CEO of Y Combinator

Tan called out Perplexity Computer as "quite special actually."

- <https://x.com/garrytan/status/2039943351278190840|Perplexity Computer>


*Claude* (claudeai on X) — Anthropic

Computer use in Claude.ai and Claude Code Desktop is now available on Windows.

- <https://x.com/claudeai/status/2039836891508261106|Computer use on Windows>


*Swyx* (swyx on X) — AI engineer, Latent Space podcast

Reacted to news that TBPN is selling podcast stakes: "wait… you guys are selling podcasts??! (congrats! time for dario x dwarkesh?)"

- <https://x.com/swyx/status/2039773480980480431|TBPN stakes reaction>


*PODCASTS*

*Training Data — How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly*

*The Takeaway:* Robotic, AI-run autonomous labs will be 10x more capital-efficient than human labs — and that structural advantage means AI agents don't need to be smarter than scientists to win.

Jason Kelly is the founder and CEO of Ginkgo Bioworks, which he started in 2008 straight out of grad school with a mission to make biology programmable. The core insight: DNA is code (ATCGs instead of zeros and ones), and cells can be programmed like computers — except unlike computers, which move information, cells move _atoms_. That means programming biology can produce anything physical. Ginkgo bootstrapped for six years before Sam Altman, newly installed at YC, wrote a blog post saying the Silicon Valley model could work for deep tech — and Kelly cold-emailed him.

For the past fifteen years, Ginkgo has split its work between two problems: designing biology (writing better DNA code) and executing experiments cheaper and faster. Kelly has shifted Ginkgo's focus almost entirely to the execution side, seeing a structural opportunity that most biopharma leaders are missing.

The insight is structural: current research labs spend less than 5% of their budgets on actual reagents — the chemicals and materials consumed in experiments. Everything else is overhead: people, equipment, lab space, all sitting underutilized. An autonomous robotic lab flips this ratio, where 90% of costs go to reagents — meaning roughly 10x more experimental data per dollar. "They can even be dumber than the scientists. I think they win."

A second advantage: AI can hold the full context of all ongoing research projects simultaneously, something no human team can do. Scientists working in parallel labs can't see each other's work in real time; AI directors can.

Ginkgo is already running a live experiment: 50 scientists submitting jobs into one centralized robotic setup in Boston. One practical unlock — scientists hate coding. Their fix: use Claude Code and Codex so scientists submit written protocols in plain language, and the model handles the rest. "You will now submit a written protocol of what you want, and the model will figure it out. And if the model sends a plate sealed, we will update the skills file, and it will never do it again."

Kelly's bottom line: every previous tech revolution — the internet, social media — was "totally meaningless" to biopharma. "Not this. This is actually going to change the fundamentals of how we do science."

<https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8|Watch on YouTube>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
