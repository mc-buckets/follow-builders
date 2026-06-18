*AI Builders Digest — June 18, 2026*


*X / TWITTER*

*Josh Woodward — VP at Google Labs, GeminiApp, and GoogleAIStudio*
Google officially expanded its AI Futures Fund to Brazil, partnering with Monashees to launch the Gama Fund. The program targets deep tech founders with early access to Google DeepMind models, up to $2M in co-investment, $350k in Google Cloud & Gemini credits, and direct co-development with Google engineers at a new IPT Open campus hub. Applications are open now.
https://x.com/joshwoodward/status/2067025851829330076

*Thibault Sottiaux — Codex and ChatGPT at OpenAI*
A mini-saga played out: Codex hit widespread "model at capacity" errors overnight. Sottiaux acknowledged the issue, then confirmed a fix with rate limits being reset across all plans — and a teaser: "You know what's coming 👀." Shortly after, posting from France, he announced the most exciting Codex features are rolling out across Europe.
- https://x.com/thsottiaux/status/2066865154902380796
- https://x.com/thsottiaux/status/2066956441173323943
- https://x.com/thsottiaux/status/2067064381855187231

*Peter Yang — AI newsletter creator with 150K+ readers*
Yang is publishing a tutorial on turning Codex or Claude Code into a personal advisor using just 4 files — and managed to save Fable's advice before it got restricted. He also voiced skepticism about an unnamed product launch ("this is what happens when nobody internally wants to tell the CEO no") and lamented another round of large-company layoffs.
- https://x.com/petergyang/status/2067056979974160749
- https://x.com/petergyang/status/2067047343971848201
- https://x.com/petergyang/status/2066975504973050077

*Madhu Guru — Former Product Leader at Google (Gemini, Veo, Nano)*
On the SpaceX-Cursor deal: Madhu argues the real prize isn't the IDE — it's Cursor's production-grade agentic harness (planning, context management, tool use, iteration, memory, error recovery). "Very few companies do even one of these well. Cursor brings all three," referring to the harness, full AI stack expertise, and end-to-end product lifecycle focus. He also made a philosophical point: humanity over-indexed on intellect as the defining human trait, under-investing in self-awareness, intuition, and compassion — and the next few years of AI will force a reckoning with that.
- https://x.com/realmadhuguru/status/2066935654500671499
- https://x.com/realmadhuguru/status/2067090477434966396

*Thariq — Claude Code at Anthropic*
Excited: Slack now renders HTML attachments inline instead of displaying them as raw text.
https://x.com/trq212/status/2067021344341098670

*Amjad Masad — CEO at Replit*
Replit won Databricks partner of the year.
https://x.com/amasad/status/2066956074360426622

*Guillermo Rauch — CEO at Vercel*
Vercel is shipping. The latest update adds 24-hour sandbox lifetimes on top of existing 30-minute function invocations, teased with a simple "It's time to ship."
- https://x.com/rauchg/status/2067106499449565265
- https://x.com/rauchg/status/2067137678772937000

*Aaron Levie — CEO at Box*
Two substantive takes. On the Cursor acquisition: Levie calls it "the first mega success in the applied layer of AI" and a template for applied AI execution — deep domain focus, acting as model router, knowing when to use frontier models vs. train your own, and GTM discipline in a competitive space. "Every aspect of their business was tuned to carve out ground and keep doubling down."
https://x.com/levie/status/2066908002809221496
Second, a market structure analysis: the biggest unresolved question in AI is whether open weights models stay 3–6 months behind frontier or fall years behind. That gap determines everything — chip stack, sovereign AI strategy, inference location, margin structures, and enterprise AI spend.
https://x.com/levie/status/2067070918300664161

*Ryo Lu — Designer at Cursor*
On Cursor mobile: much of the real app was coded by a designer using Cursor itself — "titles don't mean shit. you can just build." Also riffed on the SpaceX-Cursor deal: "crazy idea: what if X, Cursor, were the same thing?"
- https://x.com/ryolu_/status/2067124871226929526
- https://x.com/ryolu_/status/2066902677905461579

*Garry Tan — President and CEO at Y Combinator*
Shared contrarian encouragement: "You'll never achieve anything if you are afraid of being cringe." Also posted on Bowen's theory of differentiation of self — self-abandoners and bullies are both the same underlying pattern (low differentiation), and the fix is building the capacity to stay a distinct self under pressure.
- https://x.com/garrytan/status/2067101283493040518
- https://x.com/garrytan/status/2067100549775032702

