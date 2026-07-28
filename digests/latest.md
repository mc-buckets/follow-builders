*AI Builders Digest — July 28, 2026*


*X / TWITTER*

*Sam Altman* (CEO, OpenAI)
Shared a live demo of ChatGPT Work that has people paying attention: from a single phone prompt, it pulled his full chat history, planned three group trip options for 9 friends, built a full-stack coordination website, and drafted the invite email. "It...just worked." https://x.com/sama/status/2081396796174282900
Also reacted to a tweet framing the moment as needing a new kind of device: "agreed feels big, i want a new kind of computer." https://x.com/sama/status/2081513071135346814

*Thibault Sottiaux* (Codex & ChatGPT, OpenAI)
Reports the vibe inside OpenAI right now: "Never seen OpenAI more focused and humming." https://x.com/thsottiaux/status/2081534792903147881
On the heels of ChatGPT Work launching, he's pushing for people to actually use it as a task agent: "It does at least 20 things for me every single day and I'm still surprised." https://x.com/thsottiaux/status/2081444811647963244

*Aaron Levie* (CEO, Box)
Made a long-form case for why the applied AI layer is the biggest opportunity in software right now. Raw model intelligence isn't enough — you need industry-specific integrations, regulatory context, the right UX for human decision points, and feedback loops that improve the underlying data. His counterintuitive take: as models get better, this layer becomes *more* valuable, not less, because you can attempt more ambitious automations that require even deeper integration. https://x.com/levie/status/2081491621162668207

*Guillermo Rauch* (CEO, Vercel)
Vercel co-signed the Open Weights and American AI Leadership letter, calling open weights "the logical next frontier" in the tradition of open source, open data, and open protocols. https://x.com/rauchg/status/2081546513885622760
Also shared an impressive technical result: compiled the Vercel CLI TypeScript codebase to a fully static native binary using `scriptic` — 1.28mb output, 1.5ms startup overhead, compiled in under 3 seconds. No embedded V8 or QuickJS. https://x.com/rauchg/status/2081517519303737559

*Amjad Masad* (CEO, Replit)
Flagged a noteworthy security finding from a former Anthropic employee: hackers are reportedly choosing to use AI lab subscriptions (heavily subsidized) for attacks rather than open-source models — because the subsidized commercial APIs are simply cheaper and more capable for their purposes. https://x.com/amasad/status/2081576172656456076

*Dan Shipper* (CEO, Every)
Taking the week off to write what he's calling "the definitive history of how Codex happened," based on deep insider interviews at OpenAI. Publishing on Every in a few weeks. He'll be dropping breadcrumbs along the way. https://x.com/danshipper/status/2081412243388788988

*Garry Tan* (President & CEO, Y Combinator)
Wrapped YC Startup School 2026, with Sam Altman closing out as the final keynote. https://x.com/garrytan/status/2081602195292864532
Also posted a sharp two-liner that landed with YC founders: "Don't LARP. Be earnest." https://x.com/garrytan/status/2081586567211348432

*Madhu Guru* (Sr. Director, AI at Meta; former Google lead on Gemini, Veo, Nano)
Pushed back on "AI hasn't shipped impact yet" criticism with a two-phase framework. Phase 1 (now): companies with distribution are moving fast into adjacent areas — things like virtual clothes try-on that previously required heavy custom software. Phase 2 (coming): net-new features and innovation that will make the impact undeniable. "Companies are figuring out the playbook and the impact is not yet visible at the ecosystem level." https://x.com/realmadhuguru/status/2081437850466451736

*Zara Zhang* (Builder)
Two quick takes worth sitting with: (1) Stop measuring AI adoption by tokens burned — measure time from user need arriving to that thing shipping. (2) The reason AI tutorials are everywhere is structural: general-purpose chat interfaces present a blank box, and people genuinely freeze because they don't know what to ask. https://x.com/zarazhangrui/status/2081627581997269192 and https://x.com/zarazhangrui/status/2081627109299310684

*Peter Yang* (AI educator, creator of practical AI tutorials)
After talking to non-AI-obsessed people in Canada, reports that the mainstream #1 concern isn't running out of tokens — it's trust: "do I trust ChatGPT enough to share my Gmail, Calendar, Google Workspace, Microsoft Office?" A useful grounding note for anyone building AI-connected tools. https://x.com/petergyang/status/2081555286817648738

*Nikunj Kothari* (Partner, FPV Ventures)
One sharp prediction: "proof of prompt is soon going to replace proof of work." https://x.com/nikunj/status/2081383934928068619


*PODCASTS*

*The MAD Podcast with Matt Turck — "OpenAI's Compute Chief: We Can't Build Fast Enough | Sachin Katti"*

*The Takeaway:* OpenAI's biggest fear isn't over-building — it's never being able to build fast enough. Every time they've thought they had enough compute and eased off, they've regretted it.

Sachin Katti, OpenAI's head of industrial compute, came from Stanford (CS/EE professor), multiple startups, and Intel's CTO office. He now runs the full lifecycle of compute at OpenAI: sourcing land, power, and chips; financing the infrastructure; operating it; and making the internal allocation decisions that determine who at the company gets scarce GPU time. He's blunt about that last part — he is "not very popular" because someone is always unhappy.

OpenAI is spending roughly $50B on compute this year in a global market pushing $700B total. Demand still outstrips supply, and every increment that comes online gets consumed immediately.

Key things he covers:

- *Data centers as intelligence factories:* Massive liquid-cooled supercomputers the size of football fields, turning electrons into tokens. Running chips hotter = more memory bandwidth = more compute — so better cooling directly translates to more intelligence per watt.

- *Power strategy:* OpenAI funds new grid infrastructure (gas, solar, hydro) at every site it builds, arguing this makes data centers a net positive for rural communities — new property taxes, jobs, and grid upgrades that wouldn't otherwise happen. Where grid limits are reached, they're moving to on-site generation (currently gas turbines in the US).

- *Jalapeno chip (custom silicon):* Built in just 9 months with Broadcom as manufacturing partner. The key advantage: OpenAI knows what models it's designing for, so it can co-design the hardware to those workloads rather than designing for a generic customer. AI is now actively helping optimize the chip design itself. The primary metric it optimizes: tokens per watt.

- *MRC networking protocol:* A multipath packet-spraying protocol that keeps 100,000-GPU training clusters running despite constant link failures. The idea: between any two chips, spray packets across all available paths simultaneously — whatever gets through, wins. The training job never has to think about network reliability.

- *On the "over-building" question:* He's directionally confident. Scaling laws continue to hold. AI doing AI research means the number of experiments that can be run explodes — and each experiment needs compute. The real supply-side surprises are bottlenecks in physical supply chains: gas turbines, transformers, and qualified electricians are all in shortage.

- *Guaranteed capacity for enterprises:* OpenAI now lets enterprises lock in token commitments. His framing: "Intelligence is becoming a supply unit for every digital enterprise" — and it makes business sense to secure your supply of a critical input.

On the ever-present temptation to slow down: _"Anytime you have thought you have enough compute, we can slow down. Always negatively surprises like, oh, we should not have slowed down."_

https://www.youtube.com/watch?v=wEZBlmvxx4o


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
