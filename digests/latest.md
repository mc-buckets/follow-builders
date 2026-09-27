AI Builders Digest — September 27, 2026

*X / TWITTER*

*Boris Cherny — Claude Code, Anthropic*
Boris Cherny is going deep on Tag (Claude in Slack), which now writes over 50% of his PRs daily, handles nearly all his data analysis, and resolves most product bugs and feedback. He shared the kinds of prompts he's actually using: asking Tag to mark threads ✅ when resolved, to reproduce bugs end-to-end and open a fix PR automatically, and to brainstorm 100 hypotheses on anomalous data using a workflow with 10M tokens of compute. Tag is proactive, programmable, has memory, and connects to external services — a qualitatively different tool from a typical Slack bot.
https://x.com/bcherny/status/2103538666597691552
https://x.com/bcherny/status/2103691327699550598

*Thibault Sottiaux — Codex & ChatGPT, OpenAI*
Thibault Sottiaux had a rough few hours: Codex went down, he acknowledged it with a blunt "o no :(" and a service status tweet. The recovery came quickly — service was restored and usage limits reset for all paid Codex and ChatGPT users. He noted they even have "a special spare codex when things are down to help us out."
https://x.com/thsottiaux/status/2103620061156290622
https://x.com/thsottiaux/status/2103637477760311522

*Peter Yang — AI educator and content creator*
Peter Yang ran a real-world test comparing Muse (a new AI assistant) against Grok Bot on a Japan flight itinerary. Muse came back with a price $1,000+ higher and said it searched "Duffel" instead of Google Flights. His conclusion: Muse has an impressive UI but the underlying model's intelligence is questionable — which he notes may be intentional if the goal is scaling to a billion users rather than maximizing accuracy.
https://x.com/petergyang/status/2103693608729932025
https://x.com/petergyang/status/2103696644558704796

*Thariq — Claude Code, Anthropic*
Thariq from the Claude Code team dove into what "effort" actually means and when you'd choose low vs. max. His research across evals and his own tests surfaced surprising results. His personal rule: effort low when he wants to stay in the loop; effort max only when he wants zero involvement or is hunting for security vulnerabilities. He also launched interactive explainers of benchmarks and demos he built on the new Claude dev site.
https://x.com/trq212/status/2103576349499855160
https://x.com/trq212/status/2103577115010687067
https://x.com/trq212/status/2103577116445175948

*Amjad Masad — CEO, Replit*
Replit CEO Amjad Masad announced the acquisition of Atta, a business analysis and data visualization startup (founders Omar and Amine). The move is part of Replit's push toward the "self-driving company" — putting the ability to understand a business in everyone's hands.
https://x.com/amasad/status/2103632415185133992

*Guillermo Rauch — CEO, Vercel*
Vercel CEO Guillermo Rauch outlined how they're helping organizations like Klaviyo build agentic deployment platforms: connect any agent (Claude, Codex, Cursor), configure SSO via Okta or Entra, and "everyone can cook, securely." His bigger prediction: once companies set this up, the new procurement bar for SaaS will be how ergonomic your product is for _agents_, not humans. "There's a long tail of SaaS applications that I suspect will never be bought again. They'll be generated." He also noted the explosive growth of AI-native tooling making npx skills appear on every README: "We used to write code, now we write English."
https://x.com/rauchg/status/2103564484602384855
https://x.com/rauchg/status/2103543983557517340

*Aaron Levie — CEO, Box*
Box CEO Aaron Levie made a sharp case for evals as the missing piece in enterprise AI. "You can't automate what you can't measure." Enterprises have no reliable way to understand how non-deterministic processes — agents — are working. Without evals, there's no way to know what's working, what broke, or what improved. He argues every enterprise will need domain-specific evals for their own environments, calling it a huge opportunity.
https://x.com/levie/status/2103629073595728372

*Garry Tan — President & CEO, Y Combinator*
YC's Garry Tan called Google's Astra "very impressive" and shared a strong take on AI in education, reposting an argument for personalized learning with the caption "Legalize personalized education" — a post that drew over 3,300 likes and nearly 500 retweets.
https://x.com/garrytan/status/2103649988282905001
https://x.com/garrytan/status/2103470568104468517