*Zara Zhang — Builder*
Two sharp takes. First, a product manifesto on AI differentiation: "Every other product right now is 'an AI agent that does everything in your work & life & integrates with everything.' Cool, that's just Claude/Codex. If you want me to use your thing instead, it needs an opinion & a soul. Build small & sharp, not big & generic. Doing everything means doing nothing."
https://x.com/zarazhangrui/status/2066936706281206165
Second: don't chase what's already labeled "cool" — go so deep on something everyone else ignores that it becomes the cool thing.
https://x.com/zarazhangrui/status/2066994434953421226

*Nikunj Kothari — Partner at FPV Ventures*
Brief but pointed on the Cursor acquisition: "Be in the judgement (data) path or the token path. Today's cursor_ai acquisition sets the path for more application companies." Also attended Cursor Compile and noted custom mechanical keyboards are "a new kind of swag ceiling for conferences."
- https://x.com/nikunj/status/2066905445974102384
- https://x.com/nikunj/status/2066966270197805331

*Dan Shipper — CEO at Every*
Switched back from Atlas Browser to Dia after too many bugs with Atlas and no signs of improvement.
https://x.com/danshipper/status/2066914130863473048

*Aditya Agarwal — General Partner at SouthPk Commons, Co-Founder of Bevel Health*
Snowflake CEO Sridhar Ramaswamy — who grew Google's ad business from $1.5B to $100B+ — is visiting SouthPk Commons next week.
https://x.com/adityaag/status/2066915803610370098


*OFFICIAL BLOGS*

*Claude Blog — <https://claude.com/blog/claude-for-foundation-models|Building intelligent apps for Apple platforms with Claude in the Foundation Models framework>*

Anthropic released a Swift package that lets Apple developers route to Claude from within Apple's Foundation Models framework. The framework already returns typed Swift values from on-device models; the package extends that to hand off to Claude for multi-step reasoning, code generation, web search, and code execution when the on-device model isn't enough — all within the same SwiftUI view.

The design pattern: a journaling app generates daily prompts on-device, then asks Claude to surface threads across months of entries. A study app explains a concept locally, then hands off to Claude for deeper follow-up questions. "It's one experience for the user, backed by the right model for each step."

Works on iOS 27, iPadOS 27, macOS 27, visionOS 27, and watchOS 27. Add the package, sign in with an Anthropic API key, and pass typed outputs from Apple's on-device models directly into a Claude request.

https://claude.com/blog/claude-for-foundation-models


*PODCASTS*

*Training Data — "Simulating Humans at Scale: Simile's Joon Sung Park"*

_The Takeaway:_ The real bottleneck in behavioral AI isn't raw model capability — it's the gap between what people _say_ and what they actually _do_, and current frontier LLMs are almost entirely trained on the former.

Joon Sung Park is the founder and CEO of Simile, and previously a Stanford researcher whose 2023 "Smallville" project went viral for creating a town of 25 AI agents who spontaneously planned and threw a Valentine's Day party. That research has since become a company serving Fortune 500 clients — including CVS — with behavioral simulations grounded in real survey and interview data.

The counterintuitive insight: today's frontier LLMs may actually be getting _worse_ at simulating humans as they improve. As labs optimize toward rational, objective-answering "superintelligent" machines, they diverge further from the messy, irrational diversity of real human behavior. Park argues a separate class of model is needed — not a CPU of intelligence, but a GPU: massively parallel units each representing the actual values, preferences, and lived stories of real subpopulations.

Simile's method: partner with Gallup, collect 15 minutes of behavioral and biographical data from real people ("Just tell me the story of your life"), then build agents that can answer questions far beyond the original survey domain. CVS uses it to model second-order market effects of product decisions. Some clients simulate their earnings calls before they happen. Validated accuracy: 85% as close as people replicating their own responses.

On the bigger horizon: Park sees a future where a single simulation might cost $100M and take months to run — but answer one of civilization's fundamental open questions. "Simulation can be [to social sciences] what the Hubble Telescope was to understanding the universe."

https://www.youtube.com/watch?v=lfhFmwcESRw


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
