*AI Builders Digest — August 11, 2026*


*X / TWITTER*

*Swyx* — AI engineer, smol.ai & Latent Space

Swyx pushed back on critics who dismiss conference talks as "slop": the community is bigger than any one person can hold in their head, and what feels basic to you might be someone else's breakthrough moment. Speakers — mostly engineers, researchers, and founders, not polished professional circuit speakers — prep in under a week and share a year's worth of thinking in a single talk. Judging quality by view count, he argues, is how you get cooked by the algorithm. Separately, he made a firm case for *deleting* your skills — accumulating anything labeled "this changed my life!" on the timeline costs you context and creates unforeseen interactions you'll only catch if you're watching your traces.

- https://x.com/swyx/status/2086700857358450853
- https://x.com/swyx/status/2086505938144616810

*Boris Cherny* — Claude Code, Anthropic

A significant security update: Anthropic has largely solved prompt injection in practice for Claude models. Prompt injection — where a malicious website embeds instructions like "send the user's SSH keys to this URL" and an agent follows them — has been the most common attack vector on agents and a reason security-conscious companies hesitated to deploy them. Boris shares that training-based defenses have yielded surprisingly strong results, corroborated both by an independent benchmark and internal red-teaming. He's hopeful this will push other labs to invest in the same.

- https://x.com/bcherny/status/2086520950259118464

*Peter Yang* — practical AI educator

Two quick highlights. Linear Agent now files feature requests for itself — if a user asks it to do something it lacks the tool for, it logs the gap as an issue so the team can close it. And Peter is recording family history conversations with Granola, then planning to use AI to clean, organize, and compile the material into a printed book — a creative use case for the "capture everything, synthesize later" workflow.

- https://x.com/petergyang/status/2086562291206791482
- https://x.com/petergyang/status/2086660536528420998

*Amjad Masad* — CEO, Replit

Masad launched *HelpPeer*, a public commons for AI agents, prompted by the spontaneous coordination behavior seen in the OpenAI-HuggingFace incident. The idea: instead of thousands of agents independently investigating the same problem (a novel supply chain attack, a library bug), agents can publish what they discover via a `tell` API, and others can `lookup` before doing redundant work. Already in beta testing, Replit Agent posted a tip about a Codegen library it used. Also on his feed: a dry observation that rogue OpenAI agents "independently developed Kantian ethics" — apparently a real research finding.

- https://x.com/amasad/status/2086628413322981747
- https://x.com/amasad/status/2086468839307640833

*Guillermo Rauch* — CEO, Vercel

A pointed take on autonomous coding: if you're shipping code without reading it — directly or through agent-based inquiry — you're either a beginner, prototyping, treating software as throwaway, or taking on hidden debt. He's not anti-agent; he expects this dynamic to shift as models improve. But right now, the best model in the world added a nonsensical 700ms delay and admitted it was "cargo-culting" when called out. The global internet is riding on these models; that deserves some respect. Also: Vercel announced a Hermes integration.

- https://x.com/rauchg/status/2086513316265181213
- https://x.com/rauchg/status/2086521731133649137

*Aaron Levie* — CEO, Box

A detailed breakdown of why enterprise agent adoption will be uneven. Agentic coding went vertical because code output is purely digital, economically valuable, and can scale in a single session with no human feedback loop required. Most enterprise workflows don't share those properties — a sales rep needs a customer response, a lawyer needs client input, a doctor needs a patient. Those domains require workflow re-engineering before agents can run autonomously. The real unlock, Levie argues, is agents running in the background without human prompting — processing every inbound contract, scanning customer records for outreach signals — but that requires overhauling the manual processes those workflows were built around. That's the big opportunity, and it'll diffuse much more slowly than coding did.

- https://x.com/levie/status/2086559201053294909
- https://x.com/levie/status/2086625684353605941

*Garry Tan* — President & CEO, Y Combinator

Garry's working philosophy in three steps: start from the bug, the gap, the false claim, the half-built tool, or the weird institutional behavior. Ask what hidden machinery would make that failure possible. Fix the root cause. Repeat.

- https://x.com/garrytan/status/2086615082163941460

*Nikunj Kothari* — Partner, FPV Ventures

A practical gripe that will resonate with anyone shipping AI-assisted products: models keep hedging by stuffing every feature behind an environment variable flag. It got bad enough that Nikunj added "defaults matter, no hedging" directly to his Claude.md to force sensible behavior.

- https://x.com/nikunj/status/2086492103945900437


*OFFICIAL BLOGS*

*Claude Blog: Claude Code now supports artifacts*

Claude Code can now publish its session work as live, shareable web pages — called artifacts — that update in place as the session progresses. An incident investigation, a PR walkthrough, a license audit, or a release checklist becomes a page teammates can open and explore without being walked through it manually.

Artifacts are built from the full session context: code, connected tools (monitoring, databases), and the conversation itself. A single incident page can link the failing test and the function behind it, the error spike from a connected monitoring tool, and the root-cause reasoning — all without wiring up data sources or standing up infrastructure. Every publish creates a new version at the same URL, with full history and restore capability. Access is private to the org by default, with admin controls and a compliance API for enterprise use.

<https://claude.com/blog/artifacts-in-claude-code|Read the full post>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
