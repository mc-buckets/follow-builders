*AI Builders Digest — June 28, 2026*


*X / TWITTER*

*Sam Altman — OpenAI CEO*
Altman announced two model updates in quick succession: the 5.5 instant model used in ChatGPT got a refresh ("I like its vibes"), and GPT-5.6 dropped with the team having "cooked, spicily." He also teased that all-you-can-eat tokens are in the works, though not quite there yet.
- <https://x.com/sama/status/2070612055225483692|5.5 instant model update>
- <https://x.com/sama/status/2070614666288795703|GPT-5.6 announcement>
- <https://x.com/sama/status/2070614769678393846|on unlimited tokens>

*Dan Shipper — Every CEO*
Shipper sounded the alarm on GPT-5.6 Sol: by U.S. government directive, access is currently limited to roughly 20 pre-approved companies — and Every isn't on the list. He supports some government oversight but argues forcefully that democratic access to frontier models is critical for American workers, students, and independent builders. "A world where advanced models are locked up only for use by the employees of AI giants and a select few companies is one where ambitious students, independent builders, and working professionals are denied the tools they need to learn, create, and compete to their fullest potential." He says OpenAI and the government are working toward broader access soon.
- <https://x.com/danshipper/status/2070554118146412979|full post>

*Garry Tan — Y Combinator President & CEO*
Tan fired off a sharp critique of how GPT-5.6 was released, calling it "no way to release a model" and warning that continued releases this way will "salt the ground and kill all innovation by small startups." He also amplified a thread on the dangers of building a "mid startup."
- <https://x.com/garrytan/status/2070699046939820223|on the model release approach>
- <https://x.com/garrytan/status/2070494207102595495|don't be a mid startup>

*Aaron Levie — Box CEO*
Levie is bullish on GPT-5.6: "Going to be very strong for knowledge worker tasks that require heavy tool use and long running agents doing work. We're not hitting any walls in AI progress right now."
- <https://x.com/levie/status/2070563281916620895|on GPT-5.6>

*Peter Yang — AI educator*
Yang raised three sharp questions. He laid out the troubling logic of frontier model gating: publish → get distilled into cheap open source → US companies adopt open source → gate frontier access → US companies innovate less. He also observed that money is flowing to services (with software bundled), not pure-play software — "people want outcomes, not tools." And he dropped a Claude Code UX wishlist: restore mid-task conversation steering, make mobile remote control default-on, fix hotkey accessibility outside submenus, and allow project drag-and-drop in the nav.
- <https://x.com/petergyang/status/2070633838146134219|on frontier model gating>
- <https://x.com/petergyang/status/2070568705365577990|on services vs. software>
- <https://x.com/petergyang/status/2070545325497221248|Claude Code wishlist>

*Thibault Sottiaux — OpenAI (Codex & ChatGPT)*
Sottiaux announced a complimentary usage reset for all Codex users following an unspecified incident. The investigation hasn't shown large-scale user impact, but monitoring is ongoing.
- <https://x.com/thsottiaux/status/2070653282440405046|announcement>

*Guillermo Rauch — Vercel CEO*
Rauch wrote about why agents are uniquely hard to debug: non-deterministic model outputs compounded by the complexity of distributed systems — multiple API calls, sandboxes, rate limits that can fail at any step. He called out observability as a key priority for Vercel's AI stack. He also declared: "The UI for AI is here. It's shadcn."
- <https://x.com/rauchg/status/2070676383135834334|on agent observability>
- <https://x.com/rauchg/status/2070567538040422712|on shadcn as the UI for AI>

*Swyx — AI engineer, Latent Space podcast host*
Swyx took over a new media lab in San Francisco — envisioned as a "third place to make" and "finishing school for technical storytellers." Surprise: it came with a datacenter rack already wired up. He's also co-organizing the first-ever AI FDE (Field Deployment Engineer) miniconference, noting that with both OpenAI and Anthropic launching multi-billion dollar services arms, FDE is "one of the most in-demand disciplines on earth."
- <https://x.com/swyx/status/2070748857441362056|media lab announcement>
- <https://x.com/swyx/status/2070606851377672675|FDE miniconference>

