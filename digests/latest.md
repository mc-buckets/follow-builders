AI Builders Digest — October 17, 2026

*X / TWITTER*

*Boris Cherny — Claude at Anthropic*
Cherny highlighted Anthropic's progress on prompt injection and announced a partnership with Gray Swan to host a competition around it. The framing: as AI agents take on more real-world tasks, solving prompt injection becomes urgent across the industry, not just for Anthropic.
https://x.com/bcherny/status/2110791698611855624

*Thibault Sottiaux — Codex & ChatGPT at OpenAI*
Sottiaux posted a cryptic line that lit up replies: "Either we are out of ideas or we are cooking. Time will tell." (2,700+ likes, 899 replies.) He also noted he now programs in French — presumably a flex on the multilingual capabilities of whatever he's building.
https://x.com/thsottiaux/status/2110971985417441512
https://x.com/thsottiaux/status/2110864861119045840

*Aaron Levie — CEO at Box*
Levie dropped a long-form take on where AI automation is heading: we've been in "augmentation mode" for 3+ years, but the next shift is agent swarms running in the background with no human in the loop. He argues most knowledge work is constrained by moving data, reviewing documents, and processing logs — tasks AI can now parallelize at scale. Separately, he called Meta's release of the Muse open-weights model "a huge step forward for OSS" and predicted it will further accelerate AI diffusion as enterprises mix frontier models with cheaper post-trained ones.
https://x.com/levie/status/2110622982762803449
https://x.com/levie/status/2110787013809222141

*Aaron Levie also on the tech optimism wave:*
"So in fact we actually can get robots, flying cars, superintelligence, fast internet on planes, space travel, space colonies, orbital data centers, unlimited energy, likely cures for nearly every disease, and more all in our life times."
https://x.com/levie/status/2110975373219688624

*Garry Tan — President & CEO at Y Combinator*
Tan flagged the Meta open-weights model drop as a signal: "Open weight models rising." He also co-hosted a Garry's List event with Metis65.
https://x.com/garrytan/status/2110838867213668587

*Matt Turck — VC at FirstMark Capital*
Turck promoted a deep-dive MAD Podcast episode with Diogo Almeida, CEO of TypeSafe (the company behind Jev), covering what Jev actually is, why RLHF creates problems for automation, how copycats are missing the hard part, and why benchmarks mislead users. Topics include RLHF vs. RLCD, machine-native AI, composability, and why classification might be "AI-complete."
https://x.com/mattturck/status/2110799882952831302

*Nan Yu — Product at Codex, OpenAI*
Nan challenged the shallow definition of taste: "Taste does not mean taste in aesthetics. That is the shallowest definition of taste, and uninteresting because it's so common." A subtle but pointed pushback on how "taste" gets used in product conversations.
https://x.com/thenanyu/status/2110730151222980849

*Dan Shipper — CEO at Every*
Shipper riffed on the limits of AI interpretability with a Good Will Hunting-style monologue: knowing a neuron lights up for the Eiffel Tower doesn't tell you what the model is planning. Sharp critique of the idea that mechanistic interpretability alone gets us to alignment. Also dropped that something at Every went live.
https://x.com/danshipper/status/2110831666587713810

*Aditya Agarwal — General Partner at SPC*
Agarwal flagged Goodfire as potentially one of the most important companies out of SPC: "They are showing that interpretability and alignment can be approached as engineering problems." Strong conviction call.
https://x.com/adityaag/status/2110779602453066224

*Zara Zhang — Builder*
Zhang built a Harry Potter-style newspaper where images come to life — "The Toddler Times" — a fun creative AI demo. She also shared an Ezra Klein quote worth saving: "Never underestimate your audience's intelligence and never overestimate their prior knowledge."
https://x.com/zarazhangrui/status/2110984552743309530
https://x.com/zarazhangrui/status/2110815456458412179


*PODCASTS*

*The MAD Podcast with Matt Turck*
*Jev: The AI That Makes Decisions, Not Text - and Why It Changes Everything (Diogo Almeida)*

*The Takeaway:* The next major AI unlock isn't smarter chatbots — it's AI that plugs reliably into software as a decision-making layer, not a text generator.

Diogo Almeida, CEO of TypeSafe (the company behind Jev), makes a case that the AI world has been optimizing for the wrong thing. RLHF — reinforcement learning from human feedback, which Almeida co-invented at OpenAI — trained models to sound great, not to be reliable. Models became "95% Einstein, 5% Mr. Bean," and the problem is they don't tell you which mode they're in. That unreliability is why chat-based AI has failed to automate most real workflows despite years of hype.

Jev's bet is on what Almeida calls "machine-native AI" — models trained to output decisions and probabilities rather than prose. Instead of writing a giant system prompt and hoping the LLM follows it, you build explicit classifiers for each decision point. These are composable, measurable, and code-compatible. The analogy: logic gates. Software became powerful not through smart gates, but by composing simple ones reliably.

He's dismissive of critics who call Jev "just a classifier": "How does Facebook work? Classifiers. How does TikTok work? Classifiers. How does Google work? Classifiers." The point is that classification is the interface between intelligence and software — and if you get it cheap, fast, and reliable, it spreads everywhere (Jevons paradox, hence the name).

On copycats emerging just weeks after launch: Almeida says they're copying the interface, not the intelligence. Building a reliable system-one model requires years of work on training methodology, data construction, and calibration — not a weekend of wrapping an LLM's output into a probability score.

One direct quote that lands: _"Pre training is a giant dumpster fire of wasting resources."_ (He didn't do it — TypeSafe raised under $40M before their recent $870M round and built on open-weight models.)

https://www.youtube.com/@DataDrivenNYC/videos

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
