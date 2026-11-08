AI Builders Digest — November 8, 2026

*X / TWITTER*

*Swyx* (Latent Space Pod, smol.ai, Cognition)
Committing to weekly Anthropic IPO coverage alongside VC writer Jamin Ball, dusting off his equity hedge fund analyst background to track one of the most anticipated tech IPOs alongside his AI Engineer lens.
<https://x.com/swyx/status/2118905788915982341|Tweet>

*Thibault Sottiaux* (OpenAI Codex & ChatGPT PM)
Went viral Friday with a simple "It's Friday" post (5.7K likes, 1.6K replies). Followed up with "Get me out of the basement" alongside a demo clip, hinting something is cooking internally — and noting "Quite cool what you can do with a single prompt these days."
<https://x.com/thsottiaux/status/2118871902366441879|It's Friday> · <https://x.com/thsottiaux/status/2118938956301779171|Get me out of the basement>

*Peter Yang* (AI tutorials creator)
Flagged a consolidation trend: multi-model apps like Cursor are getting acquired by labs, while the ones staying independent are going open source. Wonders if enterprise demand for model-agnostic tools will keep the category alive. Also teasing a "mind-blowing" upcoming episode with a guest who may surpass Steipete as his most impressive interview yet.
<https://x.com/petergyang/status/2118811231545122998|On lab consolidation> · <https://x.com/petergyang/status/2118852799094206787|Episode teaser>

*Thariq* (formerly Claude Code at Anthropic)
Identified a pattern worth watching: creator apps like Instagram Edits and Roblox Studio are now shipping with built-in MCPs, letting agents handle work while power users continue in familiar tools. This "agent + MCP + power user" combo is becoming a blueprint. Also posted a viral quip (2.2K likes): "too many people building agents and not enough people using software to improve the quality of fish."
<https://x.com/trq212/status/2118822238262853904|MCP pattern> · <https://x.com/trq212/status/2118859267314958761|Fish tweet>

*Guillermo Rauch* (Vercel CEO)
Demonstrated Generative UI for conversational agents — combining AI SDK with Chat SDK and json-render to route directly from LLM output to native UI on platforms like Slack and Teams. He's calling this the dominant "Human-Agent Interaction" paradigm going forward. Also mused: "Imagine we get gta6.wasm before gta6."
<https://x.com/rauchg/status/2118856239719608353|Generative UI for agents> · <https://x.com/rauchg/status/2118928276118986991|GTA6.wasm>

*Aaron Levie* (Box CEO)
Brief and pointed: "The future is files. And GPUs."
<https://x.com/levie/status/2118723097901846580|Tweet>

*Garry Tan* (Y Combinator President & CEO)
Two notable posts: (1) Advocating for eval-driven agent development — he just removed /investigate as a Claude Code skill because Opus 5.5 now handles it natively. "You can feel the AGI tide rising." (2) Highlighted research showing that just 3 million tokens of real moral-dilemma advice from ordinary people reduced AI malicious behavior to 0%, with a 28x efficiency jump across model generations.
<https://x.com/garrytan/status/2118920030243139596|Eval-driven skills> · <https://x.com/garrytan/status/2118950671886287323|Moral dilemmas research>

*Zara Zhang* (builder)
Argues the personal website is the new resume: LinkedIn shows titles, your site shows taste, thinking, and actual work — unconstrained by platform defaults.
<https://x.com/zarazhangrui/status/2118939184841052386|Tweet>

*Nikunj Kothari* (FPV Ventures Partner)
Re-released "Texts Wrapped" — a Mac tool that analyzes your iMessages, WhatsApp, and phone call history locally with zero AI and no cloud. One terminal command, fully open source. Also posted an epic (satirical) guide to building a $100M company in two weeks before Thanksgiving — every absurd detail is real: "this is satire, but every sentence has personally happened to me."
<https://x.com/nikunj/status/2118840414853861627|Texts Wrapped> · <https://x.com/nikunj/status/2118758688567792008|Fundraising satire>

*Aditya Agarwal* (SPC General Partner, ex-Dropbox CTO)
Shared a clip from an SPC conversation with Trae Stephens: "SpaceX didn't build Starship overnight. Ambitious technology demands both urgency & patience."
<https://x.com/adityaag/status/2118733089887170878|Tweet>

*PODCASTS*

*Latent Space — Controlling Biology: Fabian Theis, Helmholtz Munich*

_The Takeaway: AI isn't just predicting biology anymore — it's actively steering experiments in real time._

Fabian Theis leads the Computational Health Center at Helmholtz Munich, home to 500+ researchers and arguably the largest academic hub for health AI in Europe. His lab built Scanpy and the scVerse ecosystem — tools most computational biologists reach for daily.

The core of his work: building "perturbation world models" that predict how a cell responds to any input — a drug, a gene knockout, a change in environment. The challenge isn't just the modeling, it's the data. Each cell can be described as a 20,000-dimensional vector (what genes are active, and by how much), and while cell data has scaled massively, the perturbation space — what you can _do_ to cells — is still relatively sparse.

His newest release is Lab Compass, an inverse generative model that takes a forward world model and tells you what experiments to run to reach a target biological state — closing the loop from mapping → predicting → steering. Theis ran 3-4 iterative lab loops with Cambridge collaborators and showed this actually works. "We can really now start guiding the experimentation."

On the linear-vs-deep-learning debate that rocked the field: linear models often still win for simple perturbation settings, but flow-matching approaches (like those in his CellFlow paper, just accepted in Nature Methods) pull ahead on complex cross-tissue and cross-species tasks.

The ultimate vision: reinforcement learning in the lab loop — cells as an RL environment.

<https://www.youtube.com/@LatentSpacePod|Latent Space — Controlling Biology>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
