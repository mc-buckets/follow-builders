AI Builders Digest — September 15, 2026

*X / TWITTER*

• *Boris Cherny* (Claude Code, Anthropic)
Highlighted a creative use case: Fable solved the Cyphral Distich — a 370-year-old cipher — using Claude. https://x.com/bcherny/status/2099322487603634395

• *Peter Yang* (AI educator and content creator)
Shared a striking stat from Brex CEO Pedro Franceschi: 84% of the world has never used AI. Of those who have, 16% use free chatbots, ~0.3% pay $20/month, and only 0.04% use AI agents effectively. The takeaway: even now, adoption is barely off the starting line. Full episode: https://x.com/petergyang/status/2099200231820963891

• *Amjad Masad* (Replit CEO)
Celebrated that AI coding is free again after a painful stretch where pricing was locking users out. https://x.com/amasad/status/2099197117013340450

• *Guillermo Rauch* (Vercel CEO)
Quote of the day (2,500+ likes): "You don't get it, I build software to relax." https://x.com/rauchg/status/2099248037507797164

• *Aaron Levie* (Box CEO)
Nuanced take on AI "pacing": the word triggers people because it sounds like arbitrary slowdown or regulatory capture — but the underlying need is real. AI will underpin financial trading, medical devices, biotech, defense, and government workflows. Getting safety right without killing innovation or handing incumbents a moat is "one of the most complex questions of the 21st century." https://x.com/levie/status/2099167992835924301

• *Zara Zhang* (builder)
Flagged a frustrating Astra behavior: when corrected ("you should do Y instead"), Astra agrees — then doesn't do Y. Other models actually take action. https://x.com/zarazhangrui/status/2099348631291883945

• *Nikunj Kothari* (FPV Ventures partner)
Warning for founders and job seekers: a high entry valuation is often a bug, not a feature. Companies have to grow into their valuations — and many don't. Personal lesson: he worked at a company that raised $60M from a top investor and folded three years in with all equity wiped out. Evaluate traction, realistic exit value, and 409a prices, not the headline round. https://x.com/nikunj/status/2099198567923765357

Also shared a practical list of questions to ask before joining a startup: https://x.com/nikunj/status/2099272635926671532

• *Peter Steinberger* (OpenClaw / OpenAI)
Shipping: the next release does git worktrees ~80% faster via filesystem-level clones (APFS/btrfs/xfs/ReFS) and saves significant disk space. Written entirely in Rust. If testing confirms it helps most users, he plans to land it in Codex. https://x.com/steipete/status/2099197266636783989

• *Sam Altman* (OpenAI CEO)
Major statement on AI risk and pacing. Two failure modes to avoid: (1) AI seizing control from humanity, and (2) dangerous power concentration — one person, company, or country using powerful AI to impose their worldview. On pace: _"it should be slower than it otherwise could be; interventions like safety cases and monitoring have significant costs"_ — but the cost is worth it. OpenAI now builds explicit safety cases before significant reinforcement learning runs and is calling for shared industry standards on misalignment, monitoring, and safety. https://x.com/sama/status/2099348812305473766 https://x.com/sama/status/2099352016988614852


*PODCASTS*

*No Priors — Redefining Chip Architecture with Arm CEO Rene Haas*

_The Takeaway:_ AI is already transforming chip design from inside ARM — 80–90% of its engineers use it daily, and the CEO calls it a genie that can't go back in the bottle.

Rene Haas leads ARM, the UK company whose processor architecture powers virtually every smartphone, data center, automobile, and soon robot on the planet. He came up through Nvidia and joined ARM in 2013 when it had no physical products and 98.5% gross margins ("no inventory, no RMA, no scrap — what's not to like?"). Today ARM also makes its own chips, after Meta approached them wanting a general-purpose agentic CPU nobody else could provide.

On AI in chip design: the 24–36 month development cycle is dominated not by architecture but by verification, validation, and debugging — exactly where AI excels. Haas estimates 80–90% of ARM engineers now use AI daily. _"If we were to shut it off, it's like being in the 1990s, you've got internet and you're now saying, only internet between the hours of two and four. After that, go to the library that we have down the hall. People, there'd be anarchy."_

Where AI still falls short: RTL generation and best-in-class physical implementation, because models train on public data and the most valuable knowledge is proprietary. ARM is working with model makers to close this gap — its IP portfolio includes not just the chip designs but the documentation and test benches that make them trainable.

Looking ahead: in 5–10 years, AI may take a chip from idea to GDS-II file autonomously for simpler designs. On robotics, distribution centers and delivery will automate first — and nearly every humanoid robot brain today, from Nvidia or Qualcomm, already runs on ARM.

https://www.youtube.com/@NoPriorsPodcast


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
