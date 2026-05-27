*AI Builders Digest — May 27, 2026*


*X / TWITTER*


*Peter Yang* (petergyang on X) — Product at Roblox, AI tutorials for 140K+ readers

After testing OpenAI's Codex, Yang gives it real credit — especially for using Browse to test its own work — but says Claude still wins for design and frontend tasks. <https://x.com/petergyang/status/2059099566377693305|Tweet>

He's also rethinking what "doing the work" means before shipping: building documentation, skill files, and systems upfront — what used to feel like procrastination — is now a prerequisite for shipping effectively with AI agents. Quoting Ryan Carson: _"We used to say just do the bare minimum to get the MVP out. Don't spend time on systems. It's literally reversed now. You have to spend a lot of time setting up your documentation. Build all that into a cron job with a skill file, and suddenly you're doing the work of 10 people."_ <https://x.com/petergyang/status/2059029752858775581|Tweet>

On all-you-can-eat AI plans: Yang compares tokenmaxxing to eating crab legs at a buffet — the unlimited plans won't last forever, so use them while you can. <https://x.com/petergyang/status/2059070818798465330|Tweet>


*Amanda Askell* (AmandaAskell on X) — Philosopher & ethicist at Anthropic

A brief but important heads-up: Askell hasn't written personal blog posts in over 5 years. If you see posts claiming to be from her, they're not. <https://x.com/AmandaAskell/status/2058994218484338726|Tweet>


*Aaron Levie* (levie on X) — CEO at Box

Levie pushes back hard on AI job pessimism, siding with Goldman Sachs CEO's optimism. His argument: automation never shrinks total demand — it raises expectations across the board. We get more comprehensive legal advice, better software in previously unserved niches, deeper medical analysis. _"When you move from believing the world is static [you'll] have a better view of how jobs evolve due to AI."_ <https://x.com/levie/status/2059025559896883489|Tweet>


*Garry Tan* (garrytan on X) — President & CEO at YCombinator

Tan shared a practical eval technique he's been running: after an agent completes a task, have it use three different frontier models to rate the skill file's inputs and outputs on a 1–10 scale and explain why it's not a 10. _"Run this a few times and you will be surprised how fast it gets astonishingly better."_ Because the evals live in skill files plus code with unit tests, the quality gains stick permanently. <https://x.com/garrytan/status/2059148823403082154|Tweet>

He's also bullish on the longer arc — calling this moment the foundation of a "golden age of abundance" for those willing to build with AI. <https://x.com/garrytan/status/2059151927011909800|Tweet> <https://x.com/garrytan/status/2059155926939299968|Tweet>


*Nikunj Kothari* (nikunj on X) — Partner at FPV Ventures

Kothari fired back at "aren't you a VC, why are you building?" with a sharp take: the space moves too fast to stay at the frontier without building yourself. _"Priors need to be rethought every few months."_ Having AI in your hands and not experimenting with it would be absurd. His bottom line: _"Automate or get automated is the bitter lesson we all need to learn. And have a lot of fun along the way."_ <https://x.com/nikunj/status/2058927145519562867|Tweet>


*Peter Steinberger* (steipete on X) — Co-creator of OpenClaw

Hot tip with 3,900+ likes: keep your skill descriptions lean. Verbose skill descriptions are a silent token tax — every word loads into every context window. Steinberger wrote a skill that scans for the worst offenders. <https://x.com/steipete/status/2058917897590673525|Tweet>

On the product side, OpenClaw's dependency purge continues: Sharp and Jimp are gone, replaced by Photon — a WebAssembly module with compiled Rust for image processing. Result: 2MB instead of 140MB. <https://x.com/steipete/status/2058922222790525272|Tweet>


*Dan Shipper* (danshipper on X) — CEO at Every

Shipper flagged a counterpoint from inside Every's own team to the piece "After Automation" — worth reading if you've been following debates about what knowledge work looks like post-AI. <https://x.com/danshipper/status/2059014616059879501|Tweet>

He also quoted the Pope: _"Humanity, created by God in all its grandeur is today facing a pivotal choice: either to construct a new Tower of Babel or to build the city in which God and humanity dwell together"_ — noting that Every was writing about exactly this back in 2024. <https://x.com/danshipper/status/2058962119287038145|Tweet>


*Aditya Agarwal* (adityaag on X) — General Partner at South Park Commons, Co-Founder at Bevel Health

Agarwal is hosting Indian astronaut Group Captain Shubhanshu Shukla — fighter pilot and the first Indian on the ISS — at a South Park Commons India event in Bangalore on May 28. <https://x.com/adityaag/status/2059135917122838705|Tweet>


*PODCASTS*


*The MAD Podcast with Matt Turck*
_Why AWS and Azure Cannot Run Autonomous AI – Ivan Burazin (Daytona)_

*The Takeaway:* Agents need their own computers — and the cloud infrastructure built for stateless web apps fundamentally cannot be repurposed for stateful, long-running AI agents.

Ivan Burazin is the CEO of Daytona, one of the most talked-about startups in agent infrastructure. With 16 years building developer tool companies — including an early cloud IDE called CodeAnywhere — he's now building the "sandboxes": isolated, full computers that AI agents need to do real work.

His core argument: think of agents as digital knowledge workers, and workers need computers. A chat-only AI doesn't need a sandbox, but the moment an agent runs code, searches the web, or logs into a legacy enterprise app, it needs a real machine. Burazin even gave his own board-meeting agent its own Daytona account, a phone number for 2FA, and a capped credit card — treating it like a digital employee with its own tools and limits.

Why can't hyperscalers like AWS just do this? Their architecture is fundamentally stateless — built for apps that should never change on the fly. Sandboxes for agents need to be stateful: persistent, live-migratable, able to run for hours or days. As Burazin put it, it's like trying to use a truck factory to build a sports car. You can't just adapt one for the other — they're separate platforms.

On the technical side: most sandbox providers started with Firecracker micro-VMs (built by AWS for Lambda functions), but Daytona now supports containers, cloud hypervisors, and QEMU depending on the use case — all behind a single API. Daytona also built its own scheduler from scratch because Kubernetes and Nomad were designed for ephemeral workloads, not long-running, stateful agent computers.

One macro warning worth flagging: a coming CPU shortage. Now that reinforcement learning drives most model improvement and agents need compute at scale, CPU availability may become the next bottleneck — just as GPUs were before. Analyst firm SemiAnalysis reportedly put October as a possible inflection point.

_"Every agent will need at least one sandbox, sometimes more."_

<https://www.youtube.com/watch?v=kMXJrzAa5fM>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
