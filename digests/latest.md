*AI Builders Digest — July 2, 2026*

*X / TWITTER*

*Boris Cherny* (Claude Code, Anthropic)
Claude Desktop on Linux is now available — the most-requested platform addition. The announcement landed 3,500+ likes, signaling just how long the Linux community had been waiting.
https://x.com/bcherny/status/2072000214634742243

*Thariq* (Claude Code, Anthropic)
Cleared up confusion around Claude Code's updated safety classifiers ahead of Fable's return. A small fraction of routine coding and debugging tasks may be flagged and fall back to Opus — not a widespread problem. He added: "We're continuing to refine these safeguards to better distinguish genuine misuse from legitimate requests and reduce false positives."
https://x.com/trq212/status/2072185565076988326
https://x.com/trq212/status/2072185566695977161

*Claude* (Anthropic official)
Anthropic launched Claude Sonnet 5 as the new default on Free and Pro tiers, live across all Claude apps and the API. Sonnet 5 is described as "a substantial improvement over Sonnet 4.6 on reasoning, tool use, coding, and knowledge work" — with performance close to Opus 4.8 at lower prices. Early partners noted it "finishes complex tasks where previous Sonnets stopped short, checks its own output without being asked." Introductory pricing runs through August 31.
https://x.com/claudeai/status/2072017452335087996
https://x.com/claudeai/status/2072017455833100494
https://x.com/claudeai/status/2072017457057853480

*Aaron Levie* (Box CEO)
Three substantial posts. On the Fable safety delay and resulting industry framework: Levie called the process messy but noted the framework being developed with Amazon, Microsoft, Google, and others for assessing model jailbreaks is a meaningful step — while flagging a real risk: "It would be a bad outcome if every release after this level of capability required the same review process, and we don't get the same rate of breakthroughs we've been seeing." On enterprise AI: Box ran Sonnet 5 through their Complex Work Eval benchmark and found it outperforms Sonnet 4.6 in Energy (+4.7pp), Retail (+4.4pp), and Professional Services (+2.6pp), particularly on complex multi-step document reasoning. On AI and jobs: a Box survey of 1,600+ mid-to-large companies found 58% expect headcount growth over the next three years — climbing to 79% among the most advanced AI adopters, inverting the narrative that AI adoption leads to fewer hires.
https://x.com/levie/status/2072172275017879829
https://x.com/levie/status/2072046374045249671
https://x.com/levie/status/2071992799109824562

*Guillermo Rauch* (Vercel CEO)
Two notable posts. Vercel launched "Vercel Services" — you can now collocate a Python backend API, an ExpressJS server, and a React SPA in one Vercel project, running all locally with `vc dev`, deploying and rolling back together, with shared observability and internal networking. Separately, announced a partnership with Shopify to push "the agentic web forward."
https://x.com/rauchg/status/2071966055308607765
https://x.com/rauchg/status/2072044844965400589

*Amjad Masad* (Replit CEO)
Flagged Etched as the first hardware system designed from the ground up for modern LLM inference — noting that AI running on pre-LLM generic hardware is a key reason inference costs remain high.
https://x.com/amasad/status/2071992110132117740

*Madhu Guru* (ex-Google, led Gemini / Veo / Nano)
Called out the biggest gap for traditional PMs adapting to AI-native building: "a lack of magical thinking." A decade of frameworks and metric obsession bred constraint-first, incremental thinking. His fix on his teams: imagine tech from 100 years in the future and work backward from the experiences it enables. "The funny thing is, that technology from the future is here."
https://x.com/realmadhuguru/status/2071970221477470694

*Peter Steinberger* (OpenClaw, OpenAI)
Made a point that's easy to miss amid model price debates: "Price per token != cost per task." As models get more capable, they complete tasks in fewer tokens — meaning a higher per-token price can still be cheaper end-to-end.
https://x.com/steipete/status/2072144627474579925

*Aditya Agarwal* (GP at SouthPkCommons, ex-CTO Dropbox)
Sharp observation: "It is a very strange state of the world where the models powering innovation in the USA are Chinese open source models."
https://x.com/adityaag/status/2071983952894837062

*Nan Yu* (Head of Product at Linear)
Raised an interesting edge case in the "distillation" debate: if Cursor used Claude-generated outputs as training data in its early days, that data was technically distilled from Claude — questioning how broadly the concept applies to model training.
https://x.com/thenanyu/status/2071973229070033322

*Peter Yang* (AI educator and creator)
Publicly asked what Claude's Fable usage limits actually mean in practice — specifically, whether hitting 50% of weekly usage makes Fable unavailable. The question drew 72 replies, suggesting the new usage tiers are genuinely confusing to power users.
https://x.com/petergyang/status/2072165346476511583

*Garry Tan* (YCombinator President & CEO)
Shared that GBrain — his personal knowledge tool — hits its stride at 10,000+ markdown files, whether for personal notes or a company knowledge base.
https://x.com/garrytan/status/2071910876496757145

*Zara Zhang* (builder)
Shared a sharp take on taste: "Taste isn't valuable because it's impossible to copy. Taste is valuable exactly because it defines what everyone else chooses to copy."
https://x.com/zarazhangrui/status/2072197929138602079

*PODCASTS*

*Training Data — "Why Hardware-Software Co-Design Is AI's Real 100x: Dylan Patel of SemiAnalysis"*

_The Takeaway:_ The real source of AI's efficiency gains isn't hardware improvements or model improvements in isolation — it's co-designing all three layers (hardware, systems software, and model architecture) simultaneously, which can turn three separate 2x improvements into a genuine 100x leap.

Dylan Patel built SemiAnalysis — now reportedly crossing $100M in revenue with 90 people — by obsessively tracking the semiconductor supply chain from lithography chemicals to GPU architecture. He started moderating hardware forums at 12, reached Starcraft grandmaster on the North American ladder, and now attends 40+ conferences a year across the full supply chain. The resulting firm combines technologist-engineers and former hedge fund analysts who, as he puts it, "organically fight it out."

The central insight: most AI benchmarking is dishonest because people compare an optimized configuration of their chip against a suboptimal one from a competitor. Patel launched InferenceX to fix this — a living benchmark running daily across 15+ chip types (donated by CoreWeave, Crusoe, Google, Amazon, OpenAI, and others, totaling over $50M in hardware), on the latest models and software stacks that update twice a week. It publishes the Pareto-optimal curve between throughput and latency, with open-source containers anyone can run.

On NVIDIA vs. TPUs, he refuses to declare a winner: "The way OpenAI's models are headed, it would be a terrible decision for them to use TPUs potentially. And the way that Anthropic and Google's models are headed, it's actually a terrible decision potentially for them to train with GPUs." The model architecture is inseparable from the chip it runs on. DeepSeek's expert shapes were literally tuned for Hopper; its next version targets Blackwell. CUDA's moat has softened not because of kernel-writing difficulty but because the best open-source models are co-designed for NVIDIA hardware, pulling the whole downstream ecosystem along.

On scale: he forecasts OpenAI and Anthropic alone will have over 100 gigawatts combined by 2030. Intelligence per watt has improved roughly 40x in recent years — mostly from model improvements, not hardware. Model costs have dropped 60x per year for equivalent quality. By 2040, he thinks the majority of incremental compute will be in space. On Anthropic specifically: Q2 was profitable on a net income basis (excluding SBC), with per-token margins north of 80% on Opus 4.8 API pricing.

https://www.youtube.com/watch?v=f6D_aiy8qyU

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
