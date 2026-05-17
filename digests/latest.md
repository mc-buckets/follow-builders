AI Builders Digest — May 17, 2026

*X / TWITTER*

*Swyx* (AI educator / latentspace.pub, AI dot engineer)
Swyx attended a Codex demo and was visibly impressed: "gotta say Codex is completely unrecognizable from 3 months ago. guys went extreme founder mode on this thing." Gabriel Chua was demoing what Swyx described as "agentic Excel on Mac." He also flagged a striking data point from Singapore's head of AI Govtech: 1.3 billion agents deployed in the country within two years, backed by a national MCP gateway in progress.
• <https://x.com/swyx/status/2055494400252481687|Codex is unrecognizable — demo thread>
• <https://x.com/swyx/status/2055470634331750588|Singapore: 1.3B agents + national MCP gateway>

*Peter Yang* (Roblox product / Practical AI newsletter, 140K+ readers)
On the newly launched ChatGPT Finances: useful but imperfect — "AI still has trouble classifying transactions correctly." More notably, he flagged a privacy consideration: he turned off the "improve the model for everyone" toggle to keep financial data out of training, and observed there's no separate "use for ad targeting" toggle, so presumably one controls both.
• <https://x.com/petergyang/status/2055396161910194395|ChatGPT Finances first impressions>
• <https://x.com/petergyang/status/2055450577094738018|Privacy toggle observation>

*Madhu Guru* (Product Leader, Google — Gemini, Veo, Nano)
A blunt take on the PM profession: "A generation of PMs is struggling to adapt to AI because they were trained to execute playbooks. AI requires inventing them." Madhu argues the era of repurposing stable product frameworks is over — "it's also why so much software feels the same" — and that you can't A/B test your way to a breakthrough AI product. PMs need to become inventors, not framework executors.
• <https://x.com/realmadhuguru/status/2055414865146327088|PMs need to become inventors>

*Guillermo Rauch* (Vercel CEO)
Three threads worth noting: (1) Grok CLI now has a Vercel plugin — watch a full creative coding site get generated and deployed without leaving the CLI. (2) A neat DX fix: when agents hit 401 Unauthorized on their own Vercel deployments (protected by SSO), `vercel curl` unblocks them. (3) A career take: "If you become exceptional at managing agents, but are also exceptional in your understanding of the fundamentals, you will be unstoppable."
• <https://x.com/rauchg/status/2055491454307582454|Grok CLI + Vercel plugin demo>
• <https://x.com/rauchg/status/2055440326765244742|vercel curl solves agent 401 problem>
• <https://x.com/rauchg/status/2055278852931530784|Mastery + agent amplification>

*Aaron Levie* (Box CEO)
Levie made the case for why forward deployed engineering (FDE) is becoming a core competency for AI adoption at scale. Unlike traditional software — stable once delivered — AI is "constantly evolving both due to the nature of new capabilities and best practices that emerge, but also because the underlying models change so much that they can meaningfully change the workflow." As AI moves from chat to agentic systems, having one vendor share learnings across thousands of customers is structurally more efficient than every company learning independently. He also flagged headless software as the coming paradigm.
• <https://x.com/levie/status/2055501840419328286|FDE is a core AI competency>
• <https://x.com/levie/status/2055357619888595271|Headless software is the future>

*Nikunj Kothari* (Partner, FPV Ventures)
Nikunj had a genuine awe moment watching an agent work autonomously while he had coffee with founders: "What do you mean you went through all the entire database of 2k+ line items, fixed all the product images, the frontend bugs caused by different images, the descriptions, used browser harness to get real-time info from the web, used web search for fact checking, wrote scripts for all the work you did for the future... and ran for 2 hours." His take: "/goal is just AGI if given the right tools."
• <https://x.com/nikunj/status/2055426430654439485|Agent ran autonomously for 2 hours>

