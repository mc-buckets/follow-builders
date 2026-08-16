*AI Builders Digest — August 16, 2026*


*X / TWITTER*


*Swyx* — AI engineer, affiliated with smol.ai, Cognition, AI.Engineer, and the Latent Space Podcast

Swyx took a wry shot at Databricks' eye-popping $188B "Series M" fundraise, joking that the "M" stands for "we are going to kill so many meetings" — a nod to how seriously enterprise AI productivity is now being priced. https://x.com/swyx/status/2088381680478540096

He also flagged that wave 1 acceptances for the AIE NYC conference CFP are being finalized, calling last year's New York summit the most successful event they've ever held. https://x.com/swyx/status/2088322211241447801


*Josh Woodward* — VP at Google Labs, Gemini App, and Google AI Studio

Woodward announced that Gemini 3.7 Flash has landed in the Gemini App. https://x.com/joshwoodward/status/2088344782821326980

He also highlighted a new capability for Pomelli, Google Labs' AI marketing tool for small businesses: users can now turn product photoshoots into short videos or GIFs. https://x.com/joshwoodward/status/2088261701028503965


*Thibault Sottiaux* — Codex & ChatGPT at OpenAI

Sottiaux announced that restaurant reservations are now easy to find directly in ChatGPT, part of a batch of new feature launches. https://x.com/thsottiaux/status/2088493756391768252


*Peter Yang* — AI educator and author

Yang dug into X's open-source spam-detection algorithm and found it uses a behavioral model called TweetSpamBot — trained on up to 512 recent account actions — looking for signals like posting bursts, quote-tweet spamming, and unnatural timing patterns. The gap: it doesn't read post content. That means a sophisticated AI content mill can still post high-volume templated slop by recycling viral posts through the same quote-tweet formula, evading the behavioral model entirely. His recommendation: flag accounts that repeatedly quote-tweet unrelated viral posts with the same template at high volume. https://x.com/petergyang/status/2088261100202868768


*Nan Yu* — Head of Product at Linear

Yu pushed back on the popular framing that AI is "jagged" — better than humans at some things, worse at others. His take: that's not a useful lens. It's like saying dogs are "jagged" compared to humans. AI is just AI-shaped. https://x.com/thenanyu/status/2088335744909619230

He also dropped a sharp critique of internal product culture: "There's no force in tech as destructive as the PM promo packet." https://x.com/thenanyu/status/2088461657311785236

On team dynamics, he argued that when your colleagues are smart, their ideas always come from somewhere real — and some of the best products ship as fusions or derivatives of multiple ideas, not any one original concept. https://x.com/thenanyu/status/2088278730808426900


*Madhu Guru* — Sr. Director of AI at Meta (formerly led Gemini, Veo, and Nano at Google)

Guru invoked the Jevons Paradox to argue that AI won't reduce the demand for software engineering — it will dramatically increase it. Lower cost and complexity historically unlock entirely new categories of use cases (steam engines, high-level languages, spreadsheets), and AI + software engineering will likely follow the same pattern. https://x.com/realmadhuguru/status/2088294414255112329

He credited Cursor with breaking AI products out of the chatbot rut: "Cursor's impact on AI product culture is underrated. For a while, AI products were stuck in the chatbot phase… it was then that 'cursor for X' came along and inspired a whole new product pattern." https://x.com/realmadhuguru/status/2088489059115270532

His bottom line for builders: when everyone can build with AI, the differentiators are product sense, domain knowledge, distribution, and execution. https://x.com/realmadhuguru/status/2088425380130783287


*Aaron Levie* — CEO of Box

Levie wrote a detailed breakdown of how Cursor executed the applied AI playbook flawlessly — shattering assumptions that the dev tools market was saturated and low-ceiling. Cursor's approach: find the right product shape for agentic coding, act as a neutral layer between models and workflows, post-train models where it makes sense, build the right infra for those workflows, and build a GTM motion category-aligned to the work. "Multiple mental models shattered near instantly. The market sizes for agentic coding was far larger than most realized." He called it a reference case for anyone doing applied AI today. https://x.com/levie/status/2088476232933577124


*Garry Tan* — President & CEO of Y Combinator

Tan shared a striking observation about Fable 5 and his GStack setup: on one-way-door decisions that previously required careful review in Claude Code, he can now just say "Take all recommendations" and trust the output. A real signal on how much reasoning quality has leveled up. https://x.com/garrytan/status/2088388000267002195


*Matt Turck* — VC at FirstMark Capital, host of the MAD Podcast

Turck captured the new texture of an AI-era workday in a single post: before AI, your day is filled with alternating decisions and manual process, and you're still going at 10pm. With AI, it's decision, decision, decision, decision — and by 3pm, brain empty, staring at the wall. The work volume has collapsed, but the cognitive density has spiked. https://x.com/mattturck/status/2088323186819539041


