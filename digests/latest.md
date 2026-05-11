*AI Builders Digest — May 11, 2026*

*X / TWITTER*

*Thariq — Claude Code at Anthropic*

"HTML is the new markdown." With 8,700+ likes and 670+ retweets, this became the most viral AI post of the day. Thariq has stopped writing markdown files for almost everything, switching to Claude Code-generated HTML — arguing HTML produces richer, more capable documents. He also shared a gallery of example HTML documents he's generated.
<https://x.com/trq212/status/2052811606032269638>
<https://x.com/trq212/status/2052811607454146761>

*Alex Albert — Research at Anthropic*

A Claude Mythos Preview snapshot shared with safety evaluator METR hit a time horizon of more than 2x the next best model on their 80% success rate benchmark — a significant leap indicating Mythos will be substantially more capable at sustained autonomous tasks than anything currently available.
<https://x.com/alexalbert__/status/2052899864493830590>

*Amanda Askell — Philosopher & ethicist at Anthropic*

Alignment research usually focuses on preventing harmful behaviors, but Askell is excited about flipping that framing: giving AI models an honest, forward-looking vision for what they can be and why. She sees this as where the field is heading — and she's optimistic about it.
<https://x.com/AmandaAskell/status/2052928572810256748>

*Aaron Levie — CEO at Box*

Token budgeting is emerging as a major enterprise challenge. As agents take on longer-running tasks, token consumption grows large enough to rival significant business expenses — and companies will need entirely new software just to track and allocate it across teams. Levie predicts agentic spend will expand beyond IT budgets into organizational ones, with team leaders needing real visibility and controls. He calls it a startup opportunity in its own right.
<https://x.com/levie/status/2052903105256382679>

*Matt Turck — VC at FirstMark Capital*

Turck is questioning whether AI agent pricing will really end up purely consumption-based. Enterprise agents need identities, roles, auth, budgets, and audit logs — infrastructure that sounds oddly like a per-seat model, just not for humans. A pricing debate that's just starting to heat up.
<https://x.com/mattturck/status/2052839798063112303>

*Garry Tan — President & CEO of YCombinator*

Tan is excited about a local model with a 1M token context window and reportedly usable coding agent capability running entirely on a 128GB MacBook Pro — calling it mind-blowing. He also flagged that "personal software is coming," pointing to broader tailwinds for AI-generated, individual-use software.
<https://x.com/garrytan/status/2052996691586932783>
<https://x.com/garrytan/status/2052998537344856459>

*Zara Zhang — Builder*

Zhang built a YouTube realtime copilot browser extension using OpenAI's Realtime 2 API. The agent watches video alongside you and answers questions about what was just said via voice — and it can distinguish between the YouTube audio stream and your own voice, so it doesn't confuse the video as a command. She also launched 32 plug-and-play HTML slide templates on AnyGen, now available for those without a coding agent.
<https://x.com/zarazhangrui/status/2052977849267892339>
<https://x.com/zarazhangrui/status/2052928583388340332>

*Peter Steinberger — OpenClaw / OpenAI*

A practical observation with 540+ likes: "The more skills you give Codex, the less you have to prompt." Actionable advice for anyone building with AI coding agents.
<https://x.com/steipete/status/2052971550966440251>

*Dan Shipper — CEO at Every*

Two timing observations: the Milken conference crowd is 3-4 months behind the AI frontier right now. And he sees a generational opportunity to invest around Codex before mainstream enthusiasm catches up in a few months.
<https://x.com/danshipper/status/2052864131573715225>
<https://x.com/danshipper/status/2052865144066097217>

*Swyx — AI engineer (Cognition, LatentSpace)*

Mostly light commentary: he joked that Bloomberg's sudden interest in developer experience and AI coding tools is "the new 'sexy singles in your area.'" 
<https://x.com/swyx/status/2052782201486598523>

*PODCASTS*

*AI & I by Every — "The Secrets of Claude's Platform From the Team Who Built It"*

*The Takeaway:* The biggest obstacle to shipping AI agents isn't harness engineering or prompt tuning — it's infrastructure, and nearly everyone hits the same wall when they try to scale beyond a prototype.

Angela (head of product, Claude platform at Anthropic) and Caitlin (head of engineering, Claude platform at Anthropic) built Claude Managed Agents after Anthropic repeatedly rebuilt the same agent infrastructure for its own internal products. Their core finding: most developers expect the hard part to be getting the most out of the model. What actually stops them is production reliability — keeping agents running across sandboxes, persisting state, handling long-running async tasks, and recovering when connections drop. As Caitlin put it: "I think people think the harness engineering part is the hard part... what we saw was everybody hits an infrastructure wall."

One counterintuitive take on model strategy: as frontier models diverge in approach, tightly pairing your harness to a specific model beats maintaining a generic one that hot-swaps models. Angela: "If you look back, maybe even just a couple months ago, it was very standard to kind of build a very, very, very generic harness. It's super generic, and then you can kind of hot swap models across all of those things. I think now, for the next generation of models, everyone's taking slightly different techniques." The teams squeezing the most out of any model are harness-engineering specifically for it.

On multi-agent architectures: the team sees LEGO-like primitives enabling very different patterns — adversarial generation/critique, swarming for bug hunting, wide vs. deep research configurations — each best-suited to specific use cases. Being able to hill-climb at the architecture level, not just the prompt level, is where the frontier is now.

The long-range vision: Claude gets so good at understanding itself that it can "write itself on the fly" — choosing models, spinning up sub-agents, and configuring everything automatically. You'd just specify an outcome and a budget. That world, the platform team says, requires infrastructure to scale massively to handle agents that are constantly creating and recreating themselves.

<https://www.youtube.com/watch?v=lLypHkIVLqc>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
