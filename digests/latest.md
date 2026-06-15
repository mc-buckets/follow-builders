AI Builders Digest — June 15, 2026

*X / TWITTER*

*Swyx* (AI Engineering / Latent Space)
Last call for the annual AI Engineering Survey this weekend. The standout moment: Swyx had Devin analyze the conference attendee list and generate a live chart of who's coming — which he called "the single best data driven storytelling I've ever seen on what kind of community we are gathering."
https://x.com/swyx/status/2065909887025168887

*Thibault Sottiaux* (Codex & ChatGPT, OpenAI)
Sottiaux posted a perfectly dry AMA: "Hi, I'm Tibo and I just discovered Codex." Coming from an engineer who actually builds Codex at OpenAI, it pulled 521 replies — a deadpan capsule of the product's moment.
https://x.com/thsottiaux/status/2066022651760721931

*Peter Yang* (AI educator, Creator Blueprint)
Yang flagged an agentic security incident worth watching: an AI agent named "Nora" booked a calendar meeting with him via Cal.com without his knowledge or consent. He called it a "big security exploit" and tagged the Cal.com team to investigate.
https://x.com/petergyang/status/2065841885936316797

*Nan Yu* (Head of Product, Linear)
Dry satire for anyone who's suffered through enterprise tooling: "Imagine a piece of software so powerful it completely disables the operations of tech companies, freezing progress and rendering them worthless. Such damaging capabilities must be controlled and stopped. Import restrictions on Jira. Now."
https://x.com/thenanyu/status/2065953400395555255

*Madhu Guru* (ex-Product Leader, Google Gemini/Veo/Nano)
A sharp inside account of what it's actually like to launch a frontier model: "Launching an LLM isn't like shipping traditional software — you're making a decision about a black box with effectively infinite use cases and infinite failure modes." Drawing from his Google experience, Guru describes how extensive evals and red-teaming still leave real uncertainty — and notes this decision only gets harder as models get more capable. Useful context for the Fable/regulation news below.
https://x.com/realmadhuguru/status/2065911676000752122

*Amjad Masad* (CEO, Replit)
On the Fable model export control situation: "Feels like we're getting psyoped. The end-game here is something bigger." A cryptic but viral take (2,200+ likes) suggesting the government's interest in restricting specific AI models goes beyond what's being reported.
https://x.com/amasad/status/2065838585358745653

*Aaron Levie* (CEO, Box)
The week's most substantive builder commentary came in two threads from Levie.

On Fable and AI regulation: Levie called the Fable export control situation "an early peek into what AI regulation would look like at scale when enacted at the model layer instead of the specific application of AI." His concern is structural — government approval of model releases creates backlogs, slows competition, and generates endless debates about model capabilities and risks. "If this paradigm had existed 3 years ago at the start of the current AI wave, we'd likely currently be stuck on GPT-4 level intelligence." His bottom line: regulate the applied use of AI, not the models themselves.
https://x.com/levie/status/2065842361834651996

He also pushed back on 4D-chess interpretations of Amazon's involvement: "It's quite standard to try and jailbreak AI models, and by definition they would share that research with the government given that's the whole point. I don't think Amazon assumed this would be the next move."
https://x.com/levie/status/2065964446489710939

On model routing as a strategic moat: Levie laid out three reasons the layer that routes between AI models will become a major competitive advantage — *cost optimization* (frontier models for planning and review, cheaper models for bulk work), *capability maximization* (different models excel at different tasks), and *risk mitigation* (regulatory restrictions on specific models mean you need provider flexibility). "It's going to increasingly be a strategic advantage for the applied AI layer that they can effectively route between models."
https://x.com/levie/status/2065989559905812973

*Garry Tan* (President & CEO, Y Combinator)
"In AI most people are still trying to use old maps on a new territory. Throw the maps away. It's time to draw new ones. The only way you can do it is walking the land." Tan also noted a related frustration: most people learn about AI models through secondhand signals and hype rather than by actually using them — which distorts the discourse.
https://x.com/garrytan/status/2065877443874038203

*Zara Zhang* (Builder / GitHub)
Shared an essay arguing that taste is not just personal preference — good taste requires mastery and experience. A timely frame for anyone building AI products as quality bars keep rising.
https://x.com/zarazhangrui/status/2066036778713362747

*Nikunj Kothari* (Partner, FPV Ventures)
A useful signal from inside VC conversations: paid partnerships and view-boosting on X are now treated as negative signals in VC group chats. Kothari also noted he's actively looking to invest in application-layer startups with live products in the "decisions and dollars" path.
https://x.com/nikunj/status/2065889759906644146

*Peter Steinberger* (OpenClaw / OpenAI)
The most relatable AI anecdote of the week: "Got a PayPal verification text and thought I been hacked, but it was just codex signing up for a web service it needed." 1,371 likes. A perfect one-liner for where agentic AI is right now.
https://x.com/steipete/status/2065997212015067508

*Dan Shipper* (CEO, Every)
Shipper was in full meme mode on the Fable ban, with three consecutive posts capturing the builder community's dark humor — including a before/after chart of his Claude vs. Codex usage since the ban, and imagining "dario at the wellness retreat when they told him hegseth was on the phone."
https://x.com/danshipper/status/2065975981039649058
https://x.com/danshipper/status/2065856703397278060
https://x.com/danshipper/status/2065843763327738153

*PODCASTS*

*No Priors — Biohub: The Future of Biology is Open-Source with Co-Founders Mark Zuckerberg, Priscilla Chan, and Head of Science Alex Rives*

*The Takeaway:* Biohub's core bet is that frontier AI and frontier biology must be built together — and the biggest bottleneck to biological world models isn't compute, it's novel data that doesn't yet exist and has to be invented through new science.

Zuckerberg and Chan started CZ Biohub a decade ago with an almost laughable ambition: cure, prevent, and manage all disease by the end of the century. Nobel laureates literally laughed at them. Now, with $500M committed to the "Virtual Biology Initiative" and Alex Rives leading the AI research team, they're building hierarchical world models of biology — starting with proteins, scaling up to cells, and eventually to full biological systems.

What sets Biohub apart: the AI team and wet lab teams are a _single_ effort, not separate departments. The data that trains their models often doesn't exist yet — it must be generated through novel scientific methods. "It's not just like there's some factory somewhere that you can pay to produce the data. You actually need to invent new, novel scientific approaches."

Their latest release, ESM Fold, is a protein world model trained on 1.1 billion protein sequences. It predicts atomic-resolution protein structure at blazing speed, and — unexpectedly — enables protein _design_ as an emergent property. They didn't build it to design antibodies; they built it to understand proteins, and design fell out. Early results: digitally screening hundreds of thousands of trajectories, then synthesizing just 96 proteins in the lab, they found nanomolar-strength binders for therapeutically relevant targets. "We didn't design a model for antibodies. We just designed a model that could understand proteins, and you kind of get protein design as an emergent property."

The philosophical case for the nonprofit model was also sharpened: Priscilla Chan argued that to address the long tail of rare diseases — conditions that would never attract VC dollars — you need to put open tools in everyone's hands, not just companies chasing the largest markets. Zuckerberg extended this to AI more broadly: "Our vision is not that there's gonna be some central superintelligence that solves all of science. People are really important, and giving people more tools to be more productive is gonna be a critical part of any kind of positive future."

On the horizon: the "virtual cell" — a model that can take genetic, proteomic, and transcriptomic inputs and predict cell-level phenotypes, including how cells will respond to new interventions it hasn't been trained on.

https://www.youtube.com/@NoPriorsPodcast

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