*Cat Wu — Anthropic (Claude Code + Cowork)*
Wu highlighted split screen as one of her favorite Claude Code desktop features.
- <https://x.com/_catwu/status/2070613405237432766|split screen post>

*Aditya Agarwal — South Park Commons General Partner*
The former Dropbox CTO and early Facebook engineer shared an unexpected social side effect of AI: he now has zero tolerance for shallow human interactions and craves deeper connection. His prediction: the world becomes both smaller and richer in relationship depth — agents handle everything else.
- <https://x.com/adityaag/status/2070621064271688021|on AI and human connection>

*Nikunj Kothari — FPV Ventures Partner*
Kothari pushed back on "AI has no taste" criticism: most critics have never built anything. Real taste comes from iteration — like a chef cooking a hundred dishes before the 101st one carries all the lessons. He believes AI has a genuine shot at developing taste over time. He also shouted out seed founders building in "not-so-hot" categories.
- <https://x.com/nikunj/status/2070649602953576825|on AI taste>
- <https://x.com/nikunj/status/2070532689392980369|for seed founders in unglamorous categories>

*Peter Steinberger — OpenClaw + OpenAI*
Steinberger vented a familiar developer frustration: Apple notarization breaks multiple times a year, forcing manual logins to accept new legal agreements. Nearly 1,000 likes says he's not alone.
- <https://x.com/steipete/status/2070626638887555227|on Apple notarization>

*Nan Yu — Linear Head of Product*
Yu proposed a "Secret level 6" to problem-solving frameworks: recognize when a problem isn't worth solving and leave it alone. His take: orgs full of people who know when _not_ to act win by avoiding side quests.
- <https://x.com/thenanyu/status/2070656348488937889|on knowing when not to solve>

*Zara Zhang — Builder*
Zhang recommended Borumi as an underrated video recording and editing tool — "Screen Studio + Descript + CapCut all in one." She also noted, wryly: "You do not need God to write your emails."
- <https://x.com/zarazhangrui/status/2070584764315402405|on Borumi>
- <https://x.com/zarazhangrui/status/2070589563429691698|on AI for email>


*PODCASTS*

*No Priors — "Why Traditional Benchmarks Fail Modern AI Models with OpenAI Research Scientist Noam Brown"*

<https://www.youtube.com/watch?v=AZrU6y3pUcU>

*The Takeaway:* Current AI benchmarks are fundamentally broken because they treat model capability as a fixed number rather than a function of compute budget — with serious implications for both product comparisons and AI safety.

Noam Brown is an OpenAI Research Scientist who pioneered inference-time scaling — the idea of letting models "think longer" to get better answers, first proven in poker AI and now central to every frontier model. His core argument: the benchmark grid everyone publishes (one number per benchmark per model) is misleading because it doesn't control for how much compute goes in.

GPT-5.5 is the clearest example. On the standard grid it looked only marginally better than 5.4. But 5.5 is dramatically more compute-efficient — it reaches better answers with less thinking time. Once you normalize for compute budget, it's a substantial jump. The right way to evaluate models now: plot performance as a function of tokens, cost, or time — not a single number. "If you give it a budget of $10,000, it can do a lot more than what it can do with a budget of $10. Give it a budget of $10,000,000, it can do even more. And so at what budget should you evaluate these models? The policies that exist today don't really address that question."

This problem runs deeper on the safety side. Preparedness frameworks and responsible scaling policies were built in the ChatGPT era, before test-time scaling existed. A model that appears safe at a $10 budget may not be at $10 million — and current policies largely ignore this question.

On the bigger picture: Brown is skeptical of an overnight intelligence explosion. Because unlocking maximum capability requires massive test-time compute, time itself becomes the bottleneck — no sudden discontinuous jump. He sees AI as gradually transforming what researchers do rather than replacing them. Models still lack "research taste" — they can optimize existing algorithms 1,000x but can't yet invent novel ones.

One striking data point: OpenAI used an internal model to disprove the Erdős unit distance conjecture — a decades-old open math problem — "at a budget that was dirt cheap." With some scaffolding, GPT-5.5 can reportedly reach the same result. Nobody knew because nobody had tried putting serious compute toward it. His parting advice: stop trusting benchmark grids, and if you wrote off AI after a bad 2023 experience, revisit — the gaslighting problem is largely fixed.


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
