*AI Builders Digest — July 22, 2026*


*X / TWITTER*

*Swyx* (AI engineer, advisor at Cognition and Temporal, host of Latent Space podcast)
Swyx flagged an important finding from a new RLM (reinforcement learning model) paper: the open secret of frontier model training is that you can game almost any benchmark by training on lookalikes of test data rather than the actual test set. When models release open weights, the training datasets and RL environments typically aren't included, making verification impossible — plausible deniability built in. The paper by Alex Zhang and Omar explores NLP distance metrics on hidden trajectories as a detection approach. The upside: RLMs do appear to generalize to unseen tasks that share latent structure with training data.
<https://x.com/swyx/status/2079411861150429402|View tweet>

*Thibault Sottiaux* (Codex & ChatGPT at OpenAI)
Sottiaux posted: "Never a dull moment when you work at OpenAI. Absolutely incredible place." The standalone post pulled 3,672 likes and 1,310 replies — unusually high engagement that suggests something significant is in motion at the company.
<https://x.com/thsottiaux/status/2079355529101705264|View tweet>

*Peter Yang* (AI educator and content creator)
Yang made a pointed geopolitical take: "Banning Chinese models will be the same self own as banning Chinese EVs." He also highlighted a key agent design principle from Thariq (Claude Code at Anthropic): use a separate verification agent with a rubric to review the primary agent's output. The reason is "self-preferential bias" — models grade their own outputs too leniently. For subjective tasks like "is this a good video short?" there is no deterministic answer, making an independent verifier essential.
<https://x.com/petergyang/status/2079273815004303477|View tweet>
<https://x.com/petergyang/status/2079257646939742542|View tweet>

*Madhu Guru* (Sr. Director of AI at Meta; previously led Gemini, Veo, and Nano at Google)
Guru offered two sharp takes. First: "The road to AGI is paved with economically valuable tasks. That's why enterprise AI is one of the most important frontiers. It's where many of those tasks live." Second: he reframed the current AI economics debate — open vs. closed weights, inference costs, model routing — as the tokenomics debate that actually matters, four years after the crypto/web3 version of that conversation fizzled out.
<https://x.com/realmadhuguru/status/2079369965569003691|View tweet>
<https://x.com/realmadhuguru/status/2079227605031829700|View tweet>

*Amjad Masad* (CEO at Replit)
Masad flagged what may be a new milestone: a physical product shipped by a coding agent — posing it as a question, signaling this is genuinely new territory.
<https://x.com/amasad/status/2079282869063786541|View tweet>

*Guillermo Rauch* (CEO at Vercel)
Rauch dropped the most-shared take of the day: "The big lesson from AI is that everything is code. A slide deck is code. Design is code. That cool promo video? Code. Excel automation? Code. The universe? Probably made of code too." The post drew 4,300 likes and 400 retweets — a sharp articulation of how AI is collapsing the boundary between creative and technical work.
<https://x.com/rauchg/status/2079274102129304026|View tweet>

*Aaron Levie* (CEO at Box)
Levie highlighted Cursor's new research on multi-model agentic systems: pairing a frontier model as planner/orchestrator with a cheaper workhorse model delivers a *15x cost improvement*. The key insight: "Few moments in a large task genuinely require frontier intelligence — the original decomposition, the design decisions, and certain trade-offs. Once a frontier planner has collapsed the ambiguity into a detailed, explicit instruction, less expensive models simply have to follow it." Levie sees this as the defining design pattern for complex agents, and argues that companies able to route intelligently across model tiers in specific domains — coding, finance, legal, healthcare — will win the applied AI layer.
<https://x.com/levie/status/2079402164988895293|View tweet>

*Garry Tan* (President & CEO at Y Combinator)
Tan pushed back on California's proposed asset seizure tax, calling it a "naked cash grab" by SEIU-UHW that would leave the state more impoverished. He also amplified a compute-focused post with a Wu-Tang riff: "Compute rules everything around me CREAM."
<https://x.com/garrytan/status/2079369233218306285|View tweet>
<https://x.com/garrytan/status/2079240755135357356|View tweet>

