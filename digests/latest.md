AI Builders Digest — August 23, 2026

*X / TWITTER*

*Thibault Sottiaux* (Codex & ChatGPT at OpenAI, thsottiaux on X) shared a transparency update on Codex rate limits. The team found three issues: inefficiencies when using images in long sessions with multiple compactions, high p95+ usage for the Computer History feature, and a conversation-title generator draining more usage than intended. A tiger team is shipping fixes, and all paid subscriptions will receive a full usage reset. He also teased a novel efficiency improvement unrelated to the bugs — coming the following week.
<https://x.com/thsottiaux/status/2091407991736332689|View tweet>

*Peter Yang* (AI tutorial creator, petergyang on X) shared a privacy tip: open myaccount.google.com/permissions in Chrome, then use Codex or Claude Code to audit and remove apps that shouldn't still have access to your Google data. He also announced he's building a new AI skill called /fuck-cancer — aimed at helping cancer patients and families navigate treatment and stay informed — and is crowd-sourcing what to include. Separately, he noted that Instinct now lets users delete externally imported data (like Gmail records) from the Data Privacy section, crediting the team for shipping it quickly after feedback.
<https://x.com/petergyang/status/2091331251211059468|Privacy tip> · <https://x.com/petergyang/status/2091239339204415969|/fuck-cancer skill> · <https://x.com/petergyang/status/2091187611507499321|Instinct data privacy>

*Madhu Guru* (Sr. Director of AI at Meta, realmadhuguru on X) continued his series on building great evals. In Part 6, he defines "hill climbing on evals" as picking one dimension that matters — quality, cost, or latency — and systematically improving it using better harnesses and model selection (prompt engineering, context engineering, memory, post-training, or deterministic code). His failure mode taxonomy from Part 3 serves as the compass. Example: if tool-calling failures are your biggest issue and you're stuffing 20 tools into context when each task only needs 3-5, context engineering is your hill to climb. On cost reduction: launch with the best model first to nail quality, then hill climb down to a smaller, cheaper, faster model once users love the experience.
<https://x.com/realmadhuguru/status/2091278653435072523|Part 6 tweet>

*Aaron Levie* (CEO of Box, levie on X) made a pointed argument about enterprise AI adoption: diffusion is rate-limited more by evals than most realize. Model-release benchmarks tell you about general progress and relative capability, but the bigger unlock is building evals for the specific workflows a company runs — down to individual company processes. "You can't automate what you can't assess the progress on. Enterprises will not be able to go just on vibes."
<https://x.com/levie/status/2091359223368315050|View tweet>

*Zara Zhang* (builder, zarazhangrui on X) shared two sharp observations. First: talented individuals can hit 10x their potential with AI when working on their own thing, but in a large organization the same person might only see a 20% gain (sometimes even negative). She sees this as a key driver behind more talented people leaving big companies — with AI labs being the main exception. Second observation: "Everyone who's ahead in using AI thinks they're behind."
<https://x.com/zarazhangrui/status/2091379220257603593|AI amplification tweet> · <https://x.com/zarazhangrui/status/2091338374447763481|"Everyone who's ahead">

*Nikunj Kothari* (partner at FPV Ventures, nikunj on X) called out a troubling fundraising pattern: founders rage-baiting investors on Twitter and then sending SAFE docs to "just wire money" is not how investing works. In follow-up context, he stressed how important it is for young builders to find the right people to take advice from, and expressed frustration at talented founders playing engagement games instead of building substance.
<https://x.com/nikunj/status/2091381756012511244|View tweet>

*Amjad Masad* (CEO of Replit, amasad on X) kept it brief: "A week has 7 days. That means 7 ships." — a nod to Replit's shipping velocity. He also dropped a self-aware aside: "'Pretty soon' turned out to be 3 months."
<https://x.com/amasad/status/2091346778746757204|7 ships> · <https://x.com/amasad/status/2091217410615644349|Pretty soon>


*PODCASTS*

*AI & I by Every — "Microsoft's Vision for an Internet Made for Agents With CTO Kevin Scott (Best of the Pod)"*

_The Takeaway:_ The real infrastructure work of this AI era isn't better models — it's building the open protocols and identity systems that let agents actually take action in the world, the same way HTTP and HTML built the web.

Kevin Scott has spent four decades in software, currently as CTO of Microsoft, and he brings unusual perspective: he's a potter, a woodworker, a Vi devotee who still refuses to switch editors despite building VS Code. His core argument is that AI is stuck in a "capability overhang" — model reasoning has outpaced what products deliver to users. The fix isn't more scaling; it's plumbing.

Scott points to MCP (Model Context Protocol) as the HTTP of the agentic internet — a simple, open protocol that lets agents talk to external systems without companies shipping their org chart to users. He's pushing internally for all Microsoft systems to speak a standard agent protocol, to avoid the classic Conway's Law problem: your architecture mirrors your org structure.

On security, he doesn't pretend to have all the answers, but argues MCP's simplicity makes the right security model tractable: agents need identities, entitlement systems, and a way to request permissions from users before touching systems. "Let's do it in an open way. We don't need it to be proprietary."

His take on AI and craft: developers worrying that agents will kill the joy of coding are echoing debates he's heard his whole career — hand tools vs. power tools vs. CNC in woodworking, VI vs. modern editors in programming. His advice: "Be curious. Try stuff. And if it works for you, use it. And if it doesn't, don't." He waited too long to learn 3D printing and regrets it.

His prediction for next year: the shift from synchronous AI (prompt and wait) to asynchronous (delegate, let it run, check back) will feel obvious in hindsight. And anyone still waiting for AI to get "cheaper" or "more capable" before starting will be far behind.

<https://www.youtube.com/playlist?list=PLuMcoKK9mKgHtW_o9h5sGO2vXrffKHwJL|Watch on YouTube>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
