*AI Builders Digest — July 15, 2026*


*X / TWITTER*

- - -

*Swyx* (swyx on X) — AI engineer, affiliations at Cognition, Temporal, AI Dot Engineer, Latent Space Pod

Shared his current model stack for "Big Boy projects": Sol Ultra to plan, Fable 5 to critique, Sonnet 5/Terra Ultra/SWE 1.7 to ultracode/slop cannon, and Devin Review to review. He recommends always using a variant of mattpocockuk's "grill-me" or trq212's "interview-me" to elicit key decisions upfront — a disciplined way to structure multi-model workflows before writing a line of code.
<https://x.com/swyx/status/2076811977918484795|View tweet>

- - -

*Thibault Sottiaux* (Codex & ChatGPT at OpenAI) — thsottiaux on X

Teased that tomorrow might be an "8 million active user celebration day" — hinting at a major Codex milestone announcement incoming. Separately dropped a link to a new ChatGPT Work feature announcement.
<https://x.com/thsottiaux/status/2076907789763621237|8M users tease> | <https://x.com/thsottiaux/status/2076894071323537898|ChatGPT Work announcement>

- - -

*Cat Wu* (Claude Code + Cowork at Anthropic) — _catwu on X

Announced that Claude Artifacts just got an upgrade, pointing to significant new capabilities in the feature.
<https://x.com/_catwu/status/2076867882894684314|View tweet>

- - -

*Thariq* (Claude Code at Anthropic) — trq212 on X

Expanded on the Artifacts upgrade: the changes make Artifacts much more expressive and combinable in creative ways. His favorite use case — create a project dashboard in Claude Tag that can be edited by teammates *or* by local Claude Code sessions — turns Artifacts into a shared, live workspace that bridges chat and code.
<https://x.com/trq212/status/2076790799011131735|View tweet>

- - -

*Amjad Masad* (CEO at Replit) — amasad on X

Showed off realtime progress updates on personal model training runs. His take: _"This feels like early vibe coding except it's making personal models."_ The analogy is pointed — personal model training is reaching the same accessibility inflection point that vibe coding hit.
<https://x.com/amasad/status/2076776737074184661|View tweet>

- - -

*Guillermo Rauch* (CEO at Vercel) — rauchg on X

The two breakout v0.dev features: (1) ease of use / filesystem API and (2) observability — Vercel is doubling down on both. He also highlighted that open-weight models now account for *29% of Vercel AI Gateway tokens*, up from just 11% in April — a sharp signal of what's actually running in production. Separately, flagged feature flags as powerful infrastructure for "autonomous, self-optimizing websites and applications," framing agent-controlled experimentation as the next frontier for the web stack.
<https://x.com/rauchg/status/2076817174073880957|v0.dev features> | <https://x.com/rauchg/status/2076713720731042174|Open weights at 29%> | <https://x.com/rauchg/status/2076786138195595704|Feature flags for agents>

- - -

*Aaron Levie* (CEO at Box) — levie on X

Levie dropped a detailed structural forecast for the AI stack: frontier labs keep advancing; open weights rapidly absorb those breakthroughs for lower-cost customization; the "applied AI layer" — companies combining frontier and cheap models for specific domain workflows — captures the biggest opportunity; enterprises focus on getting their context and data in front of models. His bottom line: _"even though some of this gets framed as zero sum, there's just a ton of opportunity for all layers of the stack."_

He also highlighted a case study on using Fable as a "manager" model that delegates to cheaper models for execution: _"We were surprised to find that Fable's effective delegation actually decreased cost overall. It specified constraints and outcomes instead of spelling out the implementation... These are the habits of a good manager."_ Prediction: deep domain knowledge + smart model routing = core competitive differentiation for applied AI companies.

On per-enterprise model training: skeptical. The most sensitive enterprise data can't be packed into a model without breaking security and access control. 100x more custom model use cases are coming, but training per-enterprise is harder than it looks.
<https://x.com/levie/status/2076882332821373381|Full AI stack forecast> | <https://x.com/levie/status/2076839463410671637|Fable as manager model> | <https://x.com/levie/status/2076764958579446006|Per-enterprise model skepticism>

- - -

*Ryo Lu* (Designer at Cursor) — ryolu_ on X

Built a custom e-reader firmware from scratch using Cursor — featuring beautiful Latin + CJK typography, vertical layout (縱書), proper line breaking for large character sets, book/progress sync with ryOS, and speedy rendering with caching. Works on Xteink X3 + X4; you can ask Cursor to flash it for you. A showcase of hardware hacking becoming genuinely accessible via AI coding tools.
<https://x.com/ryolu_/status/2076713331113734641|Custom firmware post> | <https://x.com/ryolu_/status/2076713700942295226|Supported devices>

- - -

*Zara Zhang* (Builder / developer) — zarazhangrui on X

Posted a framework for the 3 levels of AI adoption in organizations, noting most companies are stuck at level 2. She also surfaced a conversation from earlier this year about building in public, growing an audience on X without "the slop," and thoughts on vibe coding.
<https://x.com/zarazhangrui/status/2076862290985730481|3 levels of AI adoption> | <https://x.com/zarazhangrui/status/2076860372993388663|Building in public video>

