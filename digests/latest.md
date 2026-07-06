*AI Builders Digest — July 6, 2026*


*X / TWITTER*

*Thibault Sottiaux, Codex & ChatGPT PM at OpenAI* — crowdsourced a sharp question directly to users: "What is something that you feel is surprising that Codex still can't do well and we should have gotten right a while ago?" — 1,969 replies poured in. Also shared a funny interaction with an AI (Sol) that insisted on tracking a "332-salute debt" after some emoji math, closing with: "The salute economy is ruthless."
- <https://x.com/thsottiaux/status/2073551549494596079|Codex feedback thread>
- <https://x.com/thsottiaux/status/2073554978053005607|Salute economy>

*Cat Wu, Claude Code & Cowork PM at Anthropic* — praised Claude Fable 5 for proactively applying propensity score matching in a retention analysis without being asked — matching users on activity levels for a fair like-for-like comparison. "It's exciting to see Fable 5's improved judgment across all of its work, from writing emails and docs in Cowork to debugging complex errors in Claude Code."
<https://x.com/_catwu/status/2073439890482794966|Tweet>

*Guillermo Rauch, Vercel CEO* — shared an animated visualization of the token spend race from Vercel AI Gateway, which aggregates trillions of tokens from millions of developers monthly. Key observations: Anthropic's dominance, fluctuations among labs, and the rise of open-weight AI.
<https://x.com/rauchg/status/2073563586270781674|Token spend race>

*Nan Yu, Head of Product at Linear* — riffed on AI coding accountability: "If you drop every production table does the model get fired or do you get fired." Separately made a sharp point about code review in the AI era — you find bugs by using the product and trying to break it, not by reading code. Code review is now about architecture and API design, not bug hunting.
- <https://x.com/thenanyu/status/2073410944969932877|Model accountability>
- <https://x.com/thenanyu/status/2073410299680428445|Bug-finding philosophy>

*Peter Steinberger, OpenClaw co-founder (OpenAI)* — teased an upcoming OpenClaw feature that shows users exactly when their Claude token resets expire, helping them time usage to maximize value.
<https://x.com/steipete/status/2073482942513565713|Tweet>


*OFFICIAL BLOGS*

*Claude Blog: "Building intelligent apps for Apple platforms with Claude in the Foundation Models framework"*

Anthropic released a Swift package that integrates Claude into Apple's Foundation Models framework, letting iOS/macOS developers call Claude directly from Swift. Apple's framework already handles fast on-device tasks (summarization, extraction) in 3 lines of code — the new package hands off to Claude when a request needs multi-step reasoning, code generation, web search, or code execution. Because Apple's framework returns typed Swift values via @Generable annotations, developers arrive at the Claude API call with clean, structured inputs rather than raw user text. Works on iOS 27, iPadOS 27, macOS 27, visionOS 27, and watchOS 27.
<https://claude.com/blog/claude-for-foundation-models|Read the full post>


*PODCASTS*

*The MAD Podcast with Matt Turck: "Cloudflare CEO: The Internet's Business Model Is Dead"*

*The Takeaway:* Bot traffic has already overtaken human traffic on the internet in 2026 — and the 28-year-old advertising model powering the web can't survive bots that don't click ads.

Matthew Prince, co-founder and CEO of Cloudflare, delivers a stark diagnosis: AI agents that make users 1,000x more efficient are also exposing how fragile internet economics really are. When an agent shops for a digital camera, it visits 5,000 sites instead of 5 — a thousand-fold surge in infrastructure demand with zero ad revenue to show for it. "Over the next five years, the business model of the Internet is gonna change radically."

Prince sees Cloudflare positioned at the center of rebuilding that model. Cloudflare Workers — built originally out of internal necessity — is now the efficient compute layer for agentic workloads, using browser-style isolates instead of containers (potentially 40x more efficient). AI Gateway provides enterprises with audit trails, prompt guardrails, and intelligent model routing across providers. And on the monetization side, Cloudflare is working with Coinbase, Stripe, and the long-dormant HTTP 402 ("Payment Required") protocol to enable micropayments for AI bot access to content — targeting 10–100 million financial transactions per second, orders of magnitude beyond what Visa handles today.

On internal AI adoption: 93% of Cloudflare's R&D team uses AI coding tools. Prince cut 20%+ of the workforce — not for performance reasons, but because middle-management and measurement roles were made redundant. His warning is direct: mid-career professionals who resist AI tools are the most exposed. "You can't have one person who is 100 times as productive in the same role as somebody else making the same amount of money."

<https://www.youtube.com/watch?v=UN47z_opfmo|Watch on YouTube>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
