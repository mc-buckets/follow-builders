AI Builders Digest — May 3, 2026


*X / TWITTER*


*Swyx* (AI engineer; affiliations include Cognition, Temporal, and the Latent Space podcast)
Pitched a Chrome extension idea for image input boxes: let users generate simple text or draw with tldraw — no AI required — then optionally use those inputs to generate an image at the right proportions. He also fired off a quick observation in a reply: OpenAI Codex makes a better Slack search tool than Slack's own AI search feature.
- <https://x.com/swyx/status/2050460622706626740|Chrome extension pitch for image inputs>
- <https://x.com/swyx/status/2050432398161264664|Codex beats Slack AI search>

*Peter Yang* (Product at Roblox; practical AI newsletter, 140K+ readers)
Found his first broken Codex feature. Also bought a $3,000 MacBook Pro "to run local models" — his own emoji suggests the justification was already suspect. Also shared the feeling of a genuine Codex breakthrough.
- <https://x.com/petergyang/status/2050406287008268450|First broken Codex feature>
- <https://x.com/petergyang/status/2050394924395434233|MacBook Pro for local models>
- <https://x.com/petergyang/status/2050378287348899962|Codex breakthrough>

*Replit CEO Amjad Masad*
Celebrated Replit's 10th birthday by making the platform totally free for 24 hours starting 5am PT — tracing the founding mission to make coding accessible for all the way back to 2011.
- <https://x.com/amasad/status/2050479551537619413|Replit turns 10>

*Box CEO Aaron Levie*
Two sharp enterprise takes. First: Atlassian's strong results shouldn't surprise anyone. When there are 100x more agents than people, the systems those agents rely on — security, compliance, workflows, data storage — grow with them. If the world generates more code, reviews more contracts, and processes more invoices, the underlying systems of record only go up in value. Second: enterprises outside Silicon Valley aren't trying to replace workers. They're trying to break bottlenecks — ship more product, speed up onboarding, better serve customers. AI is also bringing technical capability to companies that could never afford it before. Where cost-cutting does happen, it typically funds another area of growth.
- <https://x.com/levie/status/2050295657836277764|On agents and the future of software>
- <https://x.com/levie/status/2050240083325030404|Enterprises want augmentation, not replacement>

*YC President and CEO Garry Tan*
Pushed back hard on proposed California asset seizure measures, warning they'd drive out billionaires and shift billions in lost tax revenue onto the middle class.
- <https://x.com/garrytan/status/2050365216421241152|Against California asset seizure>

*Zara Zhang* (builder)
Shared a reframe for working with coding agents: she treats them as cofounders, not employees. "I don't just give orders. I present problems, describe the situation, and ask for their opinion." The implication: agents do better work when you give them context and ask for judgment, not just instructions.
- <https://x.com/zarazhangrui/status/2050326543797469415|Agents as cofounders, not employees>

*Nikunj Kothari* (Partner, FPV Ventures)
Built a house-hunting report tool on Railway, Conductor Build, and Claude — and hit $36,500 in ARR. Each AI-generated report costs $8–9 to produce, so he's selling mostly at cost. Actively looking for house hunters to try it in exchange for feedback.
- <https://x.com/nikunj/status/2050407946438467878|$36,500 in ARR>
- <https://x.com/nikunj/status/2050353986742698400|Built with Railway, Conductor, and Claude>
- <https://x.com/nikunj/status/2050355231486316818|Promo codes for feedback>

*Peter Steinberger* (OpenClaw + OpenAI)
Brief but clear endorsement of Codex's new /goal feature: "The new /goal feature in codex slaps."
- <https://x.com/steipete/status/2050275598178586921|On Codex /goal>

*Dan Shipper* (CEO, Every)
A sharp asymmetry observation: "models know more than any individual human. but any individual human learns faster than models do." The implication is that human learning velocity — not current knowledge — is the durable edge against AI.
- <https://x.com/danshipper/status/2050304359024759242|On the human advantage over models>

*Aditya Agarwal* (General Partner, South Park Commons; ex-CTO, Dropbox)
Clean founder maxim: "The best way to kill your company? Focus on everything except the product."
- <https://x.com/adityaag/status/2050229509840900434|On product focus>

