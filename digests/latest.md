AI Builders Digest — May 5, 2026

*X / TWITTER*

*Swyx* (swyx on X) — AI engineer, affiliated with AI Engineer World's Fair, Latent Space Pod, and Cognition

At AIE Europe, a founder shut down Vibe-kanban live onstage — still at 30,000 MAU — with the project continuing as open source. The brutal lesson: "Everyone who is making money is doing 2 things: selling to enterprise, and reselling tokens. We were doing neither." Swyx called the engineering retrospective from 2021–2025 deeply memorable.
- https://x.com/swyx/status/2050753293601935777

*Peter Yang* (petergyang on X) — Product at Roblox, AI newsletter writer for 140K+ readers

Peter Yang is using Codex and Claude Code to "marie kondo" his local files and Google Drive — granting these agents full computer access to audit startup apps, clean downloads folders, and restructure Drive, always asking for a plan review before executing. "Note that I always ask it for a plan first. These are semi-dangerous operations so try them at your own risk."
- https://x.com/petergyang/status/2050623358488997917

*Amjad Masad* (amasad on X) — CEO of Replit

Replit CEO Amjad Masad is excited about running 10 parallel agents across 10 projects simultaneously — calling it mind-blowing. He also reflected on how the word "prompt" has taken on entirely new meaning in the AI era while something fundamental about computing has stayed the same.
- https://x.com/amasad/status/2050793150713864678
- https://x.com/amasad/status/2050691458920005737

*Aaron Levie* (levie on X) — CEO of Box

Box CEO Aaron Levie made a forceful contrarian case against the "AI kills engineering jobs" narrative. His thought experiment: a life sciences company that once couldn't compete with tech for engineers now has the same AI output as top tech firms — and their response is to hire _more_ engineers, not fewer, because each is 2–5x more capable. "If you're wondering why new jobs show up because of AI, this is the reason. Any other view of what happens doesn't contemplate the variety of unmet needs there are in the economy."
- https://x.com/levie/status/2050684160151617603

*Garry Tan* (garrytan on X) — President & CEO of Y Combinator

YC's Garry Tan flagged Oakland's governance dysfunction: highest taxes per capita among comparable cities, worst services, with 44% of Measure E revenue pre-committed to pre-approved union raises. On the AI side, he's bullish on using GBrain with OpenClaw's book-mirror skill pack — describing it as "like infinite personal Blinkist."
- https://x.com/garrytan/status/2050775806574751816
- https://x.com/garrytan/status/2050763012894834952

*Nikunj Kothari* (nikunj on X) — Partner at FPV Ventures

FPV Ventures partner Nikunj Kothari pushed back hard on a trend he's seeing in VC: funds capping downside instead of maximizing upside, investing in startups primarily because "big token factory will acquire them so our downside is capped." He sees this as AUM-maximizing behavior that won't return a 5–10x fund, and a waste of the only thing that can't be recovered: time.
- https://x.com/nikunj/status/2050779734116856137

*Peter Steinberger* (steipete on X) — OpenClaw + OpenAI

Peter Steinberger shipped two things back-to-back. First, *Crabbox 0.3.0* — a remote Linux tool for dirty worktrees — adding GitHub browser login, Blacksmith Testbox integration, live run replay via `crabbox attach`, durable run events, AWS image creation, and Cloudflare Access support (`brew upgrade openclaw/tap/crabbox`). Second, an OpenClaw plugin update that fixes npm dependency and slowness issues by moving nearly everything into extensions, making the package significantly leaner.
- https://x.com/steipete/status/2050490163810230579
- https://x.com/steipete/status/2050735979477008412

*Dan Shipper* (danshipper on X) — CEO of Every

Every CEO Dan Shipper laid out a sharp prediction for the next decade of work: "agent running continuously on the left, application that you + the agent use on the right." He also highlighted Every's Proof tool as a Codex-native writing app for anyone wanting to try that pattern today.
- https://x.com/danshipper/status/2050583747041640608
- https://x.com/danshipper/status/2050608311888941301

