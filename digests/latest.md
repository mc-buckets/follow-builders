*AI Builders Digest — May 7, 2026*


*X / TWITTER*

*Sam Altman — OpenAI CEO*

OpenAI CEO Sam Altman signaled that voice interfaces are about to become significantly more important: "pretty excited for voice models to get great" — noting that people are already changing how they interact with AI. Separately, he promised a goodwill gesture for people who applied to the GPT-5.5 party but couldn't get in.

- https://x.com/sama/status/2051464865634742334
- https://x.com/sama/status/2051318922805436896

*Aaron Levie — Box CEO*

Box CEO Aaron Levie flagged a trend that's early but about to get very big: both Anthropic and OpenAI now have active enterprise agent deployment programs. He was pointed about what this actually requires — upgrading IT systems, feeding agents the right context, modernizing workflows to work alongside agents, managing the human-agent relationship, and driving adoption. "There's no shortcut to getting that intelligence applied to a business process in a stable way" — which is creating new opportunities for jobs and firms across the market.

- https://x.com/levie/status/2051344780328858040

*Guillermo Rauch — Vercel CEO*

Vercel CEO Guillermo Rauch announced `npx deepsec`, an open-source agent orchestrator for deep security reviews. Built originally for internal use, Vercel ran it against major OSS projects before releasing it publicly. The pitch: coding agents can now find critical vulnerabilities in minutes that would take teams months to spot — and by running on Vercel Sandbox, thousands of agents can scrutinize a codebase in parallel. OSS maintainers can reach out to Rauch directly for a sponsored run.

- https://x.com/rauchg/status/2051386798899888539

*Garry Tan — YCombinator President & CEO*

YCombinator President Garry Tan shipped GBrain v0.27, adding support for non-Anthropic and non-OpenAI embeddings and LLMs. He also made the case for what sets GBrain apart: it's not a memory layer _or_ a code tool _or_ a search engine — "it's all three unified under one graph with one query interface." He uses it daily with a 100K markdown file setup via his OpenClaw+Hermes Agent configuration.

- https://x.com/garrytan/status/2051517574589116510
- https://x.com/garrytan/status/2051525161380364315

*Peter Steinberger — OpenClaw co-creator*

Peter Steinberger (steipete on X) shipped Crabbox 0.5.0 — remote CI boxes now with desktop/browser leases, VNC + authenticated WebVNC, AWS Windows + WSL2 support, and screenshots. More practically: agents can now reproduce bugs directly in ephemeral "crabboxes," set up the exact state to test and fix, and post videos of the reproduction directly on PRs.

- https://x.com/steipete/status/2051485798613111116
- https://x.com/steipete/status/2051557150040711425

*Nikunj Kothari — FPV Ventures Partner*

FPV Ventures partner Nikunj Kothari offered a cold-water take on recent startup vintages: companies founded 2023-2025 that prioritized launch videos and distribution over retention are now facing the consequences, with the seed-to-Series-A conversion gap widening and more acquihires on the way. On a separate note, he called Gemini Flash his most-used model in production — cheap, 1M context windows, great structured output — adding that Google's new live voice model is "mindblowingly good."

- https://x.com/nikunj/status/2051349526171287930
- https://x.com/nikunj/status/2051321911741972900

*Peter Yang — Roblox PM and AI newsletter writer*

Roblox PM and AI newsletter author Peter Yang (140K+ readers) framed AI's progression in three waves: coding first, knowledge work second, personal agents third. He also crowdsourced ideas for getting his 8-year-old started building agent apps she can share with her class and teachers.

- https://x.com/petergyang/status/2051508988936937764
- https://x.com/petergyang/status/2051459299860533483

*Amjad Masad — Replit CEO*

Replit CEO Amjad Masad highlighted two wins from the community: a user who leveraged Replit to find investors and land meetings, and a student who built a multi-modal learning platform for deaf students — which Masad flagged as a strong example of AI applied to real educational challenges.

- https://x.com/amasad/status/2051511694040744139
- https://x.com/amasad/status/2051406536443035922

