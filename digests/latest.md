AI Builders Digest — September 20, 2026

*X / TWITTER*

*Anthropic's Thariq (Claude Code team)* dropped the week's biggest developer news: Claude Code now supports AGENTS.md. Starting in version 2.1.277, if there's no CLAUDE.md in a folder, Claude will check for and use AGENTS.md instead. The feature is built on top of Claude Code mods — an upcoming way to customize the Claude Code harness — and can be toggled in /config. The announcement pulled 25,000+ likes and 2,000+ retweets.
- Announcement: <https://x.com/trq212/status/2101009392611278961>
- Mods context: <https://x.com/trq212/status/2101009393731223817>
- Source code: <https://x.com/trq212/status/2101009395052343462>

*OpenAI's Thibault Sottiaux* (Codex & ChatGPT team) teased a packed upcoming keynote, working alongside Romain Huet and Sam Altman. He called the lineup of new things "a bit ridiculous all in quick succession" and promised some items next week so the wait isn't too long.
- <https://x.com/thsottiaux/status/2101157729037586694>

*Peter Yang*, creator of AI tutorials and guides, spotlighted Meta's Muse personal agent with a compelling real-world example: Muse called his Comcast customer support line and negotiated $288 in annual savings on his cable bill. He says most companies' customer support lines "are NOT ready for agents" and believes Muse could become Meta's next billion-user app. He also shared a wry observation: AI getting smarter seems inversely correlated with humans' ability to write coherent sentences.
- Muse demo video: <https://x.com/petergyang/status/2101033599319613533>
- Bill negotiation transcript: <https://x.com/petergyang/status/2101083891507593576>
- Spelling joke: <https://x.com/petergyang/status/2101104320897040627>

*Vercel CEO Guillermo Rauch* shared a striking data point from Vercel AI Gateway: open models hit 78.4% of token volume vs. 21.6% for closed models — possibly a record. On spend, Moonshot AI and DeepSeek together now surpass OpenAI. He's also enthusiastic about Jev adoption, calling the anecdata "shocking" and framing it as downstream of the "AI is too expensive/slow" zeitgeist driving people to optimize and deploy AI in more places.
- Open model share data: <https://x.com/rauchg/status/2101186741042663579>
- Jev adoption: <https://x.com/rauchg/status/2101079472732848510>

*Box CEO Aaron Levie* demoed Jev integrated with Box for enterprise document automation: the agent pulls an incident report, decides whether it's customer-facing and how severe it is, moves the file into the right folder (escalate/monitor/review), and sets metadata — all nearly instantly and at almost no cost. He sees applications across insurance claims, contract management, loan processing, and security reviews.
- <https://x.com/levie/status/2101007708044574906>

*Nikunj Kothari*, partner at FPV Ventures, built a community site called Jevable to showcase weekend Jev demos, filterable by category with a + button for submissions. He also shared his own demo: scoring 3,000 kid snacks against multiple criteria in 28 seconds for $0.11.
- Jevable site: <https://x.com/nikunj/status/2101077053567332618>
- Kid snack scoring demo: <https://x.com/nikunj/status/2101006585481073093>

*Zara Zhang*, a builder focused on AI products, offered a sharp take on content quality: "It's hard not to create slop when most things you consume are slop. To fix output, first fix input."
- <https://x.com/zarazhangrui/status/2101123389528457596>

*Peter Steinberger* (OpenClaw + OpenAI) shared updates on his roboclaw project: the agent now runs their team server, lives on Discord, talks with GPT Live, and tracks all active and past coding sessions simultaneously. Team members can query it for session context during meetings.
- <https://x.com/steipete/status/2101141707375227372>

*PODCASTS*

*No Priors — Why Diffusion Will Win AI Inference*
Episode: "Why Diffusion Will Win AI Inference with Inception Co-Founder and CEO Stefano Ermon"

*The Takeaway:* Diffusion models — built for massively parallel inference — may be the "transformer moment" for AI generation, making autoregressive models look like the old sequential RNNs they replaced.

Stefano Ermon is one of the fathers of diffusion models, a Stanford professor since 2014 and now CEO of Inception, a ~50-person AI lab building diffusion-based language models. His bet: speed and efficiency will define the next wave of AI, and diffusion models are structurally better positioned for inference-time scaling than the autoregressive transformers every major lab currently uses.

The core insight is architectural. Autoregressive models generate text one token at a time — sequential, memory-bound, poorly matched to how GPUs actually work. Diffusion models generate many tokens simultaneously, creating an inference workload that maps naturally to GPU parallelism. "The bitter lesson is that the more parallel solution is the one that is eventually going to win," Ermon says.

Inception's Mercury models now match the quality of frontier "flash/mini" models (Haiku, GPT-4o mini equivalents) while being significantly faster. One voice agent customer, Open Call, switched from Cerebras custom chips to Inception's diffusion LLMs and got equivalent speed on standard NVIDIA GPUs — more available and cheaper.

What's counterintuitive: diffusion models may also be easier to control than autoregressive ones. Because generation is coarse-to-fine rather than sequential, you can steer the output midway through using external reward signals — something that's much harder when you have to wait until the full sequence is complete.

Beyond speed, Ermon hints at emerging advantages: better data efficiency (each training example is augmented by many noisy views) and potentially stronger scaling during RL post-training, since inference is the bottleneck for generating rollouts. "We don't know what we're going to find," he says — and that uncertainty is the point.

<https://www.youtube.com/@NoPriorsPodcast>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
