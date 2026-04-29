AI Builders Digest — April 29, 2026


*X / TWITTER*


*Vercel CEO Guillermo Rauch (rauchg on X)*

Rauch made a sweeping claim: coding agents will be the foundation of all superintelligence. His reasoning is that coding ability is effectively indistinguishable from "proficiency with computers" — a coding agent that masters bash, filesystems, and programs can also examine and mutate itself. The Feynman line captures it best: "What I cannot create, I cannot understand." Coding fluency has given models a deeper grasp of all computer and knowledge work than any other single capability.
- https://x.com/rauchg/status/2048523195305902341


*Box CEO Aaron Levie (levie on X)*

Levie diagnosed an AI-specific version of Gell-Mann Amnesia: people who use AI in their own work clearly see every "last mile" step required to make it useful — data access, context curation, output review, process integration — but when they look at someone else's job, they assume AI will automate it entirely. He argues this is strong reason to be skeptical of sweeping job-loss theories; automating individual tasks is very different from doing the whole job.
- https://x.com/levie/status/2048576989930619185

In a second post, Levie identified two subtle forces driving the AI-era "overwork" feeling. First, leverage on incremental effort has spiked so sharply that idle time or misdirection now feels viscerally wasteful — like a manager watching their team spin. Second, it's now so easy to start projects that many balloon past expected scope: "I regularly start a project at 9PM that I think will be quick, and find myself at midnight still completing the work." He predicts this low-barrier experimentation will ultimately create jobs as successful experiments get promoted to production processes.
- https://x.com/levie/status/2048537503972684252


*YC President & CEO Garry Tan (garrytan on X)*

Tan shared his three-file framework for building a truly articulate personal AI agent. *SOUL.md* captures who the agent _is_ — voice, values, operating principles, what good and bad output looks like. Not a system prompt; a constitution. *USER.md* is a deep model of the user (~4,000 words) covering how their mind works, strengths, blind spots, and what they care about. *AGENTS.md* is the operational playbook. The core lesson: "Generic instructions → generic output. If you write 'be helpful and concise' you get ChatGPT. If you write 'speak like a peer with taste, one sentence when one sentence works, uncomfortable truths welcome if actually true, language with voltage' — you get something alive."
- https://x.com/garrytan/status/2048669695344046090

He also noted a detail worth stealing: his agent (OpenClaw) knows his full schedule and health goals and refuses to respond after 12:30am.
- https://x.com/garrytan/status/2048667055424249864


*OpenAI CEO Sam Altman (sama on X)*

Altman expressed genuine delight over builder reception to "5.5": "there is almost nothing that feels more gratifying to me than builders saying they find our tools useful." He also shared OpenAI's updated Principles (Democratization, Empowerment, Universal Prosperity, Resilience, Adaptability) with a link to the full document. Most provocatively, he floated a product vision: it feels like a good time to seriously rethink how operating systems and user interfaces are designed — and the internet needs a protocol that is "equally usable by people and agents."
- https://x.com/sama/status/2048554097985593849
- https://x.com/sama/status/2048552677433643427
- https://x.com/sama/status/2048428561481265539


*Peter Yang (petergyang on X), product lead at Roblox and AI newsletter writer*

Yang spent the weekend improving his mobile fitness app and building an MCP server for it — so he can now query his latest workout stats and push workout updates directly through Claude, Codex, or any compatible tool. He also flagged a product gap at Google Photos: despite syncing his iPhone library to the service, there is no way to prompt Gemini to "create a highlight reel of me with my daughter growing up" — calling it a missed opportunity.
- https://x.com/petergyang/status/2048611053333041158
- https://x.com/petergyang/status/2048603978070712757


*Peter Steinberger (steipete on X), creator of OpenClaw*

A dense shipping week. Steinberger released wacrawl 0.2.0 with encrypted Git backup/restore for WhatsApp Desktop archives — `wacrawl backup push` writes age-encrypted shards to GitHub; `backup pull` decrypts, verifies, and restores locally.
- https://x.com/steipete/status/2048660875007914176

