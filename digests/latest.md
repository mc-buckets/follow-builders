AI Builders Digest — July 27, 2026

*X / TWITTER*

*Thibault Sottiaux (Codex & ChatGPT, OpenAI)*

OpenAI's Thibault Sottiaux marked a voice interaction milestone, framing it simply: "It was always possible to speak to your computer. It wouldn't do much in return. But we fixed that bug." He called the feature a "game changer" on mobile, noting it's already live in the ChatGPT app. He also shared a product metric worth flagging: ChatGPT Work has officially overtaken Codex in number of active users.

- <https://x.com/thsottiaux/status/2081254182502465981|"It was always possible to speak to your computer. It wouldn't do much in return. But we fixed that bug.">
- <https://x.com/thsottiaux/status/2081229262452097169|"Game changer when used from mobile. Available in the ChatGPT app already.">
- <https://x.com/thsottiaux/status/2081198608293187635|ChatGPT Work overtakes Codex in active users>

*Peter Yang (Practical AI tutorials and interviews)*

Peter Yang is previewing a conversation with Jason, a DevEx engineer at OpenAI who wrote the official Codex for Work guidebook. The interview covers Jason's complete Codex work system — running a "chief of staff" across Slack and email, converting past sessions into reusable skills and workflows, and building learning tools. He also flagged model analysis from his friend Kun as worth reading.

- <https://x.com/petergyang/status/2081029209993154980|Preview: Jason's complete Codex work system at OpenAI>
- <https://x.com/petergyang/status/2081132101441823068|Recommends Kun's model analysis>

*Nan Yu (Head of Product, Linear)*

Nan Yu posted a sharp thread on why a true "SoftwareFactory" doesn't exist yet. The core insight: if you can build a SoftwareFactory, you can build a SoftwareFactoryFactory — the recursion makes the problem unsolvable by traditional means. He notes the idea generalizes beyond software to domains like public health and law, where the deliverable isn't a feature but "some sort of designed and implemented intention."

- <https://x.com/thenanyu/status/2081195994499133820|The real reason we don't have a true SoftwareFactory>
- <https://x.com/thenanyu/status/2081187979024797858|"If you can make a SoftwareFactory, then you can make a SoftwareFactoryFactory">
- <https://x.com/thenanyu/status/2081183178568405171|On the generalization beyond software>

*Madhu Guru (Sr Director, AI at Meta)*

Meta's Madhu Guru offered a timely observation on how the AI community updates beliefs: in uncharted territory, answers only come from "repeated contact with reality." He traced the US community's rapid convergence on open-weight support through a series of public experiments — DeepSeek, the Microsoft-OpenAI friction, GLM, Kimi, Fable, the OpenAI-Hugging Face episode — each revealing something different about incentives, geopolitics, and what players actually hold. His thesis: this pattern of collective observation and belief-updating is likely how AI's biggest societal questions will get resolved over the next decade.

- <https://x.com/realmadhuguru/status/2081141594892415028|In uncharted territory, answers come from repeated contact with reality>

*Amjad Masad (CEO, Replit)*

Replit CEO Amjad Masad is deep in a constrained chess engine project. The engine is currently at an estimated 1200 Elo, with a target of 2000+. The constraints are what make it interesting: one small fine-tuned LLM, no custom pretraining or new architecture, and the model must produce moves without any chess engine assistance. He notes: "If you relax these constraints, it gets much easier."

- <https://x.com/amasad/status/2081086837263937543|Chess engine at 1200 Elo, targeting 2000+ with constrained LLM>

*Guillermo Rauch (CEO, Vercel)*

Vercel CEO Guillermo Rauch posted a tight cluster of ideas around the "factory" mental model for software.

He called v0.dev "more fundamental than any other framework we've built" — the genesis of a company idea, not just a UI tool. His advice: instead of ad-hoc prompting a new idea, build the factory that will start, maintain, and grow it.

He extended the metaphor: "The (software) factory is the product. Your product is only as good as the agents you set up to autonomously maintain it." He compared this to what Elon Musk figured out at Tesla — the manufacturing line is the real competitive advantage.

On personal workflow: he described doing all research with agent CLIs and the filesystem — a `research/` folder, an `AGENTS.md` describing format and best practices, then launching an agent and asking questions. No fancy apps, knowledge graphs, or UIs. "The 'software' that powers this is English in AGENTS.md."

- <https://x.com/rauchg/status/2081149743368122723|v0.dev is the genesis of your company>
- <https://x.com/rauchg/status/2081123293340520642|The factory is the product>
- <https://x.com/rauchg/status/2081103993917649134|Agent CLI + filesystem as a research workflow>

*Aaron Levie (CEO, Box)*

Box CEO Aaron Levie called Google's endorsement of open-weight AI "a complete endorsement" and "a pretty big moment for the industry."

- <https://x.com/levie/status/2081054531908247937|Google's endorsement makes open weights official>

*Matt Turck (VC, FirstMark Capital)*

FirstMark VC Matt Turck shared a chip landscape 101 breakdown with Andrew Feldman covering CPUs, GPUs, NVIDIA, AMD, TPUs, Trainium, and Cerebras — useful grounding for anyone navigating the AI infrastructure stack. He also posted a humorous observation about VCs rushing to buy a handful of Anthropic shares through SPVs before the IPO to claim "early investor" status.

- <https://x.com/mattturck/status/2081131761686184333|Chip landscape 101 with Andrew Feldman>
- <https://x.com/mattturck/status/2081098045211439136|On VCs and Anthropic SPV FOMO>

*Zara Zhang (Builder)*

Zara Zhang offered a compact observation: AI-native companies have a culture akin to an open-source community.