*Swyx — AI engineer and Latent Space podcast co-host*

Swyx (swyx on X) reconstructed an OAI vs. Anthropic valuation comparison from WSJ data: OpenAI at ~$850B valuation / ~$30B ARR vs. Anthropic at ~$900B / ~$44B ARR — though per Denise Dresser, if Anthropic used OpenAI's revenue recognition methodology, Anthropic's ARR number would be $8-10B lower.

- https://x.com/swyx/status/2051440392722391180

*Aditya Agarwal — South Park Commons General Partner*

South Park Commons GP Aditya Agarwal pushed back on the venture accelerator model: "We have never desired to be an accelerator. Velocity is not interesting without a grounding towards true north."

- https://x.com/adityaag/status/2051330205902581842

*Matt Turck — FirstMark Capital VC*

FirstMark Capital VC Matt Turck offered some dry humor: VCs should adopt the startup literal-naming trend, with suggestions including "The Capital Deployment Company of San Francisco," "The Ghosting Company," and "The Liquidated Preference Firm of Miami."

- https://x.com/mattturck/status/2051382629681828306


*OFFICIAL BLOGS*

*Anthropic Engineering*

*<https://www.anthropic.com/engineering/claude-code-auto-mode|Claude Code auto mode: a safer way to skip permissions>*

Anthropic Engineering introduced _auto mode_ for Claude Code — a new safety layer between manually approving every command and the `--dangerously-skip-permissions` flag that disables all guardrails. The motivation: 93% of manual prompts get approved anyway, creating approval fatigue, but blanket permission bypass has caused real incidents (deleting remote git branches, accidentally leaking a GitHub auth token, attempted production DB migrations).

Auto mode uses two defenses: an input-layer prompt-injection probe that scans tool outputs before they reach the agent, and a two-stage transcript classifier (running on Sonnet 4.6) that evaluates each tool call before execution. The classifier sees only user messages and tool calls — assistant text and tool results are stripped to prevent the agent from reasoning its way past the classifier.

Numbers: 0.4% false positive rate on real traffic (n=10,000) and a 17% false-negative rate on real overeager actions (n=52). The main miss pattern is the classifier finding "approval-shaped evidence" without checking whether it covers the actual blast radius of the action.

Auto mode is not a replacement for careful human review on high-stakes infrastructure. But for anyone currently running `--dangerously-skip-permissions`, it's a meaningful safety upgrade.

https://www.anthropic.com/engineering/claude-code-auto-mode


*PODCASTS*

*Training Data — Waymo's Dmitri Dolgov: 20 Million Rides and the Road to Full Autonomy*

_The Takeaway:_ Dmitri Dolgov spent 20 years building something most people thought was impossible, and the reason Waymo made it was refusing to treat safety as a variable.

Dolgov joined Google's self-driving car project in 2009 after competing in the DARPA Urban Challenge, studied physics at the Moscow Institute of Physics and Technology, and earned a PhD in AI. Waymo has now given over 20 million fully autonomous rides, with 10 million happening in just the last seven months.

His most counterintuitive point: end-to-end AI models are necessary but not sufficient. The "end-to-end vs. something else" framing is a false dichotomy. Waymo augments learned representations with structured intermediate outputs — enabling closed-loop evaluation, richer reinforcement learning reward functions, and runtime validation that pure end-to-end architectures can't provide.

On hype cycles: Dolgov has watched AV get overhyped twice. A breakthrough reshapes the early curve but doesn't change the long tail. What kept Waymo running wasn't better tech — it was mission clarity: "somebody loses their life to a crash on our roads every twenty-six seconds."

One striking technical detail: Waymo's LiDAR once detected a pedestrian hidden behind a stopped bus by picking up the movement of her feet underneath the vehicle — sparse signal, but enough for the AI to predict her trajectory and stop the car safely.

Today Waymo drives 4 million miles per week in full autonomy. Their data across 170 million miles shows 13x safer performance than human drivers in serious injury-causing collisions — currently preventing one serious injury every eight days, a number that will compound as they expand to London and Tokyo.

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
