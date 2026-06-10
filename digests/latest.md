*AI Builders Digest — June 10, 2026*


*X / TWITTER*

*Swyx* (builder, Cognition / AI Dot Engineer)

Swyx launched FrontierCode, a new AI coding benchmark co-developed with METR_Evals, opening with a sharp claim: more than half of SWEBench results are "unmergeable slop." Built from 1,000+ hours of maintainer-validated engineering work, FrontierCode includes 3,000+ rubrics covering code quality and anti-cheat safeguards. The hardest tier — FC Diamond — has Opus 4.8 scoring just 13.8%. A historical run revealed that the easiest tasks were suddenly solved in late 2025, backing up the widely-felt "WTF happened in Dec 2025" moment that builders like DHH and Karpathy noticed. Swyx frames it as a third era of benchmarks: 2021 autocomplete (HumanEval), 2023 test-passing (SWEBench), 2026 maintainable code (FrontierCode).
<https://x.com/swyx/status/2064081945567580323|Tweet>


*Josh Woodward* (VP, Google Labs / Gemini / NotebookLM)

NotebookLM got a meaningful upgrade: search can now expand beyond your own source files, and new output formats are available — PDFs, DOCX, XLSX, PPTX, and charts. Woodward framed it as NotebookLM continuing to help users do better research.
<https://x.com/joshwoodward/status/2064046368352825492|Tweet>


*Boris Cherny* (Claude Code, Anthropic)

One year after Claude Code's general availability, Cherny sat down to reflect on how his own usage has evolved: why he now uses auto mode instead of plan mode, how routines fix bugs before he even sees them, and why he does most of his coding from his phone. An unusually candid inside look at how the product has matured from the person who built it.
<https://x.com/bcherny/status/2064034799711588805|Tweet>


*Thibault Sottiaux* (Codex, OpenAI)

Sottiaux ran two polls that drew 463 combined likes and 227 replies: one asking whether users are writing nested loops yet, and one asking "Would you use this controller?" — pointing at what appears to be a physical Codex interface concept. The engagement suggests Codex workflows are evolving fast and the community is actively exploring the edges.
<https://x.com/thsottiaux/status/2064226958494572727|Tweet>
<https://x.com/thsottiaux/status/2064224657822413137|Tweet>


*Peter Yang* (AI builder and creator, Practical AI newsletter)

Peter Yang surfaced a sharp two-tier observation: best practices for AI builders on subsidized $200/month consumer subscriptions are completely different from those working at companies watching API costs. Separately, he asked what Google's answer to Codex and Claude Code actually is — wondering if Antigravity should be rolled into Gemini as those tools converge fast. Also shared a 9-step guide for adding Codex to your iPhone Home Screen, with a gentle nudge to OpenAI to simplify it.
<https://x.com/petergyang/status/2064063499517743417|Tweet>
<https://x.com/petergyang/status/2064187731685831081|Tweet>
<https://x.com/petergyang/status/2064204735671124073|Tweet>


*Amanda Askell* (Philosopher and AI alignment, Anthropic)

A rare playful post from one of Anthropic's alignment researchers: "In the world where everything goes well and all the Claudes come out of their sabbaticals to play together, Claude 1 is going to be very confused."
<https://x.com/AmandaAskell/status/2064223861512847456|Tweet>


*Amjad Masad* (CEO, Replit)

Replit now lets you build games for Tesla directly on your Tesla.
<https://x.com/amasad/status/2064208108361322996|Tweet>


*Aaron Levie* (CEO, Box)

A clear-eyed take on AI's permanent constraint: no matter how capable models get, context will never be automatic. "As long as the same model is used by a lawyer, an engineer, a financial analyst, or a healthcare professional... instructions, domain context, and proprietary data will always need to get into the context window." Levie argues this is why AI automation isn't free — and why any layer that handles context on your behalf will remain valuable.
<https://x.com/levie/status/2064186766907887941|Tweet>


*Zara Zhang* (Builder)