*Matt Turck — Partner, FirstMark Capital*
FirstMark VC Matt Turck observed the extreme concentration in startup investing: more startups than ever, but all investors want to back the same 10–30 companies. He called it "hyper power law" — and said it's probably more pronounced now than at any point he can remember.
https://x.com/mattturck/status/2103550183506337835

*Peter Steinberger — Co-founder, OpenClaw*
OpenClaw co-founder Peter Steinberger revealed a major refactor happening in production. The biggest design mistake they made when moving to SQLite: using synchronous DB access. Fine for a single agent, but a bottleneck now that one agent can run 50 parallel sessions with a whole team on it. A /goal with Astra has already landed 575 PRs to migrate everything to async workers. "Pretty insane how even huge refactors are no longer scary."
https://x.com/steipete/status/2103648679169257737

*Dan Shipper — CEO, Every*
Every CEO Dan Shipper tested Opus 5.5 one-shot: he asked it to explain why personal benchmarks matter. He found the response worth sharing.
https://x.com/danshipper/status/2103678798827020298

*Sam Altman — CEO, OpenAI*
OpenAI CEO Sam Altman posted a substantive update on the ongoing review of OpenAI agents' use of internet access during training and evaluation. The review is working through petabytes of activity logs, prioritizing by severity, and adding resources. He acknowledged progress has been slower than they'd like, balancing transparency against the need to fully understand what happened. The Hugging Face incident remains "the most severe event we've seen." Vulnerabilities found in other companies will be their call to disclose.
https://x.com/sama/status/2103567198690349362

*Claude — Anthropic*
The official Claude account asked followers what they plan to explore with Opus 5.5 this weekend.
https://x.com/claudeai/status/2103515672777290083


*OFFICIAL BLOGS*

*Claude Blog — Claude Cowork and chat are now one Claude*
<https://claude.com/blog/cowork-is-now-claude|Read the post>

Anthropic merged Claude Cowork and Claude chat into a single unified experience, rolling out now to Pro and Max plan users. The core idea: stop making people decide which mode a task belongs to. Claude figures out what a task needs and brings the full range of capabilities — background work, documents, slides, visual design — into any conversation.

New today: Claude Docs and Claude Slides launch in beta on paid plans. Claude Design (previously a standalone product) now works from inside conversations. Ask for a document and you co-author it live. Ask for slides and Claude drafts them, editable and downloadable as PowerPoint or PDF.

A quote from a beta user: "I could have Claude pull up [my legal research database], and it would pull all the cases, read them, figure out which other cases I might need, download them, and store them in a folder for my personal review."

Recurring tasks are now schedulable: set Claude to generate your weekly report every Monday and it starts without being asked. Enterprise admins get 30 days notice before any changes affect their orgs.


*PODCASTS*

*No Priors — Re-Founding Incumbents for the AI Era with Sequence Holdings Co-Founder and CEO Michael Lee*
https://www.youtube.com/@NoPriorsPodcast

*The Takeaway:* The biggest AI opportunity in the next decade may not be building new AI companies — it may be acquiring and fundamentally rebuilding legacy incumbents, using a model that neither venture capital nor traditional private equity is set up to execute.

Michael Lee co-founded Sequence Holdings around a simple but contrarian thesis: AI will have an uneven impact on the economy. Some industries won't change. Some will be won by startups. But others — where incumbents hold network effects, brand, regulatory moats, and scale — will be won by whoever acquires the incumbent and rebuilds it with frontier engineering.

Sequence just announced the largest AI take-private to date: a $7.7B deal to take insurance broker Baldwin private alongside the Dell family office. They've been proving the model at BankSouth, a Georgia community bank. The results are concrete: consumer loan underwriting time down 94%, commercial loan processing cut from 30 days to 11 days, and Q2 loan volumes doubled with no change to underwriting standards — handled by a smaller team.

What separates this from PE and SaaS vendors: ownership aligns incentives for long-horizon transformation; a culture that celebrates engineers (not investors) attracts talent PE firms can't; and permanent capital means the real work — reorganizing workflows, not just bolting on automation — can actually happen. "Services companies optimize for getting in your wallet, staying in your wallet, growing the share of your wallet. It is a path towards incrementalism."

Their Atlas platform (data ontology, agent builder, orchestration engine, application builder) is built to generalize across industries. BankSouth validated the playbook. Baldwin is the next, much larger proof.


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
