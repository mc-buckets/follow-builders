*AI Builders Digest — April 24, 2026*


*X / TWITTER*


*Swyx* (AI researcher — Cognition, Temporal, AI Dot Engineer, Latent Space podcast)

Sharp reframe on GPT-Image-2-Thinking: don't think of it as a better image model — it's a new image _agent_. It wraps search and Photoshop-like tooling inside an agent loop that can composite, self-review, and iterate, which is why generation can take tens of minutes and why it can one-shot QR codes, logos, and faces. "The same way Gemini Flash Vision destroyed benchmarks by introducing an agentic loop for image-to-text, now Image-2-Thinking is doing it for text-to-image."
<https://x.com/swyx/status/2047140362771132544|Tweet>


*Josh Woodward* (VP at Google Labs / Gemini App / Google AI Studio)

Shipped a papercut fix: conversation branching is now rolling out to 20% of Gemini users with a wider ramp on the way.
<https://x.com/joshwoodward/status/2047147030351642914|Tweet>


*Peter Yang* (Product at Roblox, AI tutorials newsletter with 140K+ readers)

"Craft > slop — I love using AI to generate things too but craft is in that last 10% where you manually apply your taste to make something you can be proud of. Many people never bother." Separately, surfaced an interview where Ryan from Mercury talks about using Claude Code as a second brain.
<https://x.com/petergyang/status/2047124883071816189|Tweet> | <https://x.com/petergyang/status/2046982893185188088|Interview tweet>


*Amjad Masad* (CEO of Replit)

Three announcements back-to-back: (1) Replit published a whitepaper showing that pairing current-gen LLMs with static analysis tools yields 90%+ performance improvements in some cases — a practical path while the next-gen Mythos model stays gated. (2) The Replit Security Agent is now reviewing apps deployed on the platform. (3) Replit Agent is now callable directly from Gemini Enterprise.
<https://x.com/amasad/status/2047156858214035590|Whitepaper tweet> | <https://x.com/amasad/status/2047150876423516384|Security Agent tweet> | <https://x.com/amasad/status/2047149103294091301|Gemini Enterprise tweet>


*Guillermo Rauch* (CEO of Vercel)

Detailed security update on an ongoing threat actor campaign that extends well beyond the initial Context.ai compromise. Vercel analyzed nearly a petabyte of logs and found a repeated pattern: malware harvesting API tokens, then rapid enumeration of environment variables once access is gained. Vercel has deepened partnerships with Microsoft, AWS, and Wiz, and has notified suspected victims outside the original event. Full details in the security bulletin linked in the tweet.
<https://x.com/rauchg/status/2047150411170320808|Tweet>


*Aaron Levie* (CEO of Box)

Called the new ChatGPT agents "probably the biggest news yet in software going headless" and shared a demo: a custom enterprise sales assistant using Box as a knowledge source via MCP and CLI, pulling content securely to answer questions and generate new material on the fly. "This is precisely what agents will start to look like for knowledge work. You'll be able to spin them up in the foreground or background to help augment work." Big moment for headless platforms and enterprise agent builders.
<https://x.com/levie/status/2047028112626749645|Tweet>


*Ryo Lu* (Designer at Cursor)

Wrote a widely-shared essay coining "overcooking" — the pattern where AI drops the cost of adding features to near-zero, letting teams pile on individually reasonable decisions that together become incoherent. The culprit isn't any single bad choice; it's the accumulation of additions that no one said no to. "What we need aren't more tools that make more slop. It's seeing through the chaos, and returning to what the thing actually is, and cutting everything that doesn't serve that. That's harder now, not easier. Because there's always something else you could add with one more prompt."
<https://x.com/ryolu_/status/2046957675079237668|Tweet>


*Garry Tan* (President and CEO of YCombinator)

