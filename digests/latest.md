AI Builders Digest — June 1, 2026


*X / TWITTER*

*Thibault Sottiaux — Codex & ChatGPT at OpenAI*

Codex hit 5 million users, and Sottiaux is resetting usage limits to celebrate — over 800 community replies already poured in on what needs fixing. On model versioning: the GPT-5.0 → 5.1 → ... → 5.5 progression maps each increment to capability improvements and token efficiency gains. "GPT-5.5 [is] our best model yet. A simple strategy that we would like to continue."

- https://x.com/thsottiaux/status/2060964284117782996
- https://x.com/thsottiaux/status/2060627747760984429

*Peter Yang — Product at Roblox, AI newsletter author*

Yang spent an hour with his daughter on Brilliant.org doing CS 101 and left with a bigger vision: "The ultimate education app is you're playing Final Fantasy or something and you're learning math and CS at the same time." He also weighed in on AI company marketing differentiation, predicting "OpenAI Codex dank memes vs. Anthropic essays."

- https://x.com/petergyang/status/2060928818383355907
- https://x.com/petergyang/status/2060930599565811774
- https://x.com/petergyang/status/2060930334620053998

*Guillermo Rauch — CEO at Vercel*

A crisp product philosophy take: "Ship the best product. Use lots of AI, some AI, maybe no AI. Just be the best." Also announced per-API key spend caps on Vercel's AI Gateway — useful for teams managing cost across multiple AI integrations.

- https://x.com/rauchg/status/2060803480823193840
- https://x.com/rauchg/status/2060787704166776927

*Aaron Levie — CEO at Box*

Levie pushed back on AI-kills-jobs framing with a detailed enterprise read: most CIOs, CTOs, and CEOs he talks to are either growing headcount due to AI (new roles like FDEs) or reinvesting efficiency savings into underfunded areas — sales, marketing, customer success. He cited Goldman Sachs CEO David Solomon's NYT op-ed as articulating it well. "The companies that better serve their customers win over the long run, and those that just try and find savings end up doing worse."

- https://x.com/levie/status/2060923684295221390

*Ryo Lu — Designer at Cursor*

Highlighted Cursor's auto-review feature: before executing a command, it explains what the command does and flags the risk level. "Makes it much easier for new coders to learn and just do things."

- https://x.com/ryolu_/status/2060766674203353190

*Garry Tan — President & CEO at Y Combinator*

Flagged that the US building boom hasn't reached San Francisco yet — and called it a problem.

- https://x.com/garrytan/status/2060949003790176667

*Zara Zhang — Builder*

A small but notable model behavior observation: Opus 4.8 appears to have stopped using em dashes in its writing.

- https://x.com/zarazhangrui/status/2060962160872919043

*Peter Steinberger — OpenClaw / OpenAI*

Strong signal on what agentic workflows look like at full throttle: with GPT-5.5, /goal, autoreview, and crabbox, Steinberger scaled his tasks from 30–60 minute prompts to 4–10 hour autonomous runs — with much higher confidence the output is production-ready. "Yielding agents is a skill." He also shared a sharp debugging trick: Codex will say "all good" when asked to review code for bugs, but if you _tell_ it there's a bug, it loops persistently until it finds issues.

- https://x.com/steipete/status/2060678430031597696
- https://x.com/steipete/status/2060672154727825718
- https://x.com/steipete/status/2060691552486175041

*Dan Shipper — CEO at Every*

Shared a personal Codex usage stat that signals how deep power users are going: 38 billion tokens used, a 56-hour longest single task, and a 41-day active streak.

- https://x.com/danshipper/status/2060771279280513362


*OFFICIAL BLOGS*

*Claude Blog — New in Claude Managed Agents: dreaming, outcomes, and multiagent orchestration*

<https://claude.com/blog/new-in-claude-managed-agents>

Anthropic shipped three major updates to Claude Managed Agents:

- *Dreaming* (research preview): A scheduled background process that reviews past agent sessions and memory stores, extracts patterns, and curates memory so agents self-improve over time — automatically, or with human review before changes land. Harvey saw ~6x improvement in task completion rates. Netflix uses it to surface recurring issues across hundreds of parallel builds.

- *Outcomes*: Write a rubric describing what success looks like; a separate grader evaluates output in its own context window (independent of the agent's reasoning) and triggers another pass if needed. Up to +10 points improvement in task success, +8.4% on docx and +10.1% on pptx in internal benchmarks. Webhooks let you fire-and-forget — get notified when the outcome is met.

- *Multiagent orchestration*: A lead agent breaks complex jobs into pieces and delegates each to a specialist subagent with its own model, prompt, and tools — running in parallel on a shared filesystem. Every step is traceable in the Claude Console. Spiral by Every uses this with outcomes to score drafts against editorial rubrics before returning them. Wisedocs cut document review time by 50%.


*PODCASTS*

*Unsupervised Learning — Ep 87: Gemini Co-Lead on World Models, RL's Next Domains & Continual Learning*

_The Takeaway:_ Oriol Vinyals believes training on narrow hard domains like math and coding generalizes more broadly than expected — but the capability he most wants to see (and hasn't yet) is a model that can genuinely innovate in machine learning research.

Vinyals is co-lead of Gemini at Google alongside Noam Shazeer and Jeff Dean, with a career spanning AlphaGo, sequence-to-sequence models, and AlphaStar. The conversation was recorded the day after Google I/O.

On *world models*: He distinguishes two things often conflated under the label. Classical representation learning compresses the world into compact internal concepts. What Gemini Omni actually does is act as a language-controllable renderer — you describe movements or actions, and it simulates them. The "GPT moment" for pure visual understanding (deriving physics from video without text supervision) hasn't happened yet, and he sees it as one of ML's oldest unsolved quests.

On *memory*: The near-term path is file-system-style episodic storage — agents writing structured notes between sessions that compound over time. "I think that's probably paradigm shifting as well, similar to how we saw reasoning a year and a half ago." Personalizing model weights per user is impractical at scale; a shared model plus a personal knowledge base is more likely.

On *RL generalization*: He was surprised how well training on narrow hard problems (math, coding) generalizes to broader reasoning. He sees model self-judging — models evaluating their own outputs without a formal verifier — as the key to expanding RL into messier, subjective domains.

On *the Bitter Lesson*: The scaffolding developers build today (multi-agent routing, delegation logic, sub-agent coordination) will eventually be written on-the-fly by the models themselves.

_"I don't think I've seen truly outstanding ideas that a model has generated yet, but I am sure I will very soon."_

https://www.youtube.com/watch?v=NQczevdpxq0


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
