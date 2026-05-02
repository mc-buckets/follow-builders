AI Builders Digest — May 2, 2026


*X / TWITTER*


*Swyx — AI engineer, Cognition and Latent Space podcast*

Swyx shared an epic thread about a months-long project to build a "vintage" language model trained exclusively on pre-1931 public domain text — old books, newspapers, patents, scientific journals, case law. The goal: a model free of modern AI slop that could channel how people a century ago thought and wrote. The team assembled ML veterans (including the original GPT-1/2 researcher), trained a custom OCR model for old documents, synthesized RLHF pairs from etiquette manuals and cookbooks, and built an anachronism classifier to keep future knowledge out. The result checked out against benchmarks — and turned out to be, in Swyx's words, "the most confidently racist model ever released by humankind." A sharp cautionary tale about what pre-modern text actually contains.

- <https://x.com/swyx/status/2049652947408372187|The vintage model project (and what went wrong)>

He also nudged builders to experiment more with base model completions — not enough people are doing weird finetunes and novel usages of the base models that actually exist today.

- <https://x.com/swyx/status/2049643473339601388|In praise of base model experimentation>


*Josh Woodward — VP at Google Labs, Gemini App, and Google AI Studio*

Gemini can now generate and export files directly — tell it what you want and the format, and it does the work. Now supporting Google Docs, Word (.docx), PDFs, Google Sheets, Excel (.xlsx), CSV, Google Slides, Markdown, LaTeX, TXT, and RTF. Available globally on all surfaces now.

- <https://x.com/joshwoodward/status/2049524400131838436|Gemini file generation launches globally>


*Kevin Weil — VP of Science at OpenAI*

A clean reframe on AI and radiology: the radiologist's job isn't to read x-rays — it's to cure people. If AI speeds up the interpretation step, radiologists can see and help more patients. A concise argument for why AI assistance expands professional capacity.

- <https://x.com/kevinweil/status/2049584046213378229|On radiologists and AI>


*Nan Yu — Head of Product at Linear*

Teased that Linear is "reinventing design to eng handoff from first principles." No details yet, but notable given how much friction lives in that handoff.

- <https://x.com/thenanyu/status/2049593061043265940|Reinventing design-to-eng handoff>


*Amjad Masad — CEO of Replit*

Masad reflected on Ron Conway's approach to Silicon Valley — turning generosity, warmth, and showing up for founders into a genuine winning strategy, not just a reputation play.

- <https://x.com/amasad/status/2049729530059960571|On Ron Conway's way>

Also announced free accounts for teachers and 50% off for students on Replit.

- <https://x.com/amasad/status/2049595212889247994|Free for teachers, half-off for students>


*Aaron Levie — CEO of Box*

Levie wrote one of the more concrete takes on what the agent economy actually means inside enterprise: Box is hiring and retraining for a new internal role he's calling "agent engineering." The job is highly technical — building secure, governed agents that wire up internal systems (Box, Salesforce, Workday, etc.) and codify workflows as skills. Think of it as an internal field delivery engineer, except instead of deploying software, they're deploying agents into business processes. He expects a companion role to emerge on the business side — essentially agent product management for internal operations. Key framing: "It's not about bringing automation to a job, but bringing automation to a process."

- <https://x.com/levie/status/2049714403050918067|The new agent engineering role>


*Ryo Lu — Designer at Cursor*

Announced that Cursor now lets you build your own agent systems using the same multi-model harness Cursor uses internally — available both locally and in the cloud.

- <https://x.com/ryolu_/status/2049529609725804575|Build your own agent systems with Cursor>


*Garry Tan — President and CEO of Y Combinator*

Tan shared two updates on GBrain, his AI-augmented knowledge system: he completed a full end-to-end test harness for the GBrain install flow on OpenClaw, so the onboarding process is now fully verifiable. He also showed that knowledge graphs in the new version are automatically built from frontmatter attributes — more inference, less manual work.

- <https://x.com/garrytan/status/2049742376307147110|GBrain E2E install harness done>
- <https://x.com/garrytan/status/2049737217208397925|Graph built from frontmatter attributes>


*Zara Zhang — Builder*

Sharp one-liner worth sitting with: "We should start thinking about the IT/internal tools team as more like 'HR for agents.'" As agentic systems proliferate inside organizations, someone has to manage their onboarding, permissions, performance, and offboarding — and that looks a lot more like HR than traditional IT.

- <https://x.com/zarazhangrui/status/2049599305825341518|IT team as HR for agents>