*Matt Turck* (VC at FirstMark Capital, host of MAD podcast)
Turck offered a dry take on competitive dynamics: OpenAI and Anthropic when a top free Chinese open-source model drops. A wry acknowledgment of the pressure that strong free Chinese models keep exerting on the frontier labs.
<https://x.com/mattturck/status/2079198838741458989|View tweet>

*Zara Zhang* (Builder and developer)
Zhang proposed a two-round interview redesign for the AI era: Round 1 is in-person with no AI — testing raw domain expertise and on-the-fly thinking. Round 2 requires completing a project that is impossible without AI; candidates are evaluated on both the result and their agent chat transcript. She also observed that companies founded after coding agents appeared look structurally different from day one — teams under ten people by design, work organized by projects not departments, each person closes their own loop, almost no internal meetings.
<https://x.com/zarazhangrui/status/2079409165424799889|View tweet>
<https://x.com/zarazhangrui/status/2079225776545968166|View tweet>

*Nikunj Kothari* (Partner at FPV Ventures)
Kothari warned founders against a seductive trap: assuming that because "AI has no moats," scale and capital automatically become the default moat. His historical roll call of well-capitalized failures — Webvan, Groupon, MySpace, Yahoo, AltaVista, Blockbuster, Nokia — each beaten by a company with a better unique insight, or collapsed under its own weight. His framing: "find a unique insight worth a 10+ year journey, while being prudent enough to not let capital and scale become a substitute for it." He also flagged the accelerating VC-to-fast-startup migration wave, with "Special Projects" emerging as the defining title for this cohort.
<https://x.com/nikunj/status/2079328912912355470|View tweet>
<https://x.com/nikunj/status/2079211477127291350|View tweet>

*Dan Shipper* (CEO at Every)
Shipper is hiring a senior engineer to work on Every's AI agent. The role requires genuinely loving agents. Currently prioritizing candidates he already knows from his network.
<https://x.com/danshipper/status/2079331654359818503|View tweet>


*PODCASTS*

*No Priors — Travel Through the Lens of AI with Booking.com CEO Glenn Fogel*

_The Takeaway:_ The CEO of a $100B+ travel company believes there is no such thing as a moat — and that conviction is exactly why he's more excited about building now than at any point in his 27-year career.

Glenn Fogel joined Priceline in 2000 when it was worth a few hundred million dollars and helped grow Booking Holdings past $180B in market cap. He now oversees the company's major bet on AI agents as the next evolution of travel.

His most counterintuitive position is rejecting the concept of durable competitive advantages entirely. "There is no such thing as somewhere you're gonna be protected against innovation. Today, we have a competitive advantage on areas. Absolutely. But those can go away tomorrow." For a company with 8.6 million alternative accommodation listings and over a billion room nights per year — close to Airbnb's scale in alternative accommodations — that's a genuinely uncomfortable thing for a CEO to say out loud.

On AI agents, Fogel is building toward what he describes as a personalized travel concierge: a system that knows everything about a customer, never forgets anything, and can iterate through infinite permutations to plan a trip the way a wealthy person's human assistant would — but at scale for everyone. He tested Priceline's agentic tool, Penny, on a complex multi-city Europe trip for his family with split flights, frequent flyer optimization, and restaurant research. "It was incredible." Penny adoption has been doubling monthly, and AI has already driven customer service costs down roughly 10% while pushing satisfaction up.

What he's still working out: the ROI math. With $186B in annual travel volume, even fast-growing agentic adoption barely registers today. Token costs, model selection for different tasks, and long-term lifetime value are all still being measured. He's investing roughly $700M in AI and tech this year, and returning record capital to shareholders — $3.6B in stock buybacks in Q4 alone — when he can't find better internal uses.

On job displacement, he is worried less about whether AI replaces jobs and more about the speed. He points to his own company's history — multilingual translation and customer service jobs disappeared when machine translation matured — and fears retraining programs won't keep pace. His internal response: upskill every employee on AI, every day. "Even if we end up that we can't replace or retrain someone, at least they are better skilled for a job somewhere else."

<https://www.youtube.com/watch?v=8nj_0wZkbtA|Watch on YouTube>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