*Sam Altman* (CEO, OpenAI)
Plans to host bigger events for future releases after more people than expected wanted to attend a recent one.
- <https://x.com/sama/status/2050427808456077541|On future release parties>

*Claude* (Anthropic)
Code with Claude, Anthropic's developer conference, returns next week — with sessions for builders at every level of experience with Claude Code.
- <https://x.com/claudeai/status/2050252933866930339|Code with Claude conference>


*OFFICIAL BLOGS*


*Anthropic Engineering — An update on recent Claude Code quality reports*
A postmortem on three separate issues that degraded Claude Code quality between March and April — all resolved as of April 20 (v2.1.116).

The three problems: (1) In early March, the default reasoning effort was quietly downgraded from high to medium to reduce latency. Users noticed the intelligence drop, and the change was reverted April 7. (2) On March 26, a caching optimization introduced a bug that stripped Claude's prior reasoning from sessions after they went idle, making it seem forgetful and repetitive. Fixed April 10. (3) On April 16, a system prompt instruction capping response length caused a 3% drop in coding quality across evals — reverted April 20. Because each change hit a different slice of traffic on a different schedule, the combined effect looked like broad, inconsistent degradation.

Going forward: Anthropic is adding stricter controls on system prompt changes, broader per-model evals for every prompt change, longer soak periods for intelligence-affecting changes, and usage limit resets for all subscribers. They launched _@ClaudeDevs_ on X for more transparent product communication.
<https://www.anthropic.com/engineering/april-23-postmortem|Read the full postmortem>

*Claude Blog — New connectors in Claude for everyday life*
Claude's connector directory has grown to 200+ integrations since launching in July 2025. Today it expands beyond work tools to everyday life apps: AllTrails, Audible, Booking.com, Instacart, Intuit Credit Karma, Intuit TurboTax, Resy, Spotify, StubHub, Taskrabbit, Thumbtack, Tripadvisor, Uber, Uber Eats, and Viator. Claude now proactively suggests relevant connectors mid-conversation based on what you're doing. Data from connected apps is not used to train models, no paid placements exist in recommendations, and Claude will ask before taking any action on your behalf (booking, purchasing).
<https://claude.com/blog/connectors-for-everyday-life|Read the announcement>

*Claude Blog — Built-in memory for Claude Managed Agents*
Memory on Claude Managed Agents is now in public beta. Agents learn across sessions using a filesystem-based memory layer — so Claude uses the same bash and code execution capabilities it already has rather than a separate retrieval system. Memories are stored as exportable files with full API access, audit logs, version history, and rollback. Enterprise deployments can scope read-only org-wide stores alongside per-user read/write stores, with multiple concurrent agents. Early results: Rakuten cut first-pass errors by 97%; Wisedocs sped up document verification by 30%.
<https://claude.com/blog/claude-managed-agents-memory|Read the announcement>


*PODCASTS*


*No Priors — Baseten CEO Tuhin Srivastava on the AI Inference Crunch, Custom Models, and Building the Inference Cloud*

_The Takeaway:_ The real AI infrastructure play isn't raw compute — it's owning the full loop between inference and post-training, because that loop is what lets companies compound model quality over time.

Tuhin Srivastava has grown Baseten 30x over the past year, on pace for $1B+ in revenue in 2026. The counterintuitive stat he leads with: 95% of tokens on Baseten run on _custom_ models — not vanilla open source. Enterprises aren't just spinning up Llama. They're post-training on proprietary data and compiling models for specific workloads.

His framework for why the application layer survives: it's not about the model, it's about workflow signal. Companies like Abridge (ambient clinical scribing) have so many steps and user interactions embedded in their product that no frontier lab can replicate that signal. "To the extent that [value] is encoded in workflows, that is where they will be able to develop moat."

On when to actually invest in custom models: "Go find, go prove to yourself with the best in class model that you have something worth optimizing." His frame — "no post training pre product market fit" — is a direct analog to "no hiring before PMF." Don't customize until you've proven the thing works.

Baseten acquired Parzed, a post-training research team that was already a Baseten customer, to close the loop between inference and customization. Their core product thesis: inference generates data, data enables evals, evals drive post-training, better models drive more inference. The goal is making that cycle a continuous process rather than a discrete, one-off project.

<https://www.youtube.com/watch?v=XAbKflCncDo|Watch on YouTube>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
