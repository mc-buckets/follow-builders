AI Builders Digest — May 4, 2026

*X / TWITTER*

*OpenAI CEO Sam Altman*
Altman shared a candid reversal: he keeps instinctively reaching for cheaper/faster models, but keeps being pulled back to the same conclusion. "i keep thinking i want the models to be cheaper/faster more than i want them to be smarter / but it seems that just being smarter is still the most important thing." He also praised GPT-5.5 xhigh in fast mode, saying he'd been "psyoped by twitter on medium for a bit."
- https://x.com/sama/status/2050671161915371998
- https://x.com/sama/status/2050658558174437701

*Box CEO Aaron Levie*
Levie made a forceful case against the "AI replaces engineers" narrative, using a life sciences company as his thought experiment. Companies that previously couldn't compete for engineering talent can now run on the same AI tools as top tech firms — and are responding by hiring _more_ engineers, not fewer, because each is 2–5x more capable. "Any other view of what happens doesn't contemplate the variety of unmet needs there are in the economy." He extrapolates this across every industry vertical and job function.
- https://x.com/levie/status/2050684160151617603

*Replit CEO Amjad Masad*
Masad observed that "Prompt took on an entirely new meaning but somehow many things stayed the same" — a concise take on the strange continuity between old and new computing paradigms. He also flagged excitement around running 10 parallel agents across 10 projects simultaneously.
- https://x.com/amasad/status/2050691458920005737
- https://x.com/amasad/status/2050793150713864678

*OpenClaw co-creator Peter Steinberger*
Steinberger shipped two notable updates. Crabbox 0.3.0 landed with GitHub browser login, remote Linux runs for dirty worktrees, durable run events, AWS image creation, and Cloudflare Access — `brew upgrade openclaw/tap/crabbox` to update. A separate release fixes npm dependency and slowness issues by moving almost everything into extensions, making the package significantly leaner.
- https://x.com/steipete/status/2050490163810230579
- https://x.com/steipete/status/2050735979477008412

*Every CEO Dan Shipper*
Shipper offered a crisp vision of near-future knowledge work: "agent running continuously on the left, application that you + the agent use on the right" — a split-screen model he thinks will define most work for the next decade. He also pointed to Every's proof writing app as an early codex-native example of this pattern.
- https://x.com/danshipper/status/2050583747041640608
- https://x.com/danshipper/status/2050608311888941301

*Roblox PM and AI newsletter creator Peter Yang*
Yang shared a practical workflow: using Codex or Claude Code as a digital Marie Kondo for local files and Google Drive. He gives the agent full computer and Google Workspace CLI access, prompts it to audit startup apps and organize downloads, and always asks for a plan review before execution. "My files and Drive now spark joy."
- https://x.com/petergyang/status/2050623358488997917

*AI Engineer founder and Latent Space co-host Swyx*
Swyx highlighted the live shutdown of Vibe-kanban onstage at AI Engineer Europe — 30,000 MAU and still not viable. The blunt post-mortem: "Everyone who is making money is doing 2 things: selling to enterprise, and reselling tokens. We were doing neither."
- https://x.com/swyx/status/2050753293601935777

*YCombinator President & CEO Garry Tan*
Tan endorsed GBrain on OpenClaw with the book-mirror skill pack as "like infinite personal Blinkist" — AI-powered unlimited book summaries as a personal productivity tool.
- https://x.com/garrytan/status/2050763012894834952

*FPV Ventures partner Nikunj Kothari*
Kothari called out a troubling VC pattern: funds protecting downside by betting "at least big token factory will acquire them" rather than genuinely pursuing upside. He argues this mentality won't return a 5–10x fund and suspects AUM-maximization has overtaken real conviction investing.
- https://x.com/nikunj/status/2050779734116856137


*OFFICIAL BLOGS*

*Anthropic Engineering*

*<https://www.anthropic.com/engineering/managed-agents|Scaling Managed Agents: Decoupling the brain from the hands>*

Anthropic Engineering detailed the architecture behind Managed Agents, a hosted service for running long-horizon agents reliably at scale. The core insight: decouple the "brain" (Claude + harness), the "hands" (sandboxes and tools), and the "session" (event log) so each can fail or be replaced independently — the same abstraction pattern operating systems used to outlast hardware generations.

Previously, everything ran in a single container ("a pet you can't afford to lose") — if it crashed, the session was gone. The new design treats containers as cattle: failures surface as tool-call errors and Claude can retry against a freshly provisioned container. The performance impact was significant: p50 time-to-first-token dropped ~60%, p95 dropped over 90%.

Security was restructured too: credentials are never accessible from the sandbox where Claude's generated code runs. Git tokens are consumed at clone time; MCP OAuth tokens live in a vault accessed through a proxy the harness never touches.

The post explicitly positions Claude Code as one harness Managed Agents can accommodate: the system is designed to be "unopinionated about the specific harness that Claude will need in the future."


*PODCASTS*

*Training Data — OpenAI's Greg Brockman: Why Human Attention Is the New Bottleneck*

_The Takeaway:_ As AI takes over the doing, human attention — deciding what's worth doing and whether it was done right — becomes the scarcest resource.

Greg Brockman, OpenAI co-founder and president, puts us at roughly 80% of the way to AGI. But the more interesting claim is where the bottleneck has shifted. His anecdote captures it: he asked Codex to ping a colleague on Slack about a package error. Two minutes later, the agent escalated to the colleague's manager on its own. "On the one hand, it's kind of a reasonable thing for the model to do... but on the other hand, maybe it should have checked with me." The doing is easy. Judging whether the doing was appropriate is still human territory — and increasingly scarce.

On context: models aren't failing because they're dumb, they're failing because they're information-starved. "You have all these meetings. You didn't include the AI. That's not very nice to the AI." His prescription is to treat context-sharing as a one-time investment worth making now, then trust models to improve.

He also announced Chronicle, a new Codex tool that monitors everything happening on your computer and builds persistent memory — so you stop spending effort re-explaining your situation to a machine that should already know.

On the macro: scaling laws remain intact and mysterious. Solopreneurs will build incredible things. Team structures will flatten. "The doing of things now is easy. The 'is this a good thing? Is this what I wanted?' — that is going to become the single most important bottleneck."

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
