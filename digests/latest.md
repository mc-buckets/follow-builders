*AI Builders Digest — July 7, 2026*


*X / TWITTER*

*Amanda Askell* — Anthropic philosopher and AI ethicist — shared a pointed observation that went viral (1,382 likes): getting a doctor to give you even a rough probability estimate is "one of life's unnecessary boss battles." Even begging for an interval-valued hunch proves nearly impossible. A small window into broader frustration with how experts resist quantifying uncertainty.
<https://x.com/AmandaAskell/status/2073786264059625897|Tweet>

*Cat Wu* — Claude Code and Cowork PM at Anthropic — shared a concrete workflow for sourcing job candidates: describe the role to Claude Code, kick off a dynamic workflow to find 100 candidates with LinkedIn, Twitter, blog, podcast links, and a one-line pitch each, have Claude email you an artifact, then lock the laptop and review the list on your phone later. A real demonstration of letting agents do the legwork end-to-end.
<https://x.com/_catwu/status/2073806626965049686|Tweet>

*Thariq* — Claude Code engineer at Anthropic — posted a wry riff on San Francisco tech culture: updating the phrase "God gave me a sign" to "I was acasually influenced by the ASI at the end of time to maximize EV for humanity."
<https://x.com/trq212/status/2073956140610924936|Tweet>

*Nan Yu* — Head of Product at Linear — pushed back on two popular patterns. First: "Bragging about running 10 Claude code tabs is just theater." Second: the "real-time strategy game" model of managing AI agents is a dead end — AI that is ancient by current standards already out-micros human players to an extreme degree. Managing agents like an RTS commander is not the right mental model.
<https://x.com/thenanyu/status/2073920959011074292|Tweet> · <https://x.com/thenanyu/status/2073920326304460847|Tweet>

*Sam Altman* — OpenAI CEO — in a widely shared tweet (11K+ likes), compared his toddler putting two words together for the first time to GPT-5.6 discovering new math: "approximately equally amazed by both cognitive feats." Equal parts parenting milestone and a casual confirmation that GPT-5.6 is doing novel mathematical discovery.
<https://x.com/sama/status/2073791666553844074|Tweet>

*Garry Tan* — YC President and CEO, posting from Osaka — made two connected observations. Japan's 30 years of zero growth produced the world's best trains, service, and craft: "When you can't compete on more, you compete on better." He then connected it to the AI moment: "The real constraint on human wealth was never resources. It was good ideas for how to serve one another, and the leverage to act on them. We just deleted the leverage constraint for everybody. Now it's only the ideas."
<https://x.com/garrytan/status/2073881438123110512|Tweet> · <https://x.com/garrytan/status/2073881439700168925|Tweet>

*Dan Shipper* — CEO of Every — posted two jokes about Fable's ultracode mode. First: "me: change this button color / Fable: sure I just spun up a fleet of 100 agents to get that done for you." Then a follow-up showing Fable running in "make no mistakes" mode. Dry humor that captures real anxiety about agent overkill for simple tasks.
<https://x.com/danshipper/status/2073764166700048480|Tweet> · <https://x.com/danshipper/status/2073894034225897602|Tweet>

*Nikunj Kothari* — Partner at FPV Ventures — questioned the standard VC pitch meeting format: still waiting for a founder who requires investors to have actually used the product and come with two pieces of feedback before getting a Zoom. "What alpha do you get from hearing the same story again?" He argues a product brainstorm or just getting to know each other would be far more productive than re-hearing a rehearsed deck.
<https://x.com/nikunj/status/2073903310982218088|Tweet>

*Zara Zhang* — developer and builder — resurfaced a Claude Code skill she built for understanding codebases, noting it is back in vogue now that code comprehension is a hot topic.
<https://x.com/zarazhangrui/status/2073768913310200310|Tweet>

*Peter Yang* — AI tutorial creator — is 1,500 subscribers away from 100K on YouTube, with his birthday on July 9. He's asking the community to help him hit the milestone before then.
<https://x.com/petergyang/status/2073930836551032858|Tweet>

*Matt Turck* — VC at FirstMark Capital — shared a humorous take on AI agent reliability with the caption: "when I ask my AI agent to 'make no mistakes.'"
<https://x.com/mattturck/status/2073972907491865062|Tweet>


*PODCASTS*

*No Priors — "Really Big Test-Time Compute in AI Changes Benchmarks, Safety and Research with OpenAI Research Scientist Noam Brown"*

*The Takeaway:* AI benchmarks are fundamentally broken because they don't control for how much compute a model is given to think — and that same blind spot is quietly undermining safety evaluations across the entire industry.

Noam Brown is an OpenAI Research Scientist and one of the original architects of inference-time scaling. His game-playing AI work (Pluribus, Libratus) proved years ago that thinking harder at inference time could beat the best human poker players in the world.

His core argument: every model release comes with a "benchmark grid" showing performance as a single number. That number is meaningless without specifying the compute budget. GPT-5.5 looked only marginally better than 5.4 on paper — until people realized 5.5 is simply more efficient. At equal compute budgets, it is a substantial jump. The right way to present benchmarks is with an x-axis: tokens, cost, or time.

The problem runs deeper than benchmarks. AI safety evaluations — the "responsible scaling policies" and "preparedness frameworks" labs use to check for dangerous capabilities — were designed before test-time compute scaling mattered. They ask what a model _can_ do, not what it can do with $10 million of inference budget. As Brown puts it: _"The capability of the model is a function of how much money you put into it, basically."_ No existing framework addresses what budget to test at.

Meanwhile, modern models can run useful agentic work for weeks. OpenAI's internal model disproved the Erdős unit distance conjecture — a long-standing math problem — at a relatively low compute budget. Brown estimates a general-purpose scaffold with $100K in compute could have done the same. Nobody had tried, because nobody had asked what $100K of inference gets you on GPT-5.5.

On fast takeoff: Brown is skeptical of an overnight intelligence explosion. Time itself is the bottleneck. If unlocking full model capability requires massive inference compute, everything is rate-limited by how long the models can run. The researchers grinding at the frontier are the constraint — not a sudden recursive explosion.

https://www.youtube.com/watch?v=AZrU6y3pUcU


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
