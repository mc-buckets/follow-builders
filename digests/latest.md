AI Builders Digest — May 22, 2026

*X / TWITTER*

*Sam Altman (OpenAI CEO)*

The headline: a general-purpose OpenAI model solved the unit distance problem, a long-standing open problem in mathematics. Altman called it "a kinda big milestone" and admitted to having "complicated feelings." He also laid out OpenAI's three current priorities — AGI accelerating research, AGI accelerating companies, and personal AGI helping individuals achieve their goals — and noted OpenAI is offering $2M in credits to every YC company.
• https://x.com/sama/status/2057203171198636251
• https://x.com/sama/status/2057218997503086888

*Aaron Levie (Box CEO)*

A detailed defense of Field Delivery Engineers (FDEs) — the technical consultants helping enterprises deploy AI agents. His core argument: agent adoption is fundamentally harder than cloud adoption because agents directly reshape employee workflows (not just developer tooling), and the pace of model improvement is so fast that best practices can't propagate before they're obsolete. "Every model change means either something new can be done that wasn't possible before, or some piece of scaffolding is now redundant or holding you back." He predicts this job category is here to stay and will be a strong path for early technical talent for years.
• https://x.com/levie/status/2057315272156135501

*Garry Tan (YC President & CEO)*

Unambiguous endorsement of Exa for web search in agents: "Exa is what I trust for all my agents. We use it at YC. We use it in all my OpenClaw and Hermes Agents. There is no other option that is as fast, as reliable, and as complete." Also shared a lighter take on idea fusion and lateral thinking ("LSD — lateral synaptic drift").
• https://x.com/garrytan/status/2057202833251000503
• https://x.com/garrytan/status/2057238298805129383

*Dan Shipper (Every CEO)*

On the $300M Anthropic acquisition of Stainless, Shipper contextualized why it matters: Stainless built the API/SDK infrastructure powering OpenAI, Anthropic, and most major tech companies — the invisible plumbing of the AI stack. He distilled five MCP design principles from his earlier interview with Stainless CEO Alex Rattray: keep toolsets small and precise; use "dynamic mode" for large APIs (just three tools: list endpoints, learn about one, execute it); apply JQ filters to strip unnecessary response data; build a company knowledge brain with Claude Code by saving customer quotes and SQL queries to a shared git repo; and treat code execution — not tool proliferation — as the future of MCP.
• https://x.com/danshipper/status/2057122805657821240

*Zara Zhang (Builder)*

Two sharp takes from Google I/O. On the T-shaped professional: AI forces everyone (not just developers) to deepen domain expertise, broaden adjacent skills, and layer AI proficiency on top — "I think this T-shape will apply to not just developers but every job function." On AI-native team structure: ICs should start thinking like managers (delegating to agents, setting standards, verifying output) while managers should become more hands-on builders rather than pure people managers.
• https://x.com/zarazhangrui/status/2057267931025957348
• https://x.com/zarazhangrui/status/2057324988009685208

*Swyx (AI engineer, Cognition / Temporal / Latent Space)*

Two data points worth noting. After an internal bake-off against competitors, his team unanimously chose Exa in just 1.5 hours. Separately, he mapped Sam Altman's idea of "build a business that gets better when models get better" onto what he calls "Agent Labs" — and reports a direct correlation between model performance and agent lab revenue, with a notable discontinuity in Q4 2025.
• https://x.com/swyx/status/2057180080078791036
• https://x.com/swyx/status/2057119153337545096

*Peter Steinberger (OpenClaw + OpenAI)*

Enthusiastic recommendation for Cotypist — an AI autocomplete tool that works system-wide. Brief post, but it resonated: 1,362 likes.
• https://x.com/steipete/status/2057040636449116222

*Nikunj Kothari (FPV Ventures partner)*

Candid post on the emotional weight of building a company: "Starting a company is so glorified — but building, scaling and maintaining one is a different story." He encouraged founders going through hard stretches and noted he's never had the courage to start a company himself for exactly this reason. Also shared a Claude-assisted summary of the SpaceX S-1 (308 pages condensed) for those short on time.
• https://x.com/nikunj/status/2057134939875991973
• https://x.com/nikunj/status/2057242868293816569

*Google Labs*

Project Genie — the AI game-creation tool shown at Google I/O — is now fully available to all Google AI Ultra subscribers globally (18+). The pitch: choose your characters, set the scene, and the AI generates a playable game in minutes.
• https://x.com/GoogleLabs/status/2057218835074437573
• https://x.com/GoogleLabs/status/2057179491693470166

*Guillermo Rauch (Vercel CEO)*

Teased something that will "bring AI to 42% of the web" — supporting every model, every provider, and every modality (text, image, video, audio). No further detail given.
• https://x.com/rauchg/status/2057212335811620987

*Kevin Weil (ex-CPO at OpenAI)*

Weighed in on the OpenAI math result, calling it "the next in a series of firsts for AI and mathematics."
• https://x.com/kevinweil/status/2057206749552066805

*Peter Yang (Product at Roblox, AI newsletter)*

Dry take on tech mental health: maybe not working at a company running repeated layoffs and performance cycles every few months is simply better for your wellbeing.
• https://x.com/petergyang/status/2057281238722072912

*Aditya Agarwal (GP, South Park Commons)*

Celebrated portfolio builder Feross completing his -1 journey at South Park Commons — proud of the progress and excited about what's ahead.
• https://x.com/adityaag/status/2057141903334990327


*PODCASTS*

*AI & I by Every — Inside Stainless: The Developer Tools Startup Anthropic Just Bought for $300 Million*

_The Takeaway:_ The best MCP servers aren't built by exposing every API endpoint — they're designed with ruthless restraint, and the real future of AI-web connectivity is code execution, not tool proliferation.

Alex Rattray is the CEO of Stainless, the developer tools startup Anthropic just acquired for a reported $300M. Stainless builds the APIs and SDKs powering OpenAI, Anthropic, Stripe, and most other major tech companies — the plumbing that lets computers talk to computers. Now they're building MCP servers, the interfaces that let AI models interact natively with those same APIs.

Rattray's MCP philosophy cuts against the "expose everything" instinct. Most MCP implementations fail, he argues, because teams try to load their entire API into the model's context — burning tokens and overwhelming the LLM. His design rules are almost zen: keep the toolset small, give each tool a precise name and description, minimize input parameters, and return only the data the model actually needs. For large APIs, Stainless uses "dynamic mode" — instead of hundreds of tools, the model gets just three: list available endpoints, learn about one, then execute it. It solves the context problem but adds latency.

His bigger bet is that MCP's current tool-calling paradigm will give way to code execution. Give the model a TypeScript sandbox and a doc-search tool. It writes SDK code against a typed library, runs it on a server, and iterates when it gets something wrong — with the type checker catching hallucinations before they propagate. The context footprint stays tiny, execution is fast, and the whole approach scales in a way that hundreds of discrete tools never could.

"We haven't figured out how to expose an API ergonomically to an LLM in the same way that we've figured out how to expose it ergonomically to a Python developer. And that's kind of like a new research problem."

He also practices what he preaches internally: Rattray uses Claude Code to maintain a shared "company brain" at Stainless — a Git repo where the AI saves useful artifacts (customer quotes, board-prep SQL queries) that the team can query later without re-fetching from MCP servers every time.

https://www.youtube.com/playlist?list=PLuMcoKK9mKgHtW_o9h5sGO2vXrffKHwJL

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