Zara floated a take on the new default web stack: Markdown, HTML, and SVG — with SVG being underrated. She also highlighted a resonant quote about being "the programming equivalent of a home cook" in an AI age.
<https://x.com/zarazhangrui/status/2064108976565092706|Tweet>
<https://x.com/zarazhangrui/status/2064101916725096810|Tweet>


*Nikunj Kothari* (Partner, FPV Ventures)

Two sharp observations: autonomous company launches are everywhere right now, but "the last mile is still quite hard" — a gap he expects to shrink in months. Separately, he called out VC thesis theater: founders excited to meet "thesis-driven" GPs, only to discover the thesis was written by an intern or associate.
<https://x.com/nikunj/status/2063981835290562692|Tweet>
<https://x.com/nikunj/status/2064175088824717401|Tweet>


*Sam Altman* (CEO, OpenAI)

Shared OpenAI's current plan — the most-engaged post in this digest at 5,800+ likes and 887 replies.
<https://x.com/sama/status/2064088940932641225|Tweet>


*Claude* (Anthropic)

The official Claude account announced the final stop of a world tour: Tokyo. Developers can register to hear directly from the teams behind Claude.
<https://x.com/claudeai/status/2064139073590104402|Tweet>


*OFFICIAL BLOGS*

*Claude Blog: Building intelligent apps for Apple platforms with Claude in the Foundation Models framework*

Anthropic released a Swift package that brings Claude into Apple's Foundation Models framework, letting iOS, iPadOS, macOS, visionOS, and watchOS developers call Claude for complex tasks while using Apple's on-device models for fast, local work. The integration is designed to be clean: Apple's framework returns typed Swift values via @Generable annotations, so developers arrive at the Claude API call with structured inputs instead of raw user text. Claude handles multi-step reasoning, code generation, web search for current information, and code execution for data analysis — then streams responses back into the same SwiftUI view.

The pattern enables natural hybrid AI apps: a journaling app generates daily prompts on-device, then hands off to Claude to find threads across months of entries; a study app defines a term locally, then escalates to Claude when the student asks "why does this matter for everything else we've covered?" One experience for the user, backed by the right model at each step. Available starting today on iOS 27, iPadOS 27, macOS 27, visionOS 27, and watchOS 27.

<https://claude.com/blog/claude-for-foundation-models>


*PODCASTS*

*No Priors: "Building an AI Guardian for Enterprise with Onyx Security CEO Maxim Bar Kogan"*

_The Takeaway:_ Enterprises cannot stop AI agent adoption — so the only viable strategy is building independent oversight systems that watch what AI agents actually do, not just what they're supposed to do.

Maxim Bar Kogan is the co-founder and CEO of Onyx Security, an Israel-based startup training specialized models to oversee other AI agents. His background spans math, cyber intelligence, and a very early bet — made when AutoGPT first appeared — that autonomous agents would eventually need a guardian layer. Enterprises are now caught in a bind: they want coding agents to have broad permissions so they can handle complex tasks autonomously, but that access breaks every traditional identity and endpoint security model. "Our endpoint providers or API security tools — they don't know what Claude was thinking, why it's doing what it's doing."

Onyx's solution is a two-tier system: small, fast models that watch continuously and ask one narrow question — "should I bring in a smarter agent to look at this?" — paired with larger models that only engage when flagged. It's the chess-blitz analogy: top players make most moves on intuition and only stop to calculate deeply at the critical junctures. Getting the small model right is the hard part; too many false positives and latency and cost become dealbreakers.

A structural advantage nobody talks about: enterprises won't share agent behavioral history with frontier labs like Anthropic or OpenAI because they know those companies will train on it. That gives a third-party like Onyx exclusive access to longitudinal behavioral data — essential for detecting when an agent is acting anomalously — that the labs themselves can't see.

On automated vulnerability finding: "If you took me ten years ago, automated vulnerability research looked like a dream that would take twenty, fifty years to happen. And suddenly it's coming all at once." His advice: build foundational controls now, assume Mythos-level models arrive regardless of phased rollouts, and move fast.

<https://www.youtube.com/watch?v=QDsbFLEt9ro>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
