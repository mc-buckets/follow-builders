*AI Builders Digest — June 17, 2026*

*X / TWITTER*

*Josh Woodward* (VP at Google Labs / GeminiApp / Google AI Studio)

Two significant Gemini updates: the voice mic now supports 70+ languages with automatic language detection — users can mix languages freely in a single session without changing any settings. A Gemini Trusted Tester program is also opening limited slots for power users who want early access to unreleased features before anyone else.
- <https://x.com/joshwoodward/status/2066673011554435450|Gemini mic: 70+ languages, no settings change needed>
- <https://x.com/joshwoodward/status/2066664862671921259|Gemini Trusted Tester program signup now open>

*Amjad Masad* (Replit CEO)

Masad highlighted Replit's domain-specific agents: a growth agent that surfaces SEO issues and a security agent that flags potential vulnerabilities. His favorite workflow: "select all, fix with Agent." He also took a jab at model naming conventions, quipping "Who needs Fable when you can have Mistral's Le Chaton Fat."
- <https://x.com/amasad/status/2066683949129330817|Replit domain-specific agents>
- <https://x.com/amasad/status/2066700847187140655|Le Chaton Fat vs Fable>

*Guillermo Rauch* (Vercel CEO)

Three related announcements: Vercel shipped longer function runtimes — the culmination of a multi-year microVM-based "Fluid Compute" investment that also powers Vercel Builds and Sandboxes. His bigger thesis: sandboxes, functions, servers, and builds are all expressions of the same underlying compute primitive, and "2026 is the year serverless and servers finally converge." The v0 coding tool also now ships with Vercel engineering skills baked in by default, with the option to pull from a community library or add team-private skills.
- <https://x.com/rauchg/status/2066553521978097921|Longer Vercel function runtimes now live>
- <https://x.com/rauchg/status/2066556235961237826|Serverless and servers converging in 2026>
- <https://x.com/rauchg/status/2066567117562868009|v0 ships Vercel engineering skills by default>

*Aaron Levie* (Box CEO)

Two sharp takes on AI strategy. On the future: the winners won't be those with the biggest models but those that combine unique data, workflows, and intelligent model routing — _"intelligence is becoming increasingly customizable."_ On AI regulation: an "FDA for AI" model that requires pre-release approval for every model would create an infinite-permutation review backlog, slowing global AI progress dramatically. His alternative: regulate the *applied uses* of AI, where risk actually shows up.
- <https://x.com/levie/status/2066735879213994434|Customizable intelligence is the future of AI>
- <https://x.com/levie/status/2066554018953146689|Against pre-release model regulation>
- <https://x.com/levie/status/2066526720480690221|Open source going to win big>

*Peter Steinberger* (OpenClaw / OpenAI)

Went viral (1,400+ likes) after discovering Apple can no longer manufacture the Mac Studio in the US: "We don't even know how to make these anymore." He also demoed clawsweeper — an open source bot that reviews incoming GitHub issues against a VISION.md file and, if the issue fits, automatically opens and self-reviews a pull request.
- <https://x.com/steipete/status/2066471737068232835|Mac Studio: we don't know how to make these anymore>
- <https://x.com/steipete/status/2066457262571360396|clawsweeper: auto-review and PR bot>

*Nikunj Kothari* (FPV Ventures partner)

Kothari observed that 32 VCs in his network — from associates to GPs — have moved back into operating roles over the past 12 months, with the pace accelerating. His read: operators get direct customer contact, greater day-to-day autonomy, and a realistic shot at liquidity far sooner than waiting ~13 years for carry.
- <https://x.com/nikunj/status/2066701833964531736|32 VCs moving back to operating — and they seem happier>

*Peter Yang* (AI educator, Creator AI newsletter, 150K+ readers)

Enthusiastic on OpenAI Codex's browser use: _"It's so good that it almost makes me forget APIs are even needed."_ Also gave Cursor AI credit for planning what he described as a Michelin-quality dinner.
- <https://x.com/petergyang/status/2066753125197967653|Codex browser use nearly makes APIs feel optional>
- <https://x.com/petergyang/status/2066756347438469602|Cursor plans a Michelin-quality dinner>

*Swyx* (builder; Cognition / Temporal / AI Engineer)

A brief but pointed note on AI news velocity: goblingate — a recent AI industry controversy — happened only 1.5 months ago, a reminder of how compressed the news cycle has become.
- <https://x.com/swyx/status/2066705614454337663|Goblingate was 1.5 months ago>

*OFFICIAL BLOGS*

*Claude Blog — New in Claude Managed Agents: dreaming, outcomes, and multiagent orchestration*

Anthropic launched three major capability updates to Claude Managed Agents:

- *Dreaming* (research preview): A scheduled process that reviews past agent sessions, extracts recurring patterns, and refines memory so agents self-improve between sessions. Teams can review changes before they land or allow automatic updates. Harvey saw ~6x completion rate gains in testing.
- *Outcomes*: Define a success rubric; a separate grader evaluates output in its own context window and sends the agent back for revisions until it clears the bar. In benchmarks, outcomes improved task success by up to 10 points, with file generation quality up +8.4% (docx) and +10.1% (pptx).
- *Multiagent orchestration*: A lead agent breaks complex jobs into pieces and delegates each to a specialist running in parallel on a shared filesystem. Netflix uses this to surface recurring issues across hundreds of build log sources; Spiral by Every uses it for parallel draft generation with outcomes-based quality gating.

<https://claude.com/blog/new-in-claude-managed-agents|Read the full post>

*PODCASTS*

*The MAD Podcast with Matt Turck — "OpenAI's Dan Roberts: Why AI Can Now Make Discoveries"*

*The Takeaway:* Reinforcement learning isn't just the cherry on top of language model training — it's the mechanism that teaches AI to think, and the same explore-vs-exploit dynamics that made AlphaGo legendary are what let AI disprove a 60-year-old conjecture in combinatorics.

Dan Roberts leads the Foundations of Reinforcement Learning team at OpenAI, arriving from theoretical physics (MIT PhD, IAS postdoc) via Facebook AI Research, a startup, and Sequoia Capital. His core claim: RL is what transforms a next-token predictor into a reasoning machine.

His centerpiece is the AI vs. Erdős moment. OpenAI's model attacked the unit distance problem not by following consensus but by taking a contrarian stance — *assuming the conjecture was false* — then spending hours of compute tracing a path through algebraic number theory that no single human expert would naturally combine. As Roberts puts it: _"You need this really strong persistence... and expertise in this other field... and then also be super contrarian and go down this really long path."_

His analogy for RL vs. supervised learning: watching your dad play Mario vs. playing yourself. Supervised learning is memorizing someone else's moves; RL is getting your hands on the controller and learning from your own mistakes and rewards. The hard problem is sparse rewards — chess doesn't tell you where you went wrong until the very last move.

Roberts also offers a physicist's answer to fears about "emergent" AI behavior appearing only at scale: there's no emergence, just gaps in understanding. The right move — borrowed directly from physics — is to build simplified toy systems that exhibit the same phenomenon at smaller scale. Once you can reproduce it in miniature, you actually understand it.

On test-time compute: the model simply generates more tokens, using that compute the way a mathematician fills a scratch pad. RL is what trains the model to make that scratch pad worth reading.

<https://www.youtube.com/watch?v=oWOz2htozfI|Watch on YouTube>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
