AI Builders Digest — April 4, 2026

---

## X / TWITTER

**Andrej Karpathy** (former Tesla AI Director, OpenAI founding team)

Karpathy published a detailed breakdown of his personal LLM knowledge-base workflow: raw source documents (articles, papers, repos) go into a `raw/` directory, an LLM "compiles" them into a Markdown wiki with summaries, backlinks, and concept articles, and then an LLM agent fields complex Q&A against the growing wiki. He uses Obsidian as the frontend IDE and notes: "the LLM writes and maintains all of the data of the wiki, I rarely touch it directly." The natural next step, he suggests, is every frontier LLM query spawning an entire ephemeral team of LLMs — building a wiki, linting it, and producing a full report — far beyond a simple `.decode()`.

- https://x.com/karpathy/status/2039805659525644595
- https://x.com/karpathy/status/2039808711452246261

---

**Aaron Levie** (Box CEO)

Levie laid out the central discipline of building AI agents: brutal unsentimental architecture. Models improve fast, and scaffolding you built last quarter to compensate for their weaknesses becomes deadweight — or actively harmful — once the model can handle those things natively. His loop: build scaffolding → model capabilities leap → tear scaffolding out → new harder problems appear → repeat. Working on Box Agent, he saw multiple components of the agent harness become constraints as reasoning, tool use, and context-window performance all improved. "The main lesson is always make sure you're taking advantage of the frontier capabilities and don't become nostalgic around the tech you've already built."

- https://x.com/levie/status/2039931799414194621

---

**Ryo Lu** (Designer at Cursor)

Ryo published a "glass vs. black box" design manifesto explaining the philosophy behind Cursor. Black-box AI takes the wheel, returns a result, and asks you to accept or reject it; over time you see less and think less. Glass AI keeps every agent step visible, every diff present, every plan editable — not because you need to watch every move, but because the best work happens when you know you *can* intervene. "Give away the wheel and you get mediocre. Keep it and you get to build something great." He also announced the launch of Cursor 3 — a simplified interface that starts clean and unfolds more tools when needed.

- https://x.com/ryolu_/status/2039895634313187619
- https://x.com/ryolu_/status/2039780768847958359

---

**Peter Yang** (Roblox PM, newsletter author)

Tried Cursor 3 and found the new interface a clear improvement — the old UI had too many buttons and toggles that interrupted flow. He wonders why the new minimal view isn't the default, noting users currently have to hit `cmd+shift+p` to access it.

- https://x.com/petergyang/status/2039850011044016291

---

**Dan Shipper** (Every CEO)

Every ran a full week-long vibe check on Cursor 3.0 and published their findings.

- https://x.com/danshipper/status/2039770244361662920

---

**Sam Altman** (OpenAI CEO)

Endorsed TBPN (The Breakfast Podcast Network) as his "favorite tech show" and expressed support for them keeping their independence — noting he expects no lighter treatment: "I don't expect them to go any easier on us, am sure I'll do my part to help enable that with occasional stupid decisions."

- https://x.com/sama/status/2039773740586918137

---

**Amjad Masad** (Replit CEO)

Announced Replit is opening a sales office in Salt Lake City, Utah, and is hiring there.

- https://x.com/amasad/status/2039777772701413396

---

**Garry Tan** (YC President & CEO)

Called Perplexity Computer "quite special."

- https://x.com/garrytan/status/2039943351278190840

---

**Peter Steinberger** (builder and OpenClaw co-founder)

Flagged an accelerating OSS stress signal: AI-generated vulnerability reports flooding the Linux kernel security mailing list jumped from 2–3 per week two years ago → ~10 per week last year → 5–10 per day since January 2026. Maintainers have had to bring in extra help. Prediction: "This is gonna kill some OSS projects."

- https://x.com/steipete/status/2039782190838686088

---

**Claude** (Anthropic)

Computer use in Claude Code Desktop is now available on Windows.

- https://x.com/claudeai/status/2039836891508261106

---

**Swyx** (AI engineer; Cognition, Temporal, AI Engineer community)

Reacted to TBPN announcing podcast sales with one ask: a Dario Amodei × Dwarkesh Patel episode.

- https://x.com/swyx/status/2039773480980480431

---

## PODCASTS

### Training Data — "How Autonomous Labs Will Transform Scientific Research: Ginkgo Bioworks' Jason Kelly"

**The Takeaway:** AI reasoning models paired with robotic labs will beat human scientists — not by being smarter, but by running more experiments per dollar and sharing every result in real time.

Jason Kelly, founder and CEO of Ginkgo Bioworks, has a conviction most of the biology world hasn't caught up to yet: this AI moment is the first tech revolution that will actually change the *fundamentals* of how science gets done. "All of the previous revolutions in tech — Internet, social media, whatever — have been totally meaningless to biotechnology and biopharma. Not this."

Ginkgo put that thesis to a direct test in partnership with OpenAI. They handed a reasoning model a robotic lab and 30,000 experiment slots to optimize cell-free protein synthesis — a technique for producing proteins cheaply outside a living cell. After six iterative rounds (design experiments, run them robotically, get data back, redesign), the model beat the Stanford state-of-the-art benchmark by 40%. What made it work wasn't exotic creativity. The model ran through the scientific method — hypothesize, test, analyze, iterate — as pure logic, just faster and without stopping.

Kelly identifies two structural edges that make this durable: **Information sharing** — today's scientists exchange results once a year via paper; 100 AI scientists on a shared lab could share every failed experiment daily, letting one agent's dead end become another's shortcut. **Cost efficiency** — biopharma R&D currently spends less than 5% of its budget on actual reagents; the rest is overhead (people, lab space, equipment duplication). Autonomous labs flip this toward 90% reagent spend, yielding roughly 10x more data per dollar.

"They can even be dumber than the scientists. I think they win."

Kelly's near-term vision: parallel AI scientists running multiple hypotheses on a shared robotic lab, pooling data nightly, publishing weekly summaries for human review and direction. The bigger implication is for how the NIH funds research and how every biopharma head of R&D should be thinking right now.

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8

---

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
