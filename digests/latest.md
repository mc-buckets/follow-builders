AI Builders Digest — July 16, 2026

*X / TWITTER*

*Sam Altman* (OpenAI CEO)

GPT-5.6 Sol growth is "insane," with Altman crediting the inference team's "heroic work" to keep up — but warning that capacity hiccups may be coming soon. He also dropped a cryptic standalone post: "also, a reason to favor open-source harnesses," suggesting that OpenAI's own infrastructure scaling strain is making the case for open alternatives.

https://x.com/sama/status/2077106587307798989
https://x.com/sama/status/2077053226080436235

*Thibault Sottiaux* (Codex & ChatGPT at OpenAI)

Sottiaux is actively soliciting feedback as Codex approaches 9M usage events — asking users whether to reset limits or give it space. He also launched a promotion offering $100 in Codex credits to the first 10k people who tweet what they love about GPT-5.6 Sol, and separately crowdsourced improvements for ChatGPT Work.

https://x.com/thsottiaux/status/2077271889626706300
https://x.com/thsottiaux/status/2077248807533003257
https://x.com/thsottiaux/status/2077212009071075330

*Aaron Levie* (Box CEO)

Levie wrote the cleanest framing of why coding captured AI agents first: code can be tested immediately, while most enterprise work (sales pitches, contracts, stock trades) only gets validated when it hits the real world. His prediction: the next wave of agent adoption will require companies to build evals for knowledge work, and "the enterprises that are able to eval their knowledge work the best also stand to gain the most from AI." He also weighed in on a proposed AI standards body, cautiously endorsing it as far better than government-speed regulation.

https://x.com/levie/status/2077201458546745553
https://x.com/levie/status/2077043523703243070

*Ryo Lu* (Designer at Cursor AI)

Lu wrote a long-form reflection on the specific pain of loving a craft when AI can now approximate its outputs. The core argument: AI raises the floor and accelerates the work, but "it cannot want on your behalf" — the original curiosity, the private fire that made you care, is both irreplaceable and now more important to protect. Worth reading in full.

https://x.com/ryolu_/status/2077162119506833627

*Guillermo Rauch* (Vercel CEO)

Vercel is opening its dataset of AI token flows from the Vercel AI Gateway, calling it "fascinating insights." Separately, he promoted agentmail's new Vercel integration — agents can set up email capabilities with a single `vercel install agentmail` command, no signup required.

https://x.com/rauchg/status/2077176141790752798
https://x.com/rauchg/status/2077154901013221444

*Thariq* (Claude Code at Anthropic)

Thariq is using Claude Code to build a personal competitive Pokemon analytics tool — it pulls live usage stats from Smogon's npm library and writes reports on matchups, damage breakpoints, and team theory. He's teasing open-sourcing it. A useful demo of Claude Code as a research assistant for any structured, API-accessible domain.

https://x.com/trq212/status/2077051280267399550
https://x.com/trq212/status/2077051282146431092

*Swyx* (AI engineer, Latent Space / AI Engineer)

Swyx is organizing a SF demo night for personal AI engineers this Thursday at New Media Lab. He's enthusiastic about the staying power of personal AI — speakers from the last meetup got acquired by Amazon's hardware division, and he's still a daily active user two years later.

https://x.com/swyx/status/2077243443391422813

*Peter Yang* (AI tutorials creator)

Yang previewed an upcoming video covering his complete 7-step setup for using ChatGPT Work (Codex) to handle most computer tasks — model selection, email, calendar, and recurring task management included.

https://x.com/petergyang/status/2077196815951417649

*Dan Shipper* (CEO of Every)

Shipper is staking his "we called it early" flag on Codex, pointing to Every's coverage from six months ago as proof subscribers were ahead of the wave. Also hosting an in-person Every subscriber meetup in Brooklyn.

https://x.com/danshipper/status/2077196636971815135

*Aditya Agarwal* (General Partner at South Park Commons, ex-CTO of Dropbox)

Agarwal flagged a real UX regression in the new ChatGPT app — the added feature depth makes it feel too heavyweight for the quick, casual queries he used to fire off 15–20 times a day. A useful signal for product teams: feature richness and lightweight daily utility can be in direct tension.

https://x.com/adityaag/status/2077130899733553560

*Nikunj Kothari* (Partner at FPV Ventures)

Quick prediction: the most technically sharp engineers waiting on AI agents are filling that idle time on X, and time-on-X in tech will keep rising as AI takes over execution tasks.

https://x.com/nikunj/status/2077144910508257317

*Claude* (Anthropic official account)

Anthropic launched Claude for Teachers — a K-12-focused product that generates lesson plans starting from state standards and curated curricula via Learning Commons, then produces student-facing materials ready to revise and bring to class. Privacy-forward: no model training on conversations, FERPA-compliant data processing.

https://x.com/claudeai/status/2077047279689535705
https://x.com/claudeai/status/2077047280767488218
https://x.com/claudeai/status/2077047282109714488

*PODCASTS*

*Training Data — "Anthropic's Katelyn Lesse & Angela Jiang: Building an Ecosystem, not a Walled Garden"*

_The Takeaway:_ Anthropic Platform thinks about the agentic stack in three layers — knowledge, execution, and coordination — and they're now moving into the coordination layer, where you assign distinct "jobs to tokens" rather than just steering models with scaffolding.

Katelyn Lesse and Angela Jiang, both on Anthropic's Platform team (responsible for the developer APIs and the infrastructure powering both Claude's consumer products and external builders), offer rare specificity about how they make product decisions at the frontier.

Two counterintuitive points stand out. First, they deliberately keep internal and external platform products identical — no bifurcation — because building for their own engineers is the best stress test for what external builders actually need. Second, on harnesses: as models get smarter and more steerable, you can delete most of the scaffolding that used to guide them step-by-step. The real harness work now is _letting models run longer_ — sandboxes, context management, multi-agent coordination — not hand-holding prompts.

Their framework for the next phase is "strategies": instead of just running an agent longer or swapping in a bigger model, you can assign tokens different jobs. One token advises, another executes, another grades. As Lesse puts it: "You can take that same token and choose to actually reflect on your past agentic sessions and write learnings to memory so that the next agent does a good job."

On the open vs. walled garden question: Anthropic isn't precious about infrastructure. They've partnered with Modal, Vercel, Cloudflare, and Amazon on sandboxes — what they care about is the architecture and interfaces, not controlling the compute.

https://www.youtube.com/watch?v=vPnVTHYplrQ

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
