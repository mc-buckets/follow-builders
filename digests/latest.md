*AI Builders Digest — September 23, 2026*


*X / TWITTER*


*Swyx* (latentspacepod co-host, smol_ai, Cognition affiliate)

New @latentspacepod episode with Allen Park is out now. Available on email, Apple Podcasts, and YouTube.
<https://x.com/swyx/status/2102160025666101658|View tweet>


*Thibault Sottiaux* — Codex & ChatGPT product at OpenAI

Dropping a cryptic but high-engagement tease: "Ladies and gentlemen... start... your... ENGINES. We are almost Tuesday and I promised a reset for Tuesday." This racked up 12,500+ likes and 760 retweets, suggesting a significant Codex or ChatGPT launch is imminent.
<https://x.com/thsottiaux/status/2102254445082116335|View tweet>


*Peter Yang* — AI tutorials and interviews creator

Yang is sounding alarms on the ad market: if agents browse the web and complete tasks without a human ever seeing a display ad, targeted advertising loses its audience entirely. He's also been leaning into agentic finance — sharing a story about ChatGPT Finances catching an erroneous hotel charge and getting a reimbursement, and noting he used an agent to cancel a hotel booking for his parents and monitor replies until the refund came through. His summary of where his attention lives now: "I no longer live in email or text, I live in the chat with my agent(s)."
<https://x.com/petergyang/status/2102215701255844074|View tweet>
<https://x.com/petergyang/status/2102186174911746151|View tweet>
<https://x.com/petergyang/status/2102181024507765167|View tweet>


*Thariq* — Claude Code at Anthropic

One pithy, high-resonance prompt tip: "I now type 'use big pictures and few words' several times a day." 1,759 likes suggests this lands widely as a prompt-engineering instinct for multimodal AI work.
<https://x.com/trq212/status/2102186805034635576|View tweet>


*Amjad Masad* — CEO of Replit

Brief but bold: "AI is reviving the American Dream." Shared as a quote tweet, pointing to the democratizing potential of AI-powered building.
<https://x.com/amasad/status/2102120769232978174|View tweet>


*Guillermo Rauch* — CEO of Vercel

Two things caught his attention: First, he put Grok 4.7 through a hard reverse-engineering problem involving a running binary and was impressed — "Beautifully solved. And it's so fast!" Second, Vercel's AI SDK now supports Jev over HTTP in AI Gateway alongside its type-safe TypeScript API.
<https://x.com/rauchg/status/2102089968860721335|View tweet>
<https://x.com/rauchg/status/2102205684544852121|View tweet>


*Aaron Levie* — CEO of Box

Levie is thinking hard about the infrastructure layer for the agent economy — and posted two dense threads worth reading together. Thread one: AI agents will use software 100x more than humans ever did, which makes data platforms (CRM, ERP, unstructured data) more important, not less. The platforms that can act as security layers, manage data for agents, and orchestrate business logic have a huge opportunity — for startups and incumbents alike. Thread two: personal agents that transact on your behalf represent a massive monetization surface. As people get comfortable delegating simple tasks, they'll hand over more complex (and higher-spend) ones. This creates opportunity for agent providers and for whoever builds the commerce/services layer that agents interact with.
<https://x.com/levie/status/2102235949430354273|View tweet>
<https://x.com/levie/status/2102253246807261579|View tweet>


*Garry Tan* — President & CEO of Y Combinator

Tan has a new agentic coding secret weapon: Capy.ai. He says it handles multi-step workflows and large PRs faster than Codex or Claude Code on its own, with clear task delineation, automatic parallelization, and clean GitHub PR/CI integration — and shared an example PR on his GBrain project as proof. Separately, he's still bullish on Cluely's concept as a "realtime thought helper and semi-adversarial assistant with ongoing context," even as the company has pivoted.
<https://x.com/garrytan/status/2102095924893827501|View tweet>
<https://x.com/garrytan/status/2102096495847551011|View tweet>
<https://x.com/garrytan/status/2102233173833007536|View tweet>


*Nikunj Kothari* — Partner at FPV Ventures

Kothari is all-in on Codex for Mac computer use, calling it "simply undefeated" for one-shotting manual workflows — and says Instinct and Muse are the best options for browser-based tasks on mobile with zero setup. He's also pushing back on "tokenmaxxing" as a product strategy: "companies boasting about tokenmaxxing have the worst product experiences." His take: good products are about curation and gardening, not throwing the kitchen sink at agents. Less is more.
<https://x.com/nikunj/status/2102186665863463199|View tweet>
<https://x.com/nikunj/status/2102049065504739366|View tweet>


*Peter Steinberger* — OpenClaw co-founder, OpenAI

Clarifying the record on the "Meta uses OpenClaw" story circulating online: Meta built their own agent inspired by OpenClaw, they didn't adopt it directly. Steinberger gave kudos to Nat and the Meta team. He also shared that OpenClaw passed a third-party security audit with nothing critical found — and made a pointed remark about platform independence: "The beauty of running a claw yourself: they cannot block you."
<https://x.com/steipete/status/2102116206371315854|View tweet>
<https://x.com/steipete/status/2102049706830647467|View tweet>
<https://x.com/steipete/status/2102044040397238286|View tweet>


*OFFICIAL BLOGS*


*Claude Blog — Claude in Chrome is generally available*

Claude in Chrome is now GA on all paid Claude plans. The big new capability: Claude can now take autonomous actions in Chrome — clicking, typing, navigating, filling forms — without requiring approval for every step, using your existing logins. This matters most for tools that don't connect to Claude natively: internal dashboards, legacy systems, vendor portals.

The centerpiece of the announcement is Anthropic's prompt injection defense stack, which has been substantially hardened since the pilot launched. Three layers work together: Claude is trained against a growing library of real-world injection attacks; probes scan web content before Claude acts on it and flag suspicious instructions; and a safety classifier reviews each action against the original user request before it runs. On their current red-team evaluation, no attacks succeeded against Claude Sonnet 5 or Opus 5 with probes plus the classifier active. Fable 5 showed a 0.3% success rate, with all confirmed breaks in low-severity scenarios.

Install from the Chrome Web Store. Enterprise admins can restrict it to approved domains.
<https://claude.com/blog/claude-in-chrome-generally-available|Read the full post>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
