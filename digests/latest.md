AI Builders Digest — November 3, 2026

*X / TWITTER*

- - -

*Andrej Karpathy*

Karpathy shipped HackerTube over the weekend: a YouTube experience filtered by 43 million Hacker News comments spanning 20 years, surfacing 6,454 videos the HN community keeps recommending. He used Claude Opus 5.5 on medium effort via Claude Code's desktop app and estimates it took about two hours total. His only "manual" contributions were spinning up a VPS, creating a Google Cloud API key, and buying the domain — Claude handled the rest, including deploying, securing, and optimizing the app. "Many awesome projects that would have normally taken weeks/months even can now be few-shotted for breakfast."

• <https://x.com/karpathy/status/2116957135661945283|Weekend hack: HackerTube>

- - -

*Peter Yang — AI educator and host of Behind the Craft*

Peter Yang teased four upcoming guests: Ashley Alexander (VP of Product at OpenAI), Nate Parrott (the Anthropic designer behind Claude's design system), Matt Pocock (whose AI coding agent curriculum has 300K+ GitHub stars), and Jacob Sansbury (who reportedly runs the most AI-pilled gaming company in the world at 10 people and $32M/year in Claude spend). He also shared a sharp quote from a Google Labs product director on the looming question of whether products even need a UI anymore: _"Anything that involves me creating something... there might be a reason for me to interact. Anytime I want to be entertained or consume something, I'm still the one using the product. But there are definitely products that I use today that I would be more than happy to not use."_ On his own AI tool stack: browser/computer use goes to ChatGPT + Codex, design/taste goes to Claude, and 24/7 agents go to Grok Bot.

• <https://x.com/petergyang/status/2117059131349868790|Upcoming Behind the Craft guests>
• <https://x.com/petergyang/status/2116987415319740756|Quote on products and UI>
• <https://x.com/petergyang/status/2116946320674152810|AI tool stack breakdown>

- - -

*Amjad Masad — CEO of Replit*

Replit CEO Amjad Masad issued a blunt warning: if you're on a subsidized AI subscription, expect a rug pull. He also highlighted a Replit product feature — a feedback widget that converts user feedback directly into agent prompts for building, closing the loop between user input and product iteration.

• <https://x.com/amasad/status/2117010858845089805|Warning on subsidized AI subscriptions>
• <https://x.com/amasad/status/2116998155925360965|Replit feedback widget>

- - -

*Guillermo Rauch — CEO of Vercel*

Rauch posted a strong take on AI and ownership: _"Own your intelligence. Anyone that opposes this has something to sell you (perhaps your own intelligence back to you.)"_ He's advocating for local models and open source, arguing that owning your own agents, harness, data, and runtime is the only durable path. He also shared that he's been testing Gemini on v0 with high-complexity projects and finding it impressive.

• <https://x.com/rauchg/status/2117000819623243925|Own your intelligence>
• <https://x.com/rauchg/status/2116988333096370443|Testing Gemini on v0>

- - -

*Aaron Levie — CEO of Box*

Levie made a sweeping prediction about knowledge work: we're moving from a world where AI helps humans work faster, to a world where humans help AI agents do the work. _"This turns everyone in one of these positions to that of a manager of a team of agents, instead of an individual contributor with just some added leverage from AI."_ The biggest impact zones: coding, cybersecurity, legal, biotech, and engineering. His key insight — the historic link between hours worked and output is breaking, and organizations that figure this out first will see compounding gains.

• <https://x.com/levie/status/2117134917847093491|The shift to managing agents>

- - -

*Garry Tan — President and CEO of Y Combinator*

YC's Garry Tan flagged Particle-1, a retrieval-focused model that matches much larger models in agentic retrieval tasks at 1/23 the price. He also noted that practical robotics is imminent, and reaffirmed that YC is the go-to for hard tech founders.

• <https://x.com/garrytan/status/2117137390016073977|Particle-1 model>
• <https://x.com/garrytan/status/2116941191526895975|Practical robotics>
• <https://x.com/garrytan/status/2116909591607099793|YC for hard tech>

- - -

*Thariq — formerly Claude Code at Anthropic*

Thariq is building a game with a new character — a taekwondo master who fights with fire — and updated the art style from 3D models to generated sprites. They shared a highlight intro video and are targeting a vertical slice next week.

• <https://x.com/trq212/status/2116976789046350040|New character and art style update>
• <https://x.com/trq212/status/2116977363728867664|Highlight intro video>

- - -

*Zara Zhang — Builder*

Zara built and shipped a creative demo: a Linktree-style page that renders as an actual tree. Short on words, long on vibes.

• <https://x.com/zarazhangrui/status/2117086544586780867|Linktree as an actual tree>

- - -

*Dan Shipper — CEO of Every*

Dan Shipper called out that "argon cooks" (a reference to Argon, likely a tool or product from Every's orbit) and flagged something he considers anti-competitive and "not cool" — though without more context from the linked sources, it's not clear what he's responding to.

• <https://x.com/danshipper/status/2117014507083948453|argon cooks>
• <https://x.com/danshipper/status/2116978123044688304|anti-competitive call-out>

- - -

*PODCASTS*

- - -

*Unsupervised Learning — Ep 95: Modal CEO on the Future of Inference, the Chaos of the GPU Market & Origins of the Sandbox Bet*

*The Takeaway:* The GPU market is still a late-night WhatsApp hustle — and the companies building serious AI infrastructure have to go far deeper into the stack than most people realize, or they'll be commoditized out of existence.

Eric Glyman is the founder and CEO of Modal, a cloud infrastructure platform used by AI teams who need to run serious compute workloads — from model inference to code sandboxes to fine-tuning. He's been building since late 2021, and Modal is now a multi-hundred-million dollar run rate business. The platform was initially built around serverless GPU functions, pivoted hard into Stable Diffusion hosting after ChatGPT, and has since grown into a full platform with inference, sandboxes, training, and storage.

On the GPU market: _"I went to GTC last year. It was like an open air drug market, but, like, GPUs. Walking around, like, talking to people, trying to get GPUs, and meeting people in hotel lobbies, exchanging numbers."_ Modal now does two to three compute deals per week across 25 different clouds, including providers in Indonesia and Europe — many of them former crypto miners who've had to learn uptime the hard way.

What separates Modal from commodity inference providers is infrastructure that took years to build: a proprietary container runtime (no Kubernetes, no Docker), their own file system for blazing fast container image loads, CPU and GPU snapshotting, and a custom RDMA-based peer-to-peer data transfer system to load large models in seconds. _"A massive source of alpha in this market is just not being afraid to do hard things."_

On where the inference market is headed: Glyman thinks straight token-serving is a race to the bottom, and differentiation will come from the platform — sandboxes, training, batch processing, fine-tuning — not from inference speed alone. _"Customers don't wanna buy single trick ponies. They wanna buy a multiproduct set of tools."_ He's also betting on continuing to scale up to Blackwell GPUs while keeping Hoppers busy on older, more cost-efficient workloads. His take on model size: LMs are basically very large lookup tables of facts, and as long as memory constraints keep pushing up, models will keep getting bigger.

<https://www.youtube.com/@RedpointAI>

- - -

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