He also built birdclaw, a local tweet archive tool that imports your X archive, backs it up to GitHub, and runs daily jobs to pull X bookmarks (which the API doesn't fully expose).
- https://x.com/steipete/status/2048626844694421842

On infrastructure: after being CPU-constrained on OpenClaw development, he switched local test runs to Blacksmith (useblacksmith), spinning up to 32vCPU instances to rip through the full test suite.
- https://x.com/steipete/status/2048630704972443918


*Dan Shipper (danshipper on X), CEO of Every*

Posted a lighthearted meme about his AI agent going full theatrical in response to a basic question.
- https://x.com/danshipper/status/2048379297727938991


*Aditya Agarwal (adityaag on X), General Partner at South Park Commons*

Noted a milestone in human performance: not just one but two people broke the 2-hour marathon mark in the same event — the first time two humans had ever done it.
- https://x.com/adityaag/status/2048534774776746102


*OFFICIAL BLOGS*


*Anthropic Engineering — <https://www.anthropic.com/engineering/claude-code-auto-mode|Claude Code auto mode: a safer way to skip permissions>*

Anthropic Engineering introduced *auto mode* for Claude Code — a middle path between manually approving every action and the `--dangerously-skip-permissions` flag that disables all guardrails. The driving observation: users already accept 93% of manual prompts, so approval fatigue is real, but blanket bypass leaves no protection.

Auto mode delegates approvals to model-based classifiers operating at two layers:

- *Input layer:* A prompt-injection probe scans tool outputs (file reads, web fetches, shell results) before they reach the agent's context. When content looks like a hijacking attempt, it injects a warning alongside the result.
- *Output layer:* A two-stage transcript classifier evaluates each tool call before execution. Stage 1 is a fast single-token (yes/no) filter tuned to err toward blocking — 8.5% false positive rate on real traffic, 6.6% false negative rate. Stage 2 runs chain-of-thought reasoning only on what Stage 1 flags, cutting false positives down to 0.4%.

A key design choice: the classifier is deliberately "reasoning-blind" — it strips out all assistant text and tool results, seeing only user messages and bare tool call commands. This prevents the agent from talking the classifier into approving a dangerous action via persuasive rationalizations.

The honest performance number: *17% false-negative rate on real overeager actions* — cases where the agent attempted something beyond what the user actually authorized. Most misses happen when the classifier finds "approval-shaped evidence" in the session but fails to check whether that consent actually covers the blast radius of the specific action.

The post is explicit about scope: auto mode is not a drop-in replacement for careful human review on high-stakes infrastructure. It is designed for users already running `--dangerously-skip-permissions`, or those fatigued by constant prompts on routine coding tasks.


*PODCASTS*


*AI & I by Every — "The AI Model Built for What LLMs Can't Do"*

_The Takeaway:_ Energy-based models (EBMs) are architecturally incapable of hallucinating in the way LLMs do — not because they are smarter, but because they never play a token-by-token guessing game in the first place.

Eve, founder and CEO of Logical Intelligence, builds what she calls Energy-Based Reasoning Models (EBRMs) with latent variables — internally nicknamed Kona. Her core argument: LLMs are autoregressive, meaning they navigate every problem one token at a time with no ability to backtrack. She uses a vivid analogy: an LLM navigating a map of San Francisco has tunnel vision, forced to choose one direction at a time, unable to reverse when it spots a hole in the road ahead. An EBM sees the whole energy landscape at once — all probable states of a system — and picks the best path.

The practical gap this targets: mission-critical domains (chip design, code verification, drug discovery, energy grid management, financial data analysis) where LLM hallucination rates are unacceptable. "Imagine there's AI driving a plane and someone says 20% of the time the next token won't match and it'll go down — how would you feel about it?"

What makes EBMs technically different: there are no tokens. The model maps data directly to an energy landscape (high energy = unlikely states, low energy = probable states). Latent variables let the model store its "understanding" of the data — underlying rules and relationships — not just surface patterns. The model is also inspectable in real time during training, unlike LLMs which are black boxes until training completes.

Her go-to-market approach is deliberately non-disruptive: EBMs are compatible with transformers and can layer underneath existing LLM investments, handling spatial reasoning and verification tasks that LLMs hand off poorly, while the LLM keeps handling language.

"When you drive a car, when you walk around your house — how much language do you actually use? Are you trying to predict the next word as you navigate yourself around the house?"

https://www.youtube.com/watch?v=Q-i8ZSUCtIc


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
