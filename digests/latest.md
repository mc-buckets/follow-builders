*AI Builders Digest — June 29, 2026*


*X / TWITTER*


*Swyx* — affiliated with Cognition, Temporal, and the AI Engineer community

Swyx made a pointed case for changing how open model benchmarks report inference budgets: since open models offer far better dollar-per-token value than closed APIs, evals should measure thinking levels by *dollar* spent on inference providers — not raw token counts. This would level the playing field for open models in side-by-side comparisons. He also hosted an impromptu AI Engineer pre-show floor tour and AMA.
- <https://x.com/swyx/status/2070949306060931312|On eval budget reporting for open models>
- <https://x.com/swyx/status/2070971772548366788|AI Engineer pre-show floor tour and AMA>


*Thibault Sottiaux* — Codex & ChatGPT at OpenAI

A significant batch of Codex improvements shipped: smoother handling of long threads, a hoverable navigation rail for jumping between turns, improved settings search with host-filtering and custom-provider options, zoom-level fixes for tooltips and dialogs, Slack paste that preserves markdown (bullets, bold, code, links), and — the highlight — a dedicated Pets panel.
- <https://x.com/thsottiaux/status/2071071289247244481|Codex improvements>


*Peter Yang* — AI tutorial creator and builder

Yang shared his "Hermes" personal agent setup: a weekly health-check email that pulls data from his Withings smart scale, Fitbit, Google Health, an MCP server, and a fitness app he vibe-coded himself. He also pushed back on rigid problem escalation frameworks — waiting to reach "level 5" before surfacing a burning fire leaves you worse off than someone who looped people in on day one.
- <https://x.com/petergyang/status/2070906940352520477|Hermes health-check agent>
- <https://x.com/petergyang/status/2071058953115767275|On problem-solving escalation frameworks>


*Guillermo Rauch* — Vercel CEO

Rauch issued a security warning: Mythos/Sol AI cybersecurity capabilities are equally effective for offense and defense. If adversaries acquire equivalent tools, companies with unpatched vulnerabilities are exposed. His recommendation: run deepsec or similar harnesses with frontier models against your own systems proactively.
- <https://x.com/rauchg/status/2071047674187714830|Cybersecurity AI warning>


*Aaron Levie* — Box CEO

Levie laid out the opportunity for the "applied AI layer" — companies that sit between foundation models and enterprise workflows. By running domain-specific evals, tuning UX, and supporting adoption through field engineers, this layer can deliver *more* intelligence per dollar than raw API access. He sees major horizontal and vertical opportunities here.
- <https://x.com/levie/status/2070937863806751154|On the applied AI layer opportunity>


*Matt Turck* — VC at FirstMark Capital

Turck traced the history of smart glasses from Google Glass (2013: "you really want this") through Microsoft HoloLens, Meta Ray-Bans, Apple Vision Pro, and now Snap in 2026 ("ok but this time for real") — each met with near-universal skepticism. A wry observation about the category's stubborn persistence despite consistent rejection.
- <https://x.com/mattturck/status/2070972014945243622|Smart glasses: a history>


*Zara Zhang* — builder and product storyteller

Zhang hit 10,000 GitHub followers despite barely knowing how GitHub worked a year ago — still writing no code by hand. She builds side projects by connecting technology to real user problems and telling stories about them, noting she's not an engineer in the traditional sense.
- <https://x.com/zarazhangrui/status/2070982013822333007|10k GitHub followers milestone>


*Peter Steinberger* — co-founder at OpenClaw, working with OpenAI

Steinberger flagged a consistent historical pattern: access restrictions rarely stop determined users. The implication for AI access policy is clear — rate limits and paywalls mainly inconvenience ordinary users while barely slowing down the most motivated ones.
- <https://x.com/steipete/status/2071063588329193551|On access restrictions>


*OFFICIAL BLOGS*


*Claude Blog — Claude Code now supports artifacts*

Claude Code can now generate live, shareable visual pages — artifacts — directly from a session. These work for PR walkthroughs, incident timelines, dashboards, license audits, and architecture maps. They update in place when Claude republishes, so all viewers see changes immediately at the same URL. Artifacts keep full version history and are private to your org by default, with admin controls for access and retention.

The value prop: instead of copy-pasting agent findings into Slack threads, teams share one self-updating link. Claude builds artifacts from full session context — codebase, connectors, and conversation — without requiring external data sources. Available in beta for Claude Team and Enterprise orgs via the CLI and desktop app.

<https://claude.com/blog/artifacts-in-claude-code|Read the full announcement>


*PODCASTS*


*Training Data — Memory and Continual Learning: Engram's Dan Biderman and Jessy Lin*

_The Takeaway:_ The key bottleneck for making AI models more useful isn't raw intelligence — it's teaching models your specific context, and that requires actual training, not just better prompting.

Dan Biderman and Jessy Lin, cofounders of Engram (a neurolab focused on memory and continual learning), argue that context engineering and RAG are hitting real limits. As people collectively generate tens of millions of tokens per day, constantly re-reading files and rebuilding context windows will become prohibitively expensive. Their alternative: apply the same training pipelines frontier labs use for math and code to company-specific knowledge.

The efficiency numbers make the case. A model that has genuinely learned your company's context can answer questions in 100 tokens that would otherwise consume 100,000 tokens of RAG context — a 100x reduction. Even more telling: the KV cache for a single Wikipedia article requires ~80GB of GPU memory, while the full weights of a 70B LLaMA model — encoding the compressed knowledge of the internet — take only ~100GB. Gradient descent is dramatically more bit-efficient than storing state.

"Why are you reading the same files over and over again, even in the same query? Definitely across people in the same company, they're running the same queries on the same documents over and over again. That should be something the model just knows. In the same way you ask an employee, they don't type into the search box, 'What was I working on yesterday?' They just know." — Dan Biderman

Engram is currently working with Notion, Microsoft, and Harvey — large knowledge-work platforms where teams interact with agents over long periods. Their vision: models that behave like a tenured employee who understands your priorities and ways of working, not just a search engine over your files.

https://www.youtube.com/watch?v=aiR7F4jqjXY


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
