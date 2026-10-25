AI Builders Digest — October 25, 2026

*X / TWITTER*

*Thibault Sottiaux* (Codex & ChatGPT, OpenAI)

Sottiaux dropped a quote that's already making the rounds: _"The difference between having a tool and being a tool is subtle these days and it's easy to accidentally build yourself into being a tool. Don't be a tool."_ (4,375 likes, 208 RTs — clearly struck a nerve.)
<https://x.com/thsottiaux/status/2113838156193894447|View tweet>

On the product side, he shared Day 19 OpenAI DevDay updates: calls connect faster in Dots, changing reasoning mid-conversation in Codex no longer invalidates cache, and the Codex CLI has been updated.
<https://x.com/thsottiaux/status/2113770573994299544|View tweet>

Codex CLI specifically got reusable prompt presets, inline model and permission settings, enterprise MCP sign-in, fixes for long session resume failures, and Windows corporate-proxy authentication. Usage has *2X'd* since DevDay.
<https://x.com/thsottiaux/status/2113770862860222611|View tweet>

*Thariq* (formerly Claude Code, Anthropic)

Big news: Thariq announced he's leaving Anthropic after more than a year working on Claude Code — watching it "scale larger than I ever imagined." He spoke warmly about the mission and his colleagues ("the most talented, thoughtful, competent, and earnest people I have ever met") and said he's taking a break before diving into something new. He recommended following addyosmani, lydiahallie, _catwu, ClaudeDevs, and bcherny for ongoing Claude Code content.
<https://x.com/trq212/status/2113844051938054167|View tweet>

*Amjad Masad* (CEO, Replit)

Two big announcements: Replit is acquiring the Chroma team — the vector database pioneers who were "building RAG before it was even a thing." They'll work on agent memory and context, which Masad called "one of the hardest problems in AI." He framed it as a step toward the "self-driving company."
<https://x.com/amasad/status/2113736007111827606|View tweet>

Also: Replit for Government is now a thing, with Michael Greenwald (ex-AWS public sector lead) joining to help transform how governments build software.
<https://x.com/amasad/status/2113676717105787192|View tweet>

*Guillermo Rauch* (CEO, Vercel)

Rauch broke down a newly-publicized OpenAI finding: agents can run "Ouija"-style timing attacks on co-hosted VMs — detecting other agents on the same machine by measuring CPU cache timing. This class of attack has been known since 2015 with no complete fix; the only real solution is dedicated hardware per agent, which has major economic consequences. Vercel Sandbox has deployed all practical mitigations available.
<https://x.com/rauchg/status/2113759533801877920|View tweet>

*Aaron Levie* (CEO, Box)

Levie is bullish on agent swarms for cyber defense becoming "one of the biggest categories in AI." His core argument: security is perfect for swarms because more compute directly equals more value — there's an endless backlog of testing humans never get to, and agents can run it continuously. "Going to be a wild time in cyber."
<https://x.com/levie/status/2113738768645808277|View tweet>

*Zara Zhang* (Builder)

Hosting a personal website building event in San Mateo on November 7 (Saturday). No coding or design experience required — beginners preferred. They'll showcase cool personal sites and help attendees build or rebuild their own.
<https://x.com/zarazhangrui/status/2113676956885807406|View tweet>

*Nikunj Kothari* (Partner, FPV Ventures)

Quick note that Anthropic hit 10X revenue growth even without launching Claude Duet — suggesting Duet could be additive upside from an already strong base.
<https://x.com/nikunj/status/2113785018497831076|View tweet>

*Dan Shipper* (CEO, Every)

Offered a crisp take on team structure for AI companies: the ideal is two types of people — pirates and architects. No further explanation, but the framing has legs.
<https://x.com/danshipper/status/2113693510629281895|View tweet>

*Aditya Agarwal* (General Partner, SPC)

Shared a clip from a conversation with Sergey Levine (physical intelligence researcher): the biggest AI advances have come from solving many problems together, not training specialized systems for individual tasks. The principle applies equally to robotics — make the problem bigger.
<https://x.com/adityaag/status/2113666947766169868|View tweet>

*Claude AI* (Anthropic)

Linked to a deeper look at how Claude Duet handles safety, privacy, and security.
<https://x.com/claudeai/status/2113736176737845353|View tweet>

*PODCASTS*

*No Priors — "Democratizing Security for the Agentic Web with Cloudflare CTO Dane Knecht"*

_The Takeaway:_ AI is creating a vulnerability apocalypse — Log4j-level security events now happen weekly, not yearly — but AI is also the best tool we have to fix it.

Cloudflare CTO Dane Knecht has a front-row seat to how fast the security landscape is deteriorating. Under his watch, Cloudflare is seeing major vulnerabilities reported at exponential frequency, driven not just by nation-states but by "agent kitties" — high school kids pointing AI agents at systems the same way earlier generations ran capture-the-flag contests.

His most counterintuitive claim: AI-generated code is actually making security *worse* in the short term. "AI, at least the early AI, is very verbose. It likes to create complexity. So AI in a sense of what we've been dealing with is actually not been helping build more secure stuff right now." His fix: start from first principles — reduce attack surface area, simplify code, let security get baked into the development lifecycle automatically.

Knecht predicts more than half of engineering time across the industry will go toward security over the next 18 months. Cloudflare is responding by expanding from one red team to four or five. His philosophy: focus resources on *discovery*, and engineers will figure out how to patch at scale when volume forces their hand.

On the agent-driven internet economy, Knecht sees a parallel web emerging — one for humans, one for machines. He's excited about Cloudflare's content monetization gateway (microtransactions for AI agent access to content), a collaboration with OpenAI called "signals" to help agents discover new content without constant crawling, and the X402 payment standard Stripe revived from a dormant HTTP error code Tim Berners-Lee created decades ago.

One wild stat: Cloudflare hired 1,000 interns this year for a 5,000-person company. The reasoning — managers who worked with AI-native interns adopted AI faster themselves, and the intern energy drives bottoms-up workflow reinvention at a pace no consulting firm could match.

<https://www.youtube.com/@NoPriorsPodcast|No Priors Podcast>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
