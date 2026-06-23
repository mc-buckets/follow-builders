AI Builders Digest — June 23, 2026

*X / TWITTER*

*Vercel CEO Guillermo Rauch*
Two sharp takes: his most-quoted line of the day — _"Coding agents will squeeze every ounce of IKEA effect out of you, if you let them"_ — is a warning that over-relying on agents erodes your sense of ownership over what you're building. He also celebrated a deep performance pass on a site where everything touchable was optimized: painting, layout, WebGPU shaders, blocking scripts, every frame scrutinized. Lessons learned will be published as a public guide.
- <https://x.com/rauchg/status/2068778558672273422|Coding agents & the IKEA effect>
- <https://x.com/rauchg/status/2068838709517336756|Performance deep-dive>

*Box CEO Aaron Levie*
Two big-picture structural takes. First: agents will consume software 100x more than humans ever did — a single agentic query could pull more data than a user touches in a month, making CRM data, documents, and corporate knowledge far more valuable in a headless world. Platforms that build toward that model win. Second: Sakana's Fugu model — a mixture-of-models system that routes tasks to the best expert model under a single API — is already how leading applied AI products build agent harnesses, and the routing layer will accrue massive value as both frontier and OSS models multiply.
- <https://x.com/levie/status/2068851573175021864|Agents use software 100x more than people>
- <https://x.com/levie/status/2068917230570795178|Fugu and the value of routing>

*YC President & CEO Garry Tan*
Tan's thesis: AGI gives you the intelligence, but you still have to collect your personal context to get the real unlock. Personal brain and company brain context is the underestimated advantage at the dawn of usable AGI — which is why he built and open-sourced GBrain.
- <https://x.com/garrytan/status/2068701356358308112|Personal context is the unlock>
- <https://x.com/garrytan/status/2068701357696323769|Why he open-sourced GBrain>

*Thibault Sottiaux (Codex & ChatGPT at OpenAI)*
The Codex PM is running two open feedback loops simultaneously: what's not delightful in the Codex app (3,380 replies and counting), and how users think about banking vs. burning usage resets now that Codex lets them roll over. A rare public window into where the product team is actively listening.
- <https://x.com/thsottiaux/status/2068736857312198928|What should we improve in Codex?>
- <https://x.com/thsottiaux/status/2068792010715324444|Hoarder or burner? Usage resets poll>

*Ryo Lu (Designer at Cursor)*
Cursor's design lead shipped Books — an epub reader inside ryOS — starting in Cursor mobile, then hand-tuning animations and textures until things felt right. Supports any epub file and syncs reading progress with a ryOS account.
- <https://x.com/ryolu_/status/2068923971136098633|Building Books in ryOS>
- <https://x.com/ryolu_/status/2068924375341179347|Works with any epub, syncs progress>

*Peter Steinberger (OpenClaw + OpenAI)*
Two takes: (1) OpenClaw is having its strongest week ever despite the hype dying down — the team improved quality, structured as a non-profit while VC-funded competitors have other agendas, and the numbers are proving it out. (2) He was skeptical about multi-model routing from the start and feels validated in that skepticism.
- <https://x.com/steipete/status/2068961217524490739|OpenClaw's strongest week>
- <https://x.com/steipete/status/2068960117253632160|Skeptical on multi-model routing>

*Zara Zhang (Builder)*
A practical anti-slop rule of thumb: your input (context) should be 3–5x longer than the output. If your input is shorter than the output, you're almost certainly getting slop. The key distinction: it's about _context_, not prompt length.
- <https://x.com/zarazhangrui/status/2068923768500793603|Input length rule of thumb for AI quality>

*Nan Yu (Head of Product at Linear)*
Yu riffed on what it actually takes to ship high-quality software: _"Quality is irrational"_ — it takes an irrational commitment to constantly choose quality, and an irrational level of self-belief that controlling things top-to-bottom beats reaching for common frameworks.
- <https://x.com/thenanyu/status/2068778750800531640|"Quality is irrational">

*Peter Yang (AI content creator, 150K+ readers)*
Shared a builder insight from liu8in: HTML is the LLM's native language for agentic video making. Agents have no visual intelligence on their own, but LLMs can express visual aesthetics through HTML, CSS, and JavaScript with footage and assets layered on top. Example use case: generating a product video from any website URL.
- <https://x.com/petergyang/status/2068755908319236338|HTML as the foundation for agentic video>

*Swyx (AI builder, Latent Space co-host)*
While shopping for insurance for a new "New Media Lab" creative studio, Swyx stumbled on a notable market-share signal: Corgi, the insurance startup, apparently has ~100% penetration across his real estate broker's entire client base. He called it "unheard of" for the insurance industry.
- <https://x.com/swyx/status/2068924451887129055|Corgi's greenfield market share>


*PODCASTS*

*Training Data — "Google DeepMind's Logan Kilpatrick: Why the Model Eats the Harness"*

*The Takeaway:* The agent harness you're building today will be absorbed directly into the model within 12 months — and the alpha will move somewhere else entirely.

Logan Kilpatrick runs Google AI Studio and the Gemini API at Google DeepMind. Over the last year he's watched Google's internal AI strategy consolidate around a single new through line: not Gemini, but *Antigravity* — Google's agent harness ecosystem that bundles an IDE, CLI, SDK, and web experience together. The same harness powering coding in AI Studio now powers agent capabilities in Search, the Gemini app, and Google Cloud. Coding, it turns out, proved to be the general-purpose agent harness.

His most contrarian claim: what the industry calls "the model" is no longer just a set of weights. It's an expanding system built around those weights — tool calling, hosted search, code execution, and the agent harness itself. Scaffolding gets built externally first, then the model absorbs it. _"The scaffolding is oftentimes a couple of steps ahead of what is baked directly into the model, and then what ends up happening is the model eats that scaffolding and it becomes part of the native model system."_ His read: the current harness-as-alpha moment has maybe 12 months left before models just do it natively.

On Google's pace of agentic adoption: deliberately slow, by design. With 13 billion-user products, stewardship matters. Most of Google is still crawling on the agentic scale — Gemini app and Antigravity are the frontier exceptions. The Windsurf acquisition happened specifically because you can't build a great coding model without a real product generating long-running agentic training signal. Google also has 100,000+ engineers dogfooding Gemini and filing feedback — that scale is a competitive advantage few can replicate.

On where narrow superintelligence lands next after coding: math, finance, and science — domains with strong verifiability. He frames the broader trajectory as _"jagged superintelligence"_ — vertical capability peaks appearing in specific domains before general AGI arrives.

<https://www.youtube.com/watch?v=cMAs8z2dehs>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
