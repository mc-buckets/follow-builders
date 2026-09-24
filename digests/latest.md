*AI Builders Digest — September 24, 2026*

*X / TWITTER*

*Boris Cherny* — Claude Code engineer at Anthropic — had the most technically striking posts of the day. He used Opus 5.5 to formally verify the Claude Agent SDK using Lean, generating 16 PRs that fixed bugs and race conditions from just a couple of short prompts. He noted that combining Lean and TLA+ works well for finding concurrency and state management issues, and that Claude is excellent at both even if you don't know the languages well. He also shared a head-to-head: both Opus 5.5 and Fable 5.1 ported HAProxy from C to Rust, passing nearly all tests, but Opus 5.5 finished in 9.5 hours vs. Fable's 12 hours — and at 51% less cost.
- https://x.com/bcherny/status/2102543349102338309
- https://x.com/bcherny/status/2102439069053747549

*Cat Wu* — Claude Code and Cowork engineer at Anthropic — announced that Claude Opus 5.5 is now the default model in Claude Code and the Claude app for Pro, Max, and Team plans. Effort medium mode is comparable to Fable 5.1 on intelligence but faster, and rate limits go 25% further compared to Opus 5.
- https://x.com/_catwu/status/2102437713781944397

*Alex Albert* — Researcher at Anthropic — shared a Blender project powered by Opus 5.5: a historically accurate 3D recreation of San Francisco's Market Street as it stood on April 17, 1906, the afternoon before the earthquake. The full prompt — sourcing Sanborn fire insurance maps, the Miles Brothers film, period photographs, and USGS topography — is worth reading. His takeaway: better 3D modeling and vision in Opus 5.5 means you can build an entire world from a single prompt.
- https://x.com/alexalbert__/status/2102466523164274839
- https://x.com/alexalbert__/status/2102466524934271381

*Thariq* — Claude Code engineer at Anthropic — pushed back on how builders are using model capability gains. His contrarian take: the right move isn't to ship 10x more features to production, but to spend more time understanding users, running experiments, and building prototypes so you ship things that actually work. He also noted that Fable-level intelligence at workflow-friendly costs has changed how he uses Claude day to day.
- https://x.com/trq212/status/2102548686303854790
- https://x.com/trq212/status/2102477527688388752

*Thibault Sottiaux* — on the Codex and ChatGPT team at OpenAI — announced GPT-6 Sol and Luna. Significant capability improvements across the board, plus a 50% permanent API price reduction. OpenAI is also loading a banked reset into Plus, Pro, and Business accounts. He framed it as the payoff of investing in frontier models: you build capability at the top, then use it to bring intelligence to everything else more cheaply.
- https://x.com/thsottiaux/status/2102463847714247142
- https://x.com/thsottiaux/status/2102440619616682120

*Aaron Levie* — CEO of Box — called it an "insane day in AI" as Opus 5.5 price cuts landed alongside the GPT-6 price drop. He framed the dynamic as Jevons paradox for agents: every time AI gets cheaper, the addressable use cases for agents expand dramatically. Box ran their own Opus 5.5 enterprise tests and saw: 63% fewer tokens used, 42% less verbosity, 30% faster vs. Opus 5 — with large accuracy gains on financial services due diligence, cloud cost analysis, client account management, and clinical data analysis tasks.
- https://x.com/levie/status/2102477253070430322
- https://x.com/levie/status/2102448415775051790

*Guillermo Rauch* — CEO of Vercel — ran fresh Next.js evals: Opus 5.5, GPT-6 Sol, and Fable 5.1 all scored 97%, with Grok 4.7 at 94% but at 2-7x lower cost. He also made a broader point: "Software will never die again. You liked Google Reader? Cool, you can generate and deploy your own. Yours, forever." And he praised Anthropic's design taste in shipping, calling it Next.js at its finest.
- https://x.com/rauchg/status/2102519097770885231
- https://x.com/rauchg/status/2102594015669756323
- https://x.com/rauchg/status/2102438365455167883

*Dan Shipper* — CEO of Every — shared two pieces worth reading: a vibe check on Opus 5.5 vs. GPT-6 Sol, and a piece on why AI automation creates more (not less) valuable work for human experts. He gained nearly 10k followers in one day, likely from the model launch coverage.
- https://x.com/danshipper/status/2102556723244564715

*Garry Tan* — President and CEO of YCombinator — recommended Capy (capydotai) as a tool that lets him ship PRs much faster than Codex or Claude Code alone. He also pushed the broader mission: teaching the world to prompt and maximally use AI so everyone can see how it gives them wings.
- https://x.com/garrytan/status/2102544711647129902
- https://x.com/garrytan/status/2102501556348440983

*Peter Yang* — AI newsletter creator with 110k subscribers — said Opus 5.5 is the most excited he's been about a Claude model in a while.
- https://x.com/petergyang/status/2102577425838485916

*Peter Steinberger* — co-creator of OpenClaw at OpenAI — shared that Astra (Google DeepMind's AI assistant) found a roughly 14-year-old bug in libuv that was causing ChatGPT to crash on macOS 27. A notable example of AI catching deep, long-lived infrastructure bugs.
- https://x.com/steipete/status/2102501642176528743

*Sam Altman* — CEO of OpenAI — posted a quick correction: he meant to say VOICE not VIDEO in an earlier post (and said sorry for the disappointment). He also commented on startups being naturally good at something that's hard to maintain at scale — no further detail, but it sparked significant engagement.
- https://x.com/sama/status/2102512794235207758
- https://x.com/sama/status/2102469008079679640

*Aditya Agarwal* — General Partner at SPC and co-founder of Bevel Health — hosted Dmitri Dolgov from Waymo for a fireside. His highlight: Waymo's extensive eval and testing infrastructure for releasing 2-ton robots at 30mph through city streets. His 9-year-old asked to attend — a signal of how compelling physical-world robotics can be.
- https://x.com/adityaag/status/2102457464432284019

*Claude* — official Anthropic account — announced Opus 5.5's availability and showcased Artifacts: an algorithmic drawing program (every drawing unique per seed) and a toy brick-building app that turns a photo or description into a buildable model.
- https://x.com/claudeai/status/2102471892099866883
- https://x.com/claudeai/status/2102471889092276516
- https://x.com/claudeai/status/2102471885061812714

*Josh Woodward* — VP at Google Labs and the Gemini App — celebrated a "big milestone" without details.
- https://x.com/joshwoodward/status/2102498448364954083

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