*Peter Steinberger* (Co-founder, OpenClaw)
In a detailed thread, Steinberger described what building software looks like when you stop worrying about token costs: ~100 Codex instances running in parallel reviewing every PR and issue, security scanning every commit, de-duplicating bug reports, spinning up ephemeral machines to reproduce issues and film before/after videos, and agents that listen to internal meetings and start opening PRs mid-discussion. The whole system is framed around one question: "How would we build software in the future if tokens don't matter?" He also launched *clawpatch 0.1.0* — an open-source tool that maps codebases into semantic feature slices and reviews them for bugs and quality issues (`npm install -g clawpatch`).
• <https://x.com/steipete/status/2055405041843052792|OpenClaw's full agent infrastructure stack>
• <https://x.com/steipete/status/2055364630709448970|clawpatch 0.1.0 launch>

*Dan Shipper* (CEO, Every)
After trying to launch an agent-as-a-service platform on top of OpenClaw, Shipper shared two hard-won lessons: (1) Building on OpenClaw as a platform is painful — it moves fast, has regressions, and "it's not great to be the layer in between OpenClaw and a user." (2) One super-agent for a whole company beats 1:1 agents for each person. Agents still require significant technical upkeep, and most people don't want to manage agent internals. The scalable model is making it someone's explicit job to build and maintain a shared company agent.
• <https://x.com/danshipper/status/2055347527457886336|Lessons from building agent-as-a-service>

*Sam Altman* (CEO, OpenAI)
A brief but telling note: the team takes user feedback reports seriously — even when the conclusion turns out to be "I got used to the current level of magic and now I'd like more please."
• <https://x.com/sama/status/2055356452286640630|On taking user reports seriously>

*PODCASTS*

*Unsupervised Learning (Redpoint): Ep 86 — Yann LeCun on Leaving Meta, Breaking The LLM Paradigm, & Why Hinton is Wrong*

_The Takeaway:_ LLMs are genuinely useful — but they are the wrong paradigm for reaching human-level intelligence, because they cannot predict consequences or plan, and those two capabilities are what intelligence actually requires.

Yann LeCun — Turing Award winner, co-creator of Meta's FAIR lab, and now founder of AMI Labs (Advanced Machine Intelligence) — built his career on the theory that real intelligence requires world models, not language models. He left Meta to prove it.

The core argument is architectural. A system that predicts the next token cannot, by construction, anticipate the consequences of its own actions or engage in planning. LLMs are excellent for tasks where language itself is the substrate of reasoning — code, math, legal text — but "reality is way more complicated than language because it's high dimensional, continuous, noisy, messy." The result: "LLMs are good programmers. They're not software architects. They're not computer scientists."

His alternative, JEPA (Joint Embedding Predictive Architecture), predicts abstract representations rather than raw pixels or tokens. Instead of generating data, JEPA jointly encodes two views of the same input and learns to predict one representation from another — a non-generative approach that has produced better results (DINO, iJEPA, VJEPA) than any generative model for learning from video and physical data.

On AI safety, LeCun's diagnosis is stark: "LLMs are intrinsically unsafe. I don't think they can be made reliable and safe." His proposed fix isn't better alignment training — it's a fundamentally different architecture: objective-driven AI that uses a world model to optimize against explicit cost functions, with safety constraints that cannot be bypassed "by construction." LLMs, he argues, can always escape any constraint via some adversarial prompt. "There's always gonna be a prompt where the system is gonna do really stupid things."

On the industry: "There's a bit of this sort of herd behavior... everybody is digging the same trench." He deliberately located AMI Labs in Paris and New York, not Silicon Valley. His timeline: "The realization that you need to change a paradigm is happening as we speak. It will become completely obvious to people by early 2027."

On what he learned running FAIR: "The best way to get breakthrough research is you hire the best people, and you get the fuck out of the way."

<https://www.youtube.com/watch?v=ngBraLDqzdI|Watch: Yann LeCun on What Comes After LLMs>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