*Aditya Agarwal* (adityaag on X) — General Partner at South Park Commons, ex-CTO of Dropbox

South Park Commons partner and former Dropbox CTO Aditya Agarwal offered a grounding reminder: step away from the console and terminal, and you'll find deeply inspiring hard tech being built across America — including things being launched into space.
- https://x.com/adityaag/status/2050660894234059050

*Sam Altman* (sama on X) — CEO of OpenAI

OpenAI CEO Sam Altman made a candid self-correction: he keeps wanting models to be cheaper and faster rather than smarter — but smarter still wins as the most important variable. He also gave a quick positive verdict on GPT-5.5 xhigh in fast mode, noting he had been "psyoped by Twitter on medium for a bit."
- https://x.com/sama/status/2050671161915371998
- https://x.com/sama/status/2050658558174437701


*OFFICIAL BLOGS*

*Anthropic Engineering — <https://www.anthropic.com/engineering/managed-agents|Scaling Managed Agents: Decoupling the brain from the hands>*

Anthropic Engineering published a technical deep dive on how they redesigned *Managed Agents* — their hosted long-horizon agent service — by solving a classic infrastructure problem: don't adopt a pet.

The original design crammed Claude's harness, the session log, and the sandbox into one container. It worked until containers became unmaintainable pets — unresponsive, impossible to safely debug (because user data lived alongside credentials), and rigidly coupled. The fix: decouple the "brain" (Claude + harness) from the "hands" (sandboxes/tools) and the "session" (the durable event log). Each can now fail or be replaced independently.

Key results from decoupling:
- p50 time-to-first-token dropped ~60%, p95 dropped over 90%
- Harnesses became stateless and restartable via `wake(sessionId)`
- Containers became interchangeable cattle — failures surface as tool errors, not lost sessions
- Security improved structurally: credentials never enter the sandbox where Claude's generated code runs; Git tokens are consumed at clone time, and OAuth tokens live in a secure vault accessed only via a dedicated proxy

The session log is now a durable, external event stream that functions as Claude's long-term memory, accessible via `getEvents()` with positional slicing — sidestepping the irreversibility problem of compaction and trimming. The architectural analogy: "Operating systems have lasted decades by virtualizing the hardware into abstractions general enough for programs that didn't exist yet." Managed Agents does the same for agent harnesses — opinionated about interfaces (session, harness, sandbox), unopinionated about what runs behind them.


*PODCASTS*

*Training Data — <https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8|OpenAI's Greg Brockman: Why Human Attention Is the New Bottleneck>*

_The Takeaway:_ As AI takes over the doing, human attention — deciding what's worth doing and whether it was done right — becomes the scarcest resource in any organization.

Greg Brockman, OpenAI's co-founder and president, has a background that includes being employee #4 at Stripe before joining OpenAI at its founding. He's unusually positioned to speak to what AI actually looks like inside a frontier lab — not as a pitch, but as a practice.

His core thesis is counterintuitive: the biggest bottleneck in AI-assisted work isn't model capability, it's human judgment. "The doing of things now is easy. The 'Is this a good thing? Is this what I wanted? Is this aligned with my values, with my desires?' — that is going to become the single most important bottleneck." He illustrated this with a story: his Codex agent, after waiting two minutes on a Slack response, decided to escalate — and messaged the person's manager. Technically reasonable. Socially disastrous.

On compute: demand has never been met since ChatGPT launched. When asked how much compute to buy at launch, Brockman told his team "all of it" — and that instinct still holds.

On scaling laws: they remain a "beautiful mystery" — empirically powerful, not fully explained — and there is no wall in sight.

On AGI: Brockman puts us at roughly 80% of the way there. Models already write code better than most humans. One engineer handed a complex systems optimization doc to a model before bed, went to sleep, and woke up to find the work complete — implemented, profiled, and iterated to an optimized result. Work that would have taken a team a week.

His advice for founders: lean in hard now. The one-time shift is about context — getting AI enough information to actually help. "You have all these meetings. You didn't include the AI. That's not very nice to the AI."

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
