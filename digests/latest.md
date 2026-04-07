*AI Builders Digest — April 7, 2026*

26 tweets across 12 builders · 1 podcast episode · No blog posts today


*X / Twitter*

*Andrej Karpathy* — AI researcher (formerly Director of AI @ Tesla, founding team @ OpenAI)

Two substantial posts today. First, a quick vision sketch: every frontier LLM query could soon spawn a swarm of sub-agents that iteratively builds an ephemeral wiki, lints it, and outputs a full report — "way beyond a `.decode()`." <https://x.com/karpathy/status/2039808711452246261|link>

The bigger post was a detailed walkthrough of his personal LLM-powered knowledge base workflow. The setup: ingest raw source docs into a directory, have an LLM compile and maintain a wiki of `.md` files with summaries and backlinks, then run Q&A agents against it. He uses Obsidian as the IDE frontend, vibe-coded a naive search engine as a CLI tool for the LLM, and runs "health checks" to catch inconsistencies and surface new article ideas. Outputs — slides, charts, reports — get filed back into the wiki so every query compounds. At roughly 100 articles and 400K words, complex Q&A works without fancy RAG. His parting thought: "I think there is room here for an incredible new product instead of a hacky collection of scripts." <https://x.com/karpathy/status/2039805659525644595|Full thread>

*Aaron Levie* — CEO @ Box

A hard-earned lesson from shipping Box Agent: be brutally unsentimental about your architecture. The loop is: build scaffolding around the LLM to handle hard tasks → model improves and makes the scaffolding a constraint → strip it out to recapture gains → repeat. Components built for chunking, retrieval, and context handling had to be jettisoned multiple times between design and launch as frontier models improved at reasoning, search, and long-context work. "Always make sure you're taking advantage of the frontier capabilities and don't become nostalgic around the tech you've already built." <https://x.com/levie/status/2039931799414194621|Full thread>

*Ryo Lu* — Designer @ Cursor

Wrote the philosophical launch post for Cursor 3. The central frame: AI tools became black boxes ("type a wish and pull the lever — you see less and think less as the model got better"), while Cursor is "glass" — visible agents, editable plans, clear state, readable diffs. Different users engage at different depths: the PM watches the plan become real, the expert lets it flow and steers when something feels off, the new programmer reads every diff and builds intuition. "As AI gets more powerful, glass gets more important. Not because you need to watch every move. But because the best work happens when you know you can." <https://x.com/ryolu_/status/2039895634313187619|Glass vs. black box>

Cursor 3 is now live — simpler default interface that unfolds more tools on demand, works across local and cloud projects. <https://x.com/ryolu_/status/2039780768847958359|Cursor 3 launch>

*Peter Steinberger* — Co-founder @ OpenClaw

Flagged a real signal buried in OSS maintainer pain: AI-generated security bug reports to the Linux kernel list have exploded from 2–3/week two years ago to 5–10/day in early 2026 — and most are reportedly valid, forcing the kernel team to bring in extra maintainers. "Prediction: This is gonna kill some oss projects." <https://x.com/steipete/status/2039782190838686088|link>

*Amjad Masad* — CEO @ Replit

Highlighted a Replit agent that runs SEO audits on your site <https://x.com/amasad/status/2039838798671126728|link>. Announced a new sales office opening in Salt Lake City, Utah, with open roles <https://x.com/amasad/status/2039777772701413396|link>. Also shared a no-setup enterprise-grade auth solution now available on Replit <https://x.com/amasad/status/2039774118443421887|link>.

*Sam Altman* — CEO @ OpenAI

Commented on OpenAI's involvement with TBPN (a tech show). Called it his favorite tech show, said he doesn't expect them to go easier on OpenAI: "am sure I'll do my part to help enable that with occasional stupid decisions." <https://x.com/sama/status/2039773740586918137|link>

*Dan Shipper* — CEO @ Every

Shared Every's week-long vibe check of Cursor 3.0, published the same day as the launch. <https://x.com/danshipper/status/2039770244361662920|Every's Cursor 3.0 vibe check>

*Peter Yang* — Product @ Roblox · AI newsletter (140K+ readers)

Tried Cursor 3 and found the new interface much cleaner — "The old one had far too many buttons and toggles that got in the way of just talking to the agent." Wonders why the new view isn't the default. <https://x.com/petergyang/status/2039850011044016291|link>

*Swyx* — AI engineer · @aidotengineer · co-host @ Latent Space

Reacted to the TBPN acquisition news with "you guys are selling podcasts?!" and mused about a potential Dario Amodei × Dwarkesh Patel episode: "time for dario x dwarkesh?" <https://x.com/swyx/status/2039773480980480431|link>

*Garry Tan* — President & CEO @ Y Combinator

Called Perplexity Computer "quite special actually" <https://x.com/garrytan/status/2039943351278190840|link> and shared a brief riff on loving your work. <https://x.com/garrytan/status/2039948180977316164|link>

*Nan Yu* — Head of Product @ Linear

Riffing on LLMs as flexible product collaborators — "Or a PM you collaborate with" and "Or it can be a product marketer when you need" — pointing toward a broader mental model shift for how builders think about AI teammates. <https://x.com/thenanyu/status/2039823494398001448|link> Also pitched "TBPN for sports." <https://x.com/thenanyu/status/2039832290490994970|link>

*Claude AI* — Anthropic

Computer use in Claude Cowork and Claude Code Desktop is now available on Windows. <https://x.com/claudeai/status/2039836891508261106|link>


*Podcast*

*Training Data — "How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly"*
<https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8|Watch on YouTube>

AI is the first tech revolution that actually matters for biology. That's Jason Kelly's central argument — and he's spent 18 years building toward it. The CEO of Ginkgo Bioworks contends that "all of the previous revolutions in tech — the internet, social media — have been totally meaningless to biotechnology. Not this."

Kelly founded Ginkgo in 2008, bootstrapped for six years straight out of grad school (biotech VCs "really don't like young people"), and got a lifeline via Sam Altman and YC in 2014. His core problem: biology labs involve high-variability, hard-to-predict work that resisted automation. He uses a transportation analogy — subways are easy to automate (fixed rails, low variability), cars aren't. Autonomous vehicles cracked that barrier. AI is doing the same for the lab.

His proof point: Ginkgo's collaboration with OpenAI on cell-free protein synthesis optimization. Their reasoning model improved on Stanford's benchmark by 40% after six iterations, running approximately 30,000 experiments. The key wasn't raw intelligence — "what really let it break through wasn't that it was so smart. It was that it could run experiments."

The long-run implication is democratization. If autonomous labs drive experiment costs low enough, original scientific research becomes accessible to millions of people — the same shift personal computers made for programming. Kelly believes biopharma, which has been largely untouched by tech for 30 years, is about to face genuine disruption.


_Generated by the Follow Builders skill: https://github.com/mc-buckets/follow-builders_