- - -

*Nikunj Kothari* (Partner at FPV Ventures) — nikunj on X

Built the *Ramp-Autofill skill* using Ramp's CLI and Claude Fable — an open-source Claude Code skill that automatically finds receipts from iMessage and Gmail (using Playwright to convert linked pages to PDFs), fills in expense memos from Google Calendar events, learns your organization's categorization style from past transactions, and auto-categorizes everything. He used it over one weekend to clear 60 days of backlogged expenses. Drop-in for Claude Code, fully open source.
<https://x.com/nikunj/status/2076775924650107151|Ramp-Autofill announcement> | <https://x.com/nikunj/status/2076776777884811671|Repo link>

- - -

*Peter Steinberger* (OpenClaw + OpenAI) — steipete on X

Shipped iOS and Android app updates alongside a new release (bumped Node for stability). Moved a maintainer agent to the cloud and noted they're "fighting already" — an honest glimpse at multi-agent coordination challenges in production. Also flagged that *"stress test"* is a surprisingly useful prompt for pushing AI systems hard.
<https://x.com/steipete/status/2076917691139674373|App release> | <https://x.com/steipete/status/2076923300593422560|Cloud agents fighting> | <https://x.com/steipete/status/2076886451455992249|"stress test" prompt>

- - -

*Sam Altman* (OpenAI) — sama on X

Sam noted it _"still sorta breaks my brain to see our models be good at design finally"_ (6.8K likes) — a candid acknowledgment of how far OpenAI's design capabilities have come. He also took a shot at Anthropic's API access policies with a cryptic tweet: _"hard questions are great but only if we deem you worthy enough to not silently downgrade you, or even get access at all"_ — and said a quoted post about the policy looked so implausible he checked for a fake handle.
<https://x.com/sama/status/2076823209589313910|Design comment> | <https://x.com/sama/status/2076824870072238299|API access critique>


*OFFICIAL BLOGS*

- - -

*Claude Blog: Building intelligent apps for Apple platforms with Claude in the Foundation Models framework*
<https://claude.com/blog/claude-for-foundation-models|Read the post>

Anthropic released a Swift package letting Apple developers use Apple's Foundation Models framework to call Claude for complex workflows. The integration is clean: Apple's on-device models handle fast, local tasks (summarization, extraction) in as few as three lines of code, then seamlessly hand off to Claude for multi-step reasoning, code generation, or live web search.

Because Apple's framework returns typed Swift values via @Generable annotations, developers arrive at the Claude API call with structured inputs rather than raw user text. Practical example: a journaling app generates daily prompts on-device, then asks Claude to find threads across months of entries — one seamless experience for the user, backed by the right model for each step. The package handles streaming, tool calls, and structured responses back into SwiftUI views. Available on iOS 27, iPadOS 27, macOS 27, visionOS 27, and watchOS 27.


*PODCASTS*

- - -

*The MAD Podcast with Matt Turck: Inside Nemotron & NVIDIA's AI Lab | Bryan Catanzaro*
<https://www.youtube.com/@DataDrivenNYC/videos|Watch on YouTube>

*The Takeaway:* The smartest path to more AI intelligence isn't applying more force — it's building more efficient systems, and every architectural decision in Nemotron flows from that conviction.

Bryan Catanzaro leads Nemotron, NVIDIA's open foundation model family — though most people don't realize NVIDIA has been quietly building frontier AI since 2017, before transformers were mainstream. The Nemotron 3 family (Nano/Super/Ultra) is purpose-built for agentic reasoning and packs several genuinely novel technical bets: pretraining in 4-bit arithmetic (NVFP4), a hybrid transformer + state-space model architecture, mixture-of-experts with a "latent MOE" that compresses activations before routing them across GPUs to save bandwidth, multi-token prediction for faster inference without accuracy loss, and multi-teacher distillation that lets 10–15 domain specialists train one generalist.

The underlying philosophy: _"If you accept as the truth that we're gonna be running at the limit, then what that means is that the way to get more intelligence is to be more efficient. We can't get more intelligence by applying more force if we're already at the limit."_

Catanzaro is skeptical of singularity framing — intelligence is too multifaceted and contextual for a single threshold to be meaningful. More interesting to him: AI becoming so embedded in everyday life that people stop thinking of it as AI at all. On reinforcement learning, he sees environments as the key unlock: today's RL environments are "still fairly simple," and as they become richer and more diverse, models will get dramatically better at real-world reasoning beyond coding and math.

One organizational insight worth noting: Nemotron isn't built by one team — it spans roughly 10 teams across NVIDIA. Their solution is to make the mission the boss, run a biweekly compute allocation process, and maintain an internal idea-submission system reviewed by 25 domain leads — a rare look at how a large company actually coordinates hundreds of researchers toward one model. The multi-teacher distillation technique isn't just a training trick; it's also what lets competing research efforts all "win" without anyone's work being sidelined.


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