Sharing early findings on agent skill composition: "fewer, fatter skills" — merging adjacent capabilities into larger skills with more parameters — produces shorter resolvers, less context bloat, and better performance overall. Composing bigger skills with branching params beats splitting into many small ones. "Short resolvers are better than long ones."
<https://x.com/garrytan/status/2047183884266402275|Tweet> | <https://x.com/garrytan/status/2047184243164651648|Tweet>


*Zara Zhang* (independent builder)

Impressed by a demo of a coding agent capable of working autonomously on long-running tasks without any human intervention in the loop.
<https://x.com/zarazhangrui/status/2047166162707042431|Tweet>


*Nikunj Kothari* (Railway / Meter)

Bullish on real-time pixel generation: "Every pixel will be generated in real time. It's just a matter of when, not if." Shared a demo as a preview of what's coming.
<https://x.com/nikunj/status/2047024714116419665|Tweet>


*Dan Shipper* (CEO of Every)

Announced a new AI & I episode with Kieran Klaassen on compound engineering and the "AI sandwich" metaphor. Core idea: humans are indispensable at the beginning (framing the problem) and end (final polish) of any AI workflow — the models handle the filling in the middle, which is "largely solved." The episode covers the four steps of compound engineering, why agents can't change frames, and how to find your role in an AI-accelerated world.
<https://x.com/danshipper/status/2047027507397005367|Tweet>


*Sam Altman* (CEO of OpenAI)

Brief endorsement of the new ChatGPT agent capabilities (responding to the same announcement Aaron Levie highlighted): "These are cool! I think most companies will want to use them."
<https://x.com/sama/status/2047017964105597009|Tweet>


*Claude* (Anthropic)

Interactive charts and diagrams are now live in Claude Cowork, available in beta on all paid plans.
<https://x.com/claudeai/status/2047047633416397076|Tweet>


*OFFICIAL BLOGS*


*Claude Blog: <https://claude.com/blog/claude-code-desktop-redesign|Redesigning Claude Code on desktop for parallel agents>* (Published Apr 14, 2026)

Anthropic shipped a major redesign of the Claude Code desktop app built around parallel agentic work. The new sidebar manages multiple simultaneous sessions across repos, filterable by status, project, or environment — and archives itself when a PR merges so the view stays focused. Key additions: drag-and-drop pane layout, integrated terminal and in-app file editor, faster diff viewer rebuilt for large changesets, expanded in-app preview for HTML files and PDFs, and full CLI plugin parity. SSH support now extends to Mac. Three view modes — Verbose, Normal, Summary — let you dial between full transparency into Claude's tool calls and results-only. Available now for Pro, Max, Team, and Enterprise plans, and via the API.


*PODCASTS*


*AI & I by Every — "The AI Sandwich: Where Humans Excel in an AI World"*
<https://www.youtube.com/watch?v=G0LTv8hQ5Cs>

Kieran Klaassen — GM of Quora and creator of the Compound Engineering framework used at Every — makes a precise and counterintuitive argument: the "work" phase of agentic coding is essentially solved. LLMs reliably execute well-specified plans. What remains irreducibly human is the framing at the start and the taste-driven polish at the end. That's the sandwich — humans as bread, AI as filling.

Compound Engineering is a four-step loop: brainstorm → plan → work → review → compound. The "compound" step — feeding learnings back into the repo so agents don't repeat the same mistakes — is what lets one engineer ship like a team of five. But Klaassen's key insight is that the loop's middle is increasingly hands-off; the bottleneck has shifted to the edges.

His music background sharpens the point: practicing a piece 100 times isn't creative — that's the middle. "At the end, the performance is where you bring it out into the world to the people." The polish step at the end is the performance; ideating from nothing is composing. Both are still human.

On whether agents will eventually take those edge steps too: "If you ship something or do something... if you want it to be your own, you cannot fully automate everything. It's maybe a little bit like art." His prescription: lean into whatever brings you joy — beautiful code, polished UI, sharp copy — because that's where human-AI collaboration compounds.


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