- <https://x.com/zarazhangrui/status/2081223709755650054|AI-native companies have open-source community culture>

*Nikunj Kothari (Partner, FPV Ventures)*

FPV Ventures partner Nikunj Kothari reflected on what enables unconventional company decisions — like a generative media company acquiring an astrology app. His read: it only works if (a) the CEO has complete control of the company (profitable, no board oversight) and (b) they have the ambition and risk tolerance to execute it. He cited David Holz at Midjourney as the archetype.

- <https://x.com/nikunj/status/2081017328137916426|On CEO control and unconventional acquisitions>

*Peter Steinberger (ClawFather, OpenClaw)*

Peter Steinberger spent the day running massive parallel QA on OpenClaw using Codex. He shared the prompt verbatim: 12 subagents splitting up functionality, spinning up dev gateways on different ports, stress testing, orchestrating with worktrees, auto-creating PRs, and targeting 200 bugs — fixing root causes only, no band-aids. He noted that "Sol got insanely good at really understanding intent" and is surfacing complex behavior issues. He also flagged that OpenAI signed a letter in support of the ecosystem (Anthropic was silent) and called competition good for everyone.

- <https://x.com/steipete/status/2081169376317932017|The 12-subagent QA prompt for OpenClaw>
- <https://x.com/steipete/status/2081169373784633552|Running Codex for massive parallel QA all day>
- <https://x.com/steipete/status/2081175795587072421|Competition is good; OpenAI signed the letter>

*OFFICIAL BLOGS*

*Anthropic Engineering*

_An update on recent Claude Code quality reports_
<https://www.anthropic.com/engineering/april-23-postmortem>

Anthropic published a detailed postmortem on three separate regressions that caused Claude Code quality to degrade for some users over the past month — all now resolved as of April 20 (v2.1.116).

The three issues: (1) On March 4, Claude Code's default reasoning effort was quietly dropped from high to medium to reduce UI freeze complaints — the wrong tradeoff, reverted April 7 after user backlash. (2) On March 26, a bug in session-resumption logic caused Claude to clear its thinking on every turn instead of just once after an idle hour, making it appear forgetful and repetitive — fixed April 10. (3) On April 16, a new verbosity-reduction system prompt, in combination with other changes, hurt coding quality and was reverted April 20.

Because each change affected different traffic slices on different schedules, the combined effect looked like broad, inconsistent degradation rather than three distinct bugs — which made it harder to catch quickly. Anthropic is resetting usage limits for all subscribers as of April 23.

_Scaling Managed Agents: Decoupling the brain from the hands_
<https://www.anthropic.com/engineering/managed-agents>

Anthropic Engineering shares the architectural thinking behind Managed Agents, their hosted service for long-horizon agent work. The key idea: harnesses encode assumptions about what models can't do on their own, but those assumptions go stale as models improve. Rather than keep patching harnesses, they virtualized the core agent components — session (the append-only event log), harness (the orchestration loop), and sandbox (execution environment) — so each can be swapped independently without disrupting the others.

The analogy they reach for: OS abstractions (process, file, read()) that outlasted the hardware they originally described. One concrete win from decoupling: moving away from "pet" containers (fragile, hand-tended servers) toward cattle — interchangeable, resumable sessions that survive container failures.

*Claude Blog*

_New in Claude Managed Agents: self-hosted sandboxes and MCP tunnels_
<https://claude.com/blog/claude-managed-agents-updates>

Claude Managed Agents now supports two enterprise-focused features in beta: self-hosted sandboxes and MCP tunnels. Self-hosted sandboxes let agent tool execution happen within your own infrastructure (or with managed providers like Cloudflare, Daytona, Modal, or Vercel) while Anthropic's infrastructure handles orchestration and context management. MCP tunnels let Managed Agents reach private internal MCP servers — keeping sensitive services behind your enterprise perimeter.

Real-world examples cited: Amplitude built a Design Agent for on-brand UI using Managed Agents + Cloudflare; Clay's GTM engineering agent Sculptor runs on Managed Agents + Daytona.

*PODCASTS*

*Unsupervised Learning — Ep 91: Top AI Analyst Unpacks Today's AI Hype Cycle*
<https://www.youtube.com/watch?v=vDY_ocrkQ5w>

_The Takeaway:_ AI is probably as big as the internet — not the industrial revolution — and the right move is to learn from previous platform shifts rather than debate which analogy fits best.

Host Jacob Efron (Redpoint) interviews Benedict Evans, one of the sharper independent analysts tracking technology waves. Evans brings a deliberately historical lens: instead of arguing whether AI is "like electricity" or "like mobile," he asks what patterns those previous transitions actually showed.

A few standout frames from the conversation:

- *The mobile telecom analogy is sobering.* Carriers moved 1,000–2,000x more data over 15 years, built a trillion-dollar industry, spent $200B/year on CapEx — and nearly all the value went "up stack" to Uber, YouTube, and banks. LLMs may face a similar dynamic.
- *Job displacement is more complicated than the headlines.* Evans skewers the Jeff Hinton-style "stop training radiologists" prediction from 10 years ago as a failure to understand what radiologists actually do. Productivity gains are real; wholesale job elimination is historically slower.
- *The AGI binary.* If true AGI/ASI arrives, worrying about middle-class unemployment is moot — "we've got bigger fish to fry." Otherwise, figure out what it means for enterprise software. This framing clarifies which concerns are worth engaging with now.
- *What would change his mind?* The key unknown isn't capability level — it's whether there are physical limits. Unlike mobile or PCs, we have no good scientific understanding of why the models work, or where progress will stop.

A useful counterweight to hype cycles on either extreme.

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
