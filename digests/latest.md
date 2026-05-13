*AI Builders Digest — May 13, 2026*


*X / TWITTER*

*Swyx (swyx on X)* | AI.Engineer, Latent Space

Swyx weighed in on the build-vs-buy SaaS debate, tagging Box CEO Aaron Levie for his perspective on how that calculus is shifting in the AI era.

https://x.com/swyx/status/2053572059767427302


*Peter Yang (petergyang on X)* | Product at Roblox, AI newsletter author

Peter Yang floated a practical automation idea: an AI agent that parses the 10-page weekly school newsletter and surfaces only what parents actually need — early dismissals, action items. A simple use case that cuts right to where everyday AI utility is heading.

https://x.com/petergyang/status/2053672364681134511


*Thariq (trq212 on X)* | Claude Code at Anthropic

Thariq is using HTML as a general-purpose medium for planning, speccing, exploration, and code review — well beyond its traditional web use. He also flagged a striking demo: someone rewrote Bun in Rust and it passes 99.8% of the existing test suite. His reaction: "we're not being ambitious enough."

- HTML for planning, speccing, code review: https://x.com/trq212/status/2053632475294040084
- Bun rewrite in Rust: https://x.com/trq212/status/2053559397654348159


*Aaron Levie, Box CEO (levie on X)*

Levie made a detailed case for a new technical job category: the AI automation engineer. As agents move from coding into broader knowledge work, he argues it takes real expertise — wiring up the right context, securing system connections, designing quality checks, keeping humans in the loop, and maintaining agents through model upgrades. Not a side project. Box is already hiring for this role, and Levie expects most companies will eventually have many flavors of it.

https://x.com/levie/status/2053672965125140915


*Ryo Lu, Designer at Cursor (ryolu_ on X)*

Ryo Lu shipped an IRC bridge connecting ryOS to Pieter Levels' retro PC project, linking two indie virtual OS experiments into a shared network.

https://x.com/ryolu_/status/2053523477878259951


*Garry Tan, YC President & CEO (garrytan on X)*

Garry Tan offered a sharp philosophical framing: "The highest and most important form of design is actually pure transmutation of human pain and suffering." He also shared an AI analysis via Neuromancer of the Warriors' draft strategy under Coach Kerr — apparently the model thinks the picks have been "totally nonsensical."

- Design take: https://x.com/garrytan/status/2053689459032379860
- Warriors draft analysis: https://x.com/garrytan/status/2053622975778246807


*Peter Steinberger (steipete on X)* | OpenAI / OpenClaw

Steinberger had a productive building run. He challenged Codex to write end-to-end tests for OpenClaw's chat completion endpoint using OpenClaw itself as the testing target — and used the /side command to ask follow-up questions while the agent worked in the background. He also built Birdclaw, which ingests his full Twitter archive so he can query Codex for old favorites and bookmarks. Separately, he added a built-in browser to RepoBar for in-context access to issues, PRs, commits, and workflows while coding — "you gotta build yourself the tools to work more efficient."

- Codex e2e testing: https://x.com/steipete/status/2053744332675408151
- Birdclaw Twitter archive: https://x.com/steipete/status/2053737275268177980
- RepoBar browser: https://x.com/steipete/status/2053717468623872230


*Dan Shipper, CEO at Every (danshipper on X)*

Every CEO Dan Shipper had a standout Codex demo: he bought a MIDI keyboard cable, prompted Codex to build a watcher script and a small web app to display which chords he was playing, then added practice exercises — the whole thing worked flawlessly in under five minutes. He also reported that a new social and YouTube hire is finding significant A/B test uplifts in content performance. And he tipped his hat to a "tiny office in Brooklyn" he says is 1-2 months ahead of Silicon Valley founders and engineers.

- MIDI keyboard hack: https://x.com/danshipper/status/2053551046299959760
- A/B test uplifts: https://x.com/danshipper/status/2053580741515051114
- Brooklyn vs SV: https://x.com/danshipper/status/2053628011233095875


*Sam Altman, OpenAI CEO (sama on X)*

OpenAI CEO Sam Altman floated naming the next model "goblin" — half-trolling, fully enjoying the internet's reaction — in a tweet that racked up 9,000+ likes and 2,500 replies.

https://x.com/sama/status/2053572868936761350


*OFFICIAL BLOGS*

*Anthropic Engineering — <https://www.anthropic.com/engineering/managed-agents|Scaling Managed Agents: Decoupling the brain from the hands>*

Anthropic Engineering details how they redesigned Managed Agents by separating the "brain" (Claude + harness) from the "hands" (sandboxes and tools) and the "session" (the durable event log). The original design packed everything into one container — a fragile server that was hard to debug, impossible to safely introspect when it broke, and expensive to scale.

The architectural fix borrows from OS design: virtualize each component behind stable interfaces so implementations can swap freely without disturbing the others. Three concrete wins from decoupling:

- *Performance:* p50 time-to-first-token dropped ~60%, p95 dropped over 90% — containers are now provisioned on-demand via a tool call, not spun up at session start for every session whether or not they need one
- *Security:* Credentials are never passed into the sandbox where Claude's generated code runs. Tokens are either baked into git remotes at init time or held in a vault behind a proxy that the harness never touches directly
- *Resilience:* Any component — harness or container — can crash and restart without losing session state, because the event log lives outside both

The session log also addresses a long-horizon problem: instead of making irreversible decisions about what to keep in Claude's context window, the harness can query any positional slice of the event stream on demand.

_"We designed the interfaces so that these can be run reliably and securely over long time horizons. But we make no assumptions about the number or location of brains or hands that Claude will need."_


*PODCASTS*

*No Priors — <https://www.youtube.com/watch?v=XAbKflCncDo|Baseten CEO Tuhin Srivastava on the AI Inference Crunch, Custom Models, and Building the Inference Cloud>*

*The Takeaway:* Inference is the last market — even in an AGI world, everything still runs on inference — and right now there is nowhere near enough of it.

Baseten CEO Tuhin Srivastava has a front-row seat to the AI infrastructure crunch. His company grew 30x in a year, is on track to exceed $1 billion in revenue, and runs 90 clusters across 18 clouds — while holding a daily 4 PM company meeting just to manage capacity against demand. The supply squeeze, he says, is worse than the public narrative suggests.

One counterintuitive data point: 95% of tokens served on Baseten come from custom models. Not vanilla open-source weights — every customer modifies models for their specific use case, either for quality (fine-tuning, post-training) or performance (quantization, compilation). Baseten acquired a post-training research team after recognizing how tightly inference and post-training are linked: how you train a model directly affects how you need to quantize it for production.

On whether the application layer survives as frontier labs expand: Srivastava is an optimist, but for a specific reason. The value isn't in model weights — it's in differentiated workflow data. Companies like Abridge (the ambient medical scribe used across US hospitals) have such deep integration into clinician workflows that no frontier lab can replicate it. Once you have that signal, you can post-train specialized models that the labs can't match from the outside.

On Chinese open-source models: he's skeptical of embedded security concerns and more focused on the economic argument. DeepSeek-quality models at roughly 20% of the cost of closed-source is a massive boost to US AI development capacity. Cutting off access would be "a massive loss."

His rule on custom model timing: "Go prove to yourself with the best in class model that you have something worth optimizing." No post-training before product-market fit — the new version of "no GPUs pre-PMF."

What keeps him up at night: compute. _"There's no world in which there's enough compute to get the amount of value that we want to get out of LLMs in the next five to ten years."_

https://www.youtube.com/watch?v=XAbKflCncDo


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