*Nikunj Kothari* — Partner at FPV Ventures

Kothari flagged that Claude Code's `/goal` command isn't the most token-efficient tool, but he found it remarkable to watch it one-shot an extremely detailed spec — with generous CLI tools — over a 14-hour run. https://x.com/nikunj/status/2088351343434138111


*Peter Steinberger* — Co-founder at OpenClaw (OpenAI)

Steinberger shared two workflow upgrades for their team. First, they added a simple instruction to their shared `AGENTS.md` file requiring video uploads for every PR that changes UI state — a low-cost way to make visual regressions visible at review time. https://x.com/steipete/status/2088486859244741020

Second, the team has fully moved to building OpenClaw with OpenClaw. He called the ability to share agent sessions as URLs "a superpower." https://x.com/steipete/status/2088473882357530979


*Dan Shipper* — CEO of Every

Shipper pushed back on the assumption that AI-native companies must be in a constant fundraising cycle and market share death match. His contrarian take: you can build an AI-native rocketship on very different terms — but the rules for doing so are different. https://x.com/danshipper/status/2088270756043993503

He's also recruiting for Thesis 2027, an event for people using AI in ways that make everyone around them feel slightly behind — executives, builders, and creatives who are operating at a different level. https://x.com/danshipper/status/2088298533912989736


*OFFICIAL BLOGS*


*Claude Blog: Building intelligent apps for Apple platforms with Claude in the Foundation Models framework*

Anthropic released a new Swift package that lets Apple developers call Claude through Apple's Foundation Models framework — bringing Claude into the same workflow that powers on-device features across iOS, iPadOS, macOS, visionOS, and watchOS (all on their 27-series releases).

The integration is designed for handoff: Apple's on-device models handle fast, local tasks like summarization and extraction using typed Swift values from `@Generable` annotations. When a request calls for multi-step reasoning, code generation, web search, or data analysis, the framework hands off to Claude — and streams the response back into the same SwiftUI view.

The practical unlock: a journaling app can generate daily prompts on-device, then ask Claude to find threads across months of entries. A study app can define a term locally, then hand off to Claude when a student asks "why does this matter for everything else we've covered?" One experience, backed by the right model at each step.

Developers add the package, authenticate with an Anthropic API key, and pass typed outputs from Apple's on-device models into a Claude request. The package handles streaming, tool calls, and structured responses.

<https://claude.com/blog/claude-for-foundation-models|Read the full post>


*PODCASTS*


*The MAD Podcast with Matt Turck: How to Build Long-Horizon AI Agents — Mitch Troyanovsky, Basis*

*The Takeaway:* Passing 100 evals is a starting point, not a guarantee — and the quality of your English context matters more than the quality of your code.

Mitch Troyanovsky is the co-founder of Basis, a unicorn AI company whose agents run autonomously for hours — sometimes days — and can complete complex tasks like end-to-end tax return preparation. The conversation is a dense, practical reference on what it actually takes to build agents that work in the real world.

His framing of long-horizon agents starts with a simple analogy: LLMs have enormous working memory but, by default, no short-term or long-term memory. He compares it to the protagonist in the film _Memento_ — someone who wakes up every day knowing who they are, but with no memory of recent events. To make progress toward any goal, they have to write things down for themselves and reconstruct their state each day. That's what well-designed agent harnesses do: they compensate for context rot by giving agents structured ways to maintain coherence over time.

On evals, Troyanovsky is blunt: "Let's say you have 100 evals. Great. They all pass. Are you confident that generalizes to the real world? Our answer has been no. Even if you got it right 100 out of 100 times, if a person is just going to Wikipedia, the accounting firm wouldn't hire them, and so they shouldn't hire us either." Real production evals need to test for the quality of reasoning, not just whether an answer was technically correct.

On what actually affects agent performance: "You'll see people freaking out over a code file that isn't abstracted properly, and yet their context is total shit. The English is more precious because the English affects the performance. The code does not affect the performance." His team uses directional microphones to whisper context to their agents — spoken input is faster and richer than typed, and agents don't need you to clean up your thoughts the way a Slack message would.

On autonomy: he's careful to distinguish between "done" and "unreviewed." True autonomous agents shouldn't hand you a 1,000-line PR with "trust me." They should deliver their output the way a good junior engineer delivers a clean PR stack — with clear reasoning, explicit assumptions, and easy-to-review diffs. Autonomy is about quality of hand-off, not absence of review.

The model breakthrough that changed everything for him: Opus 3, which was the first model that could genuinely understand content at long context windows. Then o1 for reasoning. Then o3 for showing that reasoning quality could scale with better training — each token of inference-time thinking becoming more efficient and higher-quality.

https://www.youtube.com/@DataDrivenNYC/videos


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
