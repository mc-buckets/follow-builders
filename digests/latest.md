AI Builders Digest — September 28, 2026

*X / TWITTER*

*Thibault Sottiaux* (Codex & ChatGPT, OpenAI)
After what appears to be a service incident, Sottiaux gave the all-clear in a short post that drew over 13,900 likes: "Resets all propagated. That will be all. Have a fantastic weekend." Cryptic and minimal, but clearly the message a lot of people were waiting for.
<https://x.com/thsottiaux/status/2103911959544610829>

*Peter Yang* (AI educator and tutorial creator)
Noticed Claude's usage limits dramatically loosened — "they went from barely usable to basically unlimited" — and separately shared he's building a Japanese language learning app using Google's Gemini audio API (10 lessons, 10 phrases each). Also ran into an ambiguous support situation while trying out the new Google audio tools via @antigravity.
- <https://x.com/petergyang/status/2104066667361992892>
- <https://x.com/petergyang/status/2104059554204188833>

*Thariq* (Claude Code, Anthropic)
Marked roughly one year since posting early experiments using Claude Code to generate videos. Reflected on how much manual iteration was required back then — pointing out specific errors, nudging the model on details — compared to where things stand today. "Crazy how far things have come."
<https://x.com/trq212/status/2103897226154328502>

*Guillermo Rauch* (Vercel CEO)
Made a pointed case against AI-generated slop — and extended the concern beyond code. He's worried that _reading_ itself gets devalued as people grow exhausted by constant low-quality AI prose. He cited a viral thread where an AI tool explained in the PR description that a performance improvement wasn't due to a compiler change — but the developer missed it and attributed it to the compiler anyway. His bottom line: "I want AI in the service of understanding the universe and enhancing human cognition and creativity."
<https://x.com/rauchg/status/2103939888513274147>

*Garry Tan* (YCombinator President & CEO)
Shared his current favorite workflow for fixing production bugs: @capydotai with GStack /autoplan, running on GPT-6 medium reasoning. No lengthy explanation — just enthusiasm for the approach.
<https://x.com/garrytan/status/2103989902476259702>

*Peter Steinberger* (OpenClaw, OpenAI)
Reacted to a demo with notable enthusiasm: "Now I see why some people talk about AGI. This is so clever!" Not often you see that reaction from a seasoned engineer without caveats.
<https://x.com/steipete/status/2103883264054505493>

*Dan Shipper* (Every, CEO)
Experimenting with Claude Opus 5.5 as a film director: wrote a novelization of Plato's Protagoras, then had Opus 5.5 adapt it into a short film scene by scene. A low-key but genuinely interesting test of what frontier models can do with classical narrative.
- Scene 1: <https://x.com/danshipper/status/2103850415930708437>
- Scene 2: <https://x.com/danshipper/status/2103894152316645620>

*PODCASTS*

*No Priors — "Why Diffusion Will Win AI Inference with Inception Co-Founder and CEO Stefano Ermon"*

*The Takeaway:* The most widely used architecture for language models — generating text one word at a time — has a structural bottleneck at inference that diffusion models are built to avoid, and the Stanford researcher who helped invent diffusion thinks that gap will only matter more as AI scales.

Stefano Ermon spent a decade at Stanford developing generative models before they were fashionable. His lab's 2019 work on score-based generative models became the mathematical foundation for diffusion — the approach behind Stable Diffusion, Midjourney, Sora, and essentially every serious image and video generation tool today. In 2024, his lab demonstrated that diffusion could match the quality of a 1B-parameter autoregressive language model while generating text roughly 10x faster. That result led him to co-found Inception.

The core argument is about hardware efficiency. Today's language models generate text sequentially — one token at a time, left to right — which means GPUs sit mostly idle while weights are shuffled through memory. Diffusion models generate many tokens simultaneously, which maps far better to how GPUs actually work. "The bitter lesson is that the more parallel solution is the one that is eventually going to win."

Inception's Mercury models are already in production, reaching quality comparable to fast frontier models (Claude Haiku, GPT-4o mini class) while running significantly faster. One customer, Open Call — a voice agent company — switched from running autoregressive models on custom Cerebras chips to Mercury on standard NVIDIA GPUs, getting comparable speed at lower cost with broader availability.

Beyond speed, Ermon points to controllability as an underappreciated structural advantage. Autoregressive models finish generating before you can evaluate the output against any reward or constraint. Diffusion models generate coarse-to-fine, meaning external signals can steer the output from the very beginning — potentially a meaningful edge for enterprise use cases where outputs need to stay on-brand or within guardrails.

Inception is 50 people, two years old, and still mostly R&D-heavy — building training pipelines, a custom serving engine, and post-training infrastructure from scratch since nothing in the open-source ecosystem handles diffusion-based LLMs. The closed-source bet is intentional: Ermon sees the serving stack itself as defensible IP.

https://www.youtube.com/@NoPriorsPodcast

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