*Peter Steinberger — Co-creator of OpenClaw*

Built codex review into clawsweeper — his automated code review tool now uses a system prompt similar to `/review`, with automerge that loops until it stops finding new issues.

- <https://x.com/steipete/status/2049518771023360010|Codex review integrated into clawsweeper>


*Aditya Agarwal — General Partner at South Park Commons, former CTO of Dropbox*

Agarwal shared a grounded, contrarian thread on agents after spending serious time with OpenClaw, Hermes, and similar tools. His main observations: most people who rave about these tools haven't actually used them. Agents are developer products today — nowhere near consumer-grade in reliability or simplicity. He wishes agents generated more dynamic, interactive UIs instead of defaulting to chat. His most useful framing: once you understand the core loop of agentic AI (iterative tool calling + code generation), one-off chat prompts start to feel like search queries — "always-on" agents that adapt and maintain state are a fundamentally more compelling paradigm. The UX friction today is real — he compared installing OpenClaw to "running Linux in the early 2000s. You spend a lot of time compiling device drivers, setting up configurations... you feel a real sense of accomplishment from jerry-rigging everything together, but it is a lot of work."

- <https://x.com/adityaag/status/2049530878083379427|Honest observations on agents>


*Sam Altman — CEO of OpenAI*

Announced the rollout of GPT-5.5-Cyber, a frontier cybersecurity model, to "critical cyber defenders" in the coming days. OpenAI says it will work with the broader ecosystem and government to define trusted access, with the goal of rapidly securing companies and infrastructure.

- <https://x.com/sama/status/2049712078836170843|GPT-5.5-Cyber rolls out to cyber defenders>


*Claude — Anthropic's AI assistant*

Highlighted hackathon winners from a recent event. ARIA (Best Use of Claude Managed Agents) — a maintenance system that reads machine manuals and, when something breaks, generates a work order with the fix that worked last time. Built by Idriss Benguezzou and Adam Hnaien from France.

- <https://x.com/claudeai/status/2049523910173966597|ARIA: managed agents for maintenance>

MaestrIA ("Keep Thinking" Prize) — a home repair tool that photographs damage, diagnoses the problem, prices parts at local stores, and drafts a message to a nearby tradesperson. Built by a carpenter's son from Chile.

- <https://x.com/claudeai/status/2049523908584386582|MaestrIA: home repair diagnosis tool>


*PODCASTS*


*AI & I by Every — "How Stripe Is Building for an Agent-native World"*

_The Takeaway:_ Compute is the new credit card number — and Stripe's view of 2% of global GDP reveals that the agent economy is already reshaping fraud, pricing, and growth in ways most people haven't internalized.

Emily Glassberg Sands, Head of Data and AI at Stripe, brings a uniquely grounded perspective: Stripe processes transactions for a swath of the global Internet economy, and as agents have proliferated, the patterns are genuinely new.

The fraud picture is alarming. Free-trial abuse has quadrupled in six months. For one large AI company, Stripe is now blocking 250,000 fraudulent free trials per week. The root problem: in AI, every prompt and every API call has a real cost attached, making free compute the new customer acquisition cost — and a prime target. About 7% of sign-ups at AI companies on Stripe are multi-account abusers burning free credits and disappearing. "Compute theft is the new payment fraud." Stripe's Radar has responded by moving up-funnel: fraud detection now starts at sign-up, not checkout, and now works across all payment methods and processors, not just Stripe transactions.

The growth data is striking. Top AI companies on Stripe reach $30M ARR in about 18 months — three times faster than the top 100 SaaS companies from 2018. It's scaling faster at every milestone: $1M, $5M, $30M ARR. So far it looks like net new spend rather than cannibalized software budgets.

The pricing model shift is equally fast. Seat-based SaaS made sense when marginal costs were near zero and users were human. AI companies are now iterating through usage-based billing (tokens, API calls, workflows, outcomes), hybrid subscriptions with overages, and prepaid credits. Stripe's "token billing" product — which prices dynamically to the real-time cost of underlying model tokens — is being used by Lovable, Mesa, and Ship to protect margins as model costs fluctuate.

The most provocative frame: "Over time, agents will become the predominant actors on the Internet." Stripe is building its entire infrastructure — fraud, identity, billing — around that assumption now.

<https://www.youtube.com/playlist?list=PLuMcoKK9mKgHtW_o9h5sGO2vXrffKHwJL|AI & I: How Stripe Is Building for an Agent-native World>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
