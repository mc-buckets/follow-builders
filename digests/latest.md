AI Builders Digest — November 4, 2026

*X / TWITTER*

*Swyx* — smol.ai / Cognition / Latent Space

Swyx is riffing on "weight-space programming" — the emerging idea that you can directly manipulate model weights rather than just prompting. He drew a literary parallel to Ted Chiang's _Exhalation_, saying we're at paragraph two of that story. He's also teeing up what he promises will be a "melt on Twitter" follow-up conversation with CompleteSkeptic and typesafeai.

- <https://x.com/swyx/status/2117492548780589510|Weight-space programming post>
- <https://x.com/swyx/status/2117331535007531009|Upcoming conversation teaser>

*Thibault Sottiaux* — Codex & ChatGPT at OpenAI

The OpenAI Codex team is now talking publicly about Git capabilities they've been building. Sottiaux also highlighted that ChatGPT's "dot" is now routing tasks across different models automatically — choosing the best model for each part of the work rather than locking users into a single one.

- <https://x.com/thsottiaux/status/2117412956950638872|On Codex Git capabilities>
- <https://x.com/thsottiaux/status/2117283355427495983|On dot's model routing>

*Peter Yang* — AI tutorials and guides

Peter Yang ran a head-to-head writing experiment: Gemini's copy-editing suggestions were "actually great" while ChatGPT's were "almost entirely bad." His frustration: Antigravity (ChatGPT's canvas tool) lacks working browser use, so he has to manually copy Gemini's edits back in. His take — the best writing model is being held back by its harness, not its intelligence.

- <https://x.com/petergyang/status/2117333424403042330|On Gemini vs ChatGPT for editing>
- <https://x.com/petergyang/status/2117473529797214279|On AI-native product growth>

*Nan Yu* — Product at OpenAI Codex (prev Head of Product at Linear)

A sharp take: group chat is a fundamentally broken interface for multiplayer AI. Nan's framing — it's "literally guaranteed slop" except in rare circumstances. Coordinating multiple people around a single AI context creates noise, not signal.

- <https://x.com/thenanyu/status/2117432599559716940|On group chat and AI>

*Thariq* — Formerly Claude Code at Anthropic

One week into using his own setup: the $200/month plans are "amazing" and you don't need unlimited tokens to do great work. His most striking line: "this is the most expensive intelligence will ever be." He's betting hard on falling costs.

- <https://x.com/trq212/status/2117305792923889731|On AI plan value and intelligence costs>

*Replit CEO Amjad Masad*

Two sharp posts from Amjad. First, a principled take on AI agent security: agents should run in dedicated, org-controlled environments with minimal permissions for each task — not given the keys to everything. Second, a warning shot to AI use in finance: "the ban hammer is coming down."

- <https://x.com/amasad/status/2117499074496872882|On AI agent security>
- <https://x.com/amasad/status/2117481616943820843|On AI in finance>

*Vercel CEO Guillermo Rauch*

Bullish on WebMCP — the emerging standard for connecting web apps to AI agents. His bigger argument: stateless sandboxes are the wrong benchmark for agents. Agents need their full workspace — identity, skills, repos, memories — not a fresh empty box every time. He called out Vercel's Sandbox team for shipping 19 global regions, double-digit weekly growth in demand, and consistent SLO performance while pushing new features weekly.

- <https://x.com/rauchg/status/2117419661654720671|On WebMCP>
- <https://x.com/rauchg/status/2117338179535810957|On stateful agent sandboxes>

*YC President & CEO Garry Tan*

Garry's been using Capy Captains — a multi-agent coordination tool — and says it increased his issue-fixing throughput 5X overnight. The unlock: coordinating across captains and subthreads. He also flagged an interesting use of smaller models: direct weight manipulation. On the policy front, he's pushing hard for CEQA repeal, calling it the "primary NIMBY tool" blocking hospitals, high speed rail, and housing in California.

- <https://x.com/garrytan/status/2117410016730964358|On Capy Captains productivity>
- <https://x.com/garrytan/status/2117384926052135106|On weight manipulation with smaller models>
- <https://x.com/garrytan/status/2117274654981452000|On CEQA repeal>

*Nikunj Kothari* — Partner at FPV Ventures

Nikunj is launching a new invite-only SF event series called *Slice for Thought* — 60-minute sessions where he interviews an expert for 45 minutes, then the guest gets to interview him back. First guest: Peter Walker, head of insights at OpenRouter. Wednesday, Nov 4, noon, 10–12 people, pizza included, all off the record. He also dropped a sharp VC observation: the median pipeline from "vague posting revenue numbers" to a fundraise kickoff is about 11 days (n=17).

- <https://x.com/nikunj/status/2117413490256433207|On Slice for Thought event series>
- <https://x.com/nikunj/status/2117362283223687621|On startup fundraise pipeline timing>

*Dan Shipper* — CEO at Every

Dan is bullish on Argon (a new Claude model) — linking to Every's vibe check review of it. His read: Argon is so good that Antigravity (ChatGPT) looks stuck in 2025 by comparison, missing the latest capabilities. He's letting the quality differential speak for itself.

- <https://x.com/danshipper/status/2117428596688171450|Linking to Every's Argon vibe check>
- <https://x.com/danshipper/status/2117363007340609556|On Argon vs Antigravity>

*Aditya Agarwal* — General Partner at SPC (prev CTO at Dropbox)

SPC alumni highlight: Tankots (Tomas Reimers), four-time founder and IOI medalist, is joining SPC's speaker series Nov 12. His company WisprFlow just raised a $280M Series B at a $2B valuation.

- <https://x.com/adityaag/status/2117313674981355761|On WisprFlow and SPC alumni>


*PODCASTS*

*Latent Space: Building Legal Agents When You Can't See the Data — Jacob Lauritzen, CTO of Legora*

_The Takeaway: The most defensible legal AI isn't the most intelligent — it's the one that actually earns lawyer trust by getting citations right, structuring the work, and running on data it can never show you._

Jacob Lauritzen built Legora out of a Stockholm basement as an underdog, starting with "ChatGPT with Swedish laws and a search tool." Today it's one of the fastest-growing legal tech companies in history, and he's learned a few things the hard way.

The hardest problem in legal AI isn't intelligence — it's data access. Law firms won't let you see their most sensitive matters, so Legora operates on-premise, inside clients' environments. You can't train on what you can't read. That constraint forces a different architecture: heavy investment in evals, an in-house team of three engineers and three lawyers, and a heat map tracking model performance across different practice areas and task types. Models improve most things on each release — but they also quietly regress on others more often than you'd expect.

Legora's "Tabular Review" — bulk extraction and review across many agreements — has become industry terminology, with Claude for Legal apparently borrowing the concept. The product has also evolved from pure research assistant to full work orchestration: Lists (like Linear for legal work), Intake (client collaboration), and Portal (lawyer-to-lawyer and agent-to-agent workflows).

On model selection, Lauritzen fought off a model picker for a long time before caving. His instinct was right — lawyers don't want to choose between Sonnet and Opus any more than they want to choose their own search algorithm. But power users insisted, and now the picker stays. His prediction: AI won't eliminate lawyers, it'll expand what a small legal team can take on. "We're just gonna be twenty engineers for the rest of the company's history, and we're gonna beat everyone who's much bigger. We're a hundred engineers now, and it feels like we're way too small."

<https://youtube.com/watch?v=bJBEFzlKPoQ>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
