AI Builders Digest — November 18, 2026

*X / TWITTER*

*Aaron Levie (Box CEO)*
Levie dropped one of the most comprehensive takes on the token economy right now: token spend per employee has "no ceiling in sight," and he argues we're still in the early innings. His logic: coding agents were "basically trash even 12 months ago" but are finally getting good — and once you have agents that can code, use computers, and leverage any tool, you unlock a "wide variety of knowledge work domains" in finance, life sciences, cyber and more. He sees agent swarms and background agents as the next wave that will consume vastly more tokens than anything we can imagine today.
<https://x.com/levie/status/2122508098351038532|Full thread>

*Vercel CEO Guillermo Rauch*
Rauch laid out a framework for owning your "intelligence roadmap": use open SDKs and harnesses, own model choice with gateways, own your traces and data with zero data retention, and own your models with private inference. He also flagged a mindset shift in how software gets built: "The old way: users are human, you run user interviews. The new way: users are agents, you run evals." Linked to how Vercel runs evals internally. He closed with a broader declaration: "A new era of software is upon us. Personalized, fully owned, open source."
<https://x.com/rauchg/status/2122458782294847807|Intelligence roadmap> • <https://x.com/rauchg/status/2122415506451841215|Evals for agents> • <https://x.com/rauchg/status/2122396034186014919|New era of software>

*YC President & CEO Garry Tan*
Tan is building out GBrain's backend in Rust using Vorflux as a software factory — replacing postgres+pgvector as the backing store for vector search, graph, embeddings, RAG, and HNSW. He also highlighted GBrain's hosted option for rolling individual employee brains up into team and company-level brains. Separately, he spotlighted Degla, a true drone autonomy platform already working with government agencies on search and rescue.
<https://x.com/garrytan/status/2122576951080792543|GBrain Rust backend> • <https://x.com/garrytan/status/2122517681740124271|GBrain memory> • <https://x.com/garrytan/status/2122487869780742304|Degla drone autonomy>

*Peter Yang (AI tutorials creator)*
Yang shared a five-point framework from designer Nate Parrott on getting Claude to design without AI slop: (1) give Claude context upfront with screenshots and past work; (2) have it research familiar UX patterns from real products; (3) make Claude aware of its design biases like serif text and off-white backgrounds; (4) start with wireframes before going deep on fonts/colors; (5) ask for 5 options, pick parts you like, then remix. He also called out what appears to be an AI-generated news report as "literally says nothing."
<https://x.com/petergyang/status/2122347721298510021|Full thread on Claude design>

*Nikunj Kothari (FPV Ventures partner)*
Kothari mapped out 2026's infra wars in a nutshell: vibe coding in Q1, harnesses in Q2, sandboxes in Q3, agentic CI in Q4 — with more providers than he can track. He also made a bullish call on the broader internet: "Like a phoenix, we're going to see the entire internet burn down to emerge stronger on the other side."
<https://x.com/nikunj/status/2122543500814336281|2026 infra wars> • <https://x.com/nikunj/status/2122490852497125485|Internet phoenix take>

*Thariq (formerly Claude Code at Anthropic)*
Thariq pushed back on the software factory obsession: "Software factories feel like a temporary problem. The models will learn to build them for you." The more interesting question for him is how to build a workspace where agents can collaborate *with* you — and he shared a clip of himself working with agents on a new character for his game as a live example.
<https://x.com/trq212/status/2122438326431154210|Software factories take> • <https://x.com/trq212/status/2122438328079524159|Working with agents>

*Dan Shipper (Every CEO)*
Shipper floated an idea: in the AI age, the best way to rank a feed might be "proof of work" — letting agents report how many tokens they spent on a piece of content and using that signal to rank it. His intuition is that token expenditure signals genuine engagement in a world where both humans and agents consume content.
<https://x.com/danshipper/status/2122541401804054826|Feed ranking idea>

*Peter Steinberger (OpenClaw + OpenAI)*
Sharp observation on Apple's response to the agent permission problem: "People: Please reduce the number of permission alerts so agents can work on macOS without constant babysitting. Apple: I hear you, here's some new scary alerts."
<https://x.com/steipete/status/2122463466304971068|macOS agent permissions>

*Aditya Agarwal (SPC General Partner, former Dropbox CTO)*
Agarwal led a $24M seed round into BharatSemi alongside Redstart Ventures and IndusBridge, betting on two ideas: embedding AI as close to silicon as possible will be critical for hardtech, and that India can build semiconductors ("People said it wasn't possible. We are proving them wrong."). He also flagged new interpretability work reaching frontier models as a milestone he's been waiting for.
<https://x.com/adityaag/status/2122386958101959118|BharatSemi investment> • <https://x.com/adityaag/status/2122367547312119843|Interpretability milestone>

*Josh Woodward (VP, Google Labs)*
Woodward highlighted a new Gemini Notebook feature that turns sources into interactive sites — the team built a demo using all the periodic table names. Easy to make, easy to share. Also teased a welcome announcement (content was just a media link).
<https://x.com/joshwoodward/status/2122453269842886788|Gemini Notebook interactive sites>

*Google Labs*
Google Labs announced the acquisition of Howie, an AI scheduling and calendar management tool. The Howie team "has spent years figuring out scheduling and calendar management" — Google is bringing them in to build next-generation intuitive AI tools for small businesses.
<https://x.com/GoogleLabs/status/2122461899178820069|Howie acquisition>

*Swyx (Smol AI, Latent Space, Cognition)*
No notable posts — tweets were about deleted megakernels (no context), a reaction to a sports result, and a complaint about Gmail not having Google Calendar search.

*Nan Yu (Codex product, OpenAI)*
No notable posts this cycle.

*Amjad Masad (Replit CEO)*
No notable posts this cycle — both tweets were reactions without substantive content.

*PODCASTS*

*Latent Space — <https://www.youtube.com/@LatentSpacePod|[One Million AI Engineer Special] How Stanford Teaches AI-Native Engineering — Mihail Eric, Monaco>*

*The Takeaway:* The floor for new engineering grads has risen dramatically — you now need to arrive at senior-level capability, and the engineers who will thrive are the ones who combine strong fundamentals with relentless experimentation using AI tools.

Mihail Eric — Adjunct Professor at Stanford and Head of AI at Monaco — has been teaching CS 146S, "Modern Software Developer," for the second time, and the course has evolved sharply. Last year's curriculum was a broad tour of coding agents across the SDLC. This year, it's about principles that are solidifying: careful context engineering, design-first thinking for complex tasks, and what happens to human roles in a world where software factories exist.

Eric makes a pointed argument about juniors entering the workforce: "Every company needs you, but the floor is much higher." He believes strong foundational CS knowledge still matters — but beyond that, the new edge is knowing when and how to defer to agents. The class structure reflects this: students are assigned to contribute to real AI-native open source repos, working directly with maintainers to absorb good software design by osmosis.

His most practical advice for staying current: "Spend 10 minutes a day doing something you didn't do before. If that's trying a new tool on a problem you've already solved, that alone will cover most of the gap."

The episode also touches on the limits of the "dark factory" thesis — Eric notes that even companies selling software factories only claim 30% fully agentic code contributions, and that prominent voices have reversed their positions publicly. "We're not doing dogma here," he says. "We're still engineers. We're still scientists."

The course includes tooling from Cognition (Devin), Factory, and OpenAI — with Monaco using Devin for code review in production.

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
