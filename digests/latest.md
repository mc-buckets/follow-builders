*AI Builders Digest — August 19, 2026*


*X / TWITTER*

*Thibault Sottiaux* (Codex & ChatGPT, OpenAI) is crowdsourcing product ideas in a big way — his open ask, "What is an obvious thing that we should do with Codex, API or our models that we should just do but haven't yet?", drew nearly 4,700 replies. It's a rare public invitation for the community to directly shape OpenAI's near-term roadmap. He also lightened the mood with an ABBA parody about shipping code after midnight.
- <https://x.com/thsottiaux/status/2089500941842342287|What should Codex do next? (4,700+ replies)>
- <https://x.com/thsottiaux/status/2089604619936956778|Codex After Midnight (ABBA parody)>

*Boris Cherny* (Claude Code, Anthropic) teased ongoing quality-of-life improvements to Claude Code, with two posts hinting at new features rolling out: "Small quality of life improvements like this add up. More on the way" and inviting user feedback on something new.
- <https://x.com/bcherny/status/2089538781909332210|QoL improvements, more coming>
- <https://x.com/bcherny/status/2089537919795212565|Let us know what you think!>

*Thariq* (Claude Code, Anthropic) made a contrarian observation: recent procedurally-generated art, video editing, and 3D game demos have updated his view that LLM coding models outperform diffusion models at a lot of creative work. He also promoted the new `/design` command in Claude Code for in-context UI design.
- <https://x.com/trq212/status/2089415712007938315|LLM coding models vs. diffusion for creative work>
- <https://x.com/trq212/status/2089529798850969805|/design command in Claude Code>

*Josh Woodward* (VP, Google Labs / Gemini / Google AI Studio) shared a detailed progress update on Gemini improvements: revamped Workspace tools shipping in 1-2 weeks, better tool-calling in Gemini 3.7 Flash, a new Projects design in implementation, 49 connectors and counting, plus a series of items now fully done and ramping.
- <https://x.com/joshwoodward/status/2089520767281324112|Gemini progress update>

*Nikunj Kothari* (partner at FPV Ventures) dropped a sharply funny — and pointed — observation: every layer of AI (models, IDEs, harnesses, app builders, inference, voice, data labeling, infra, neoclouds, generative media) gets described as having "no moat"... except the venture firm. He also argued seriously that brand marketing — not product or distribution — will be the defining differentiator of the AI era, especially as agents become the primary user of most software.
- <https://x.com/nikunj/status/2089486802356961364|"Nobody in AI has a moat — except the VC">
- <https://x.com/nikunj/status/2089374392295842086|Brand marketing as the last moat>

*Guillermo Rauch* (CEO, Vercel) announced that Cursor Origin now lets you host repos and deploy to Vercel — and Cursor Origin itself runs on Vercel. The jab at GitHub availability ("unlike GitHub, it's online 😁") landed with 3,600 likes.
- <https://x.com/rauchg/status/2089409162270965858|Cursor Origin + Vercel integration>

*Madhu Guru* (Sr. Director of AI, Meta; prev. led Gemini, Veo, Nano at Google) laid out a practical framework for getting good at evals: start with a workflow you know deeply, make its quality measurable, study real traces to understand what good looks like at each step, capture failure cases (messy tool calls, missing context), and build toward automated, continuously-updated eval suites that track real user patterns over time. A grounded, experience-backed thread from someone who's shipped models at scale.
- <https://x.com/realmadhuguru/status/2089480958571331623|How to get good at evals>

*Aaron Levie* (CEO, Box) argued that in an AI world, data is literally a balance sheet asset — not just a metaphor. As AI's appetite for data grows, how companies manage and mine their organizational intelligence will become a core competitive factor. A data sale in the news prompted him to make the case that most companies still dramatically undervalue their own information.
- <https://x.com/levie/status/2089499887905997272|Data as a balance sheet asset>

*Garry Tan* (President & CEO, YCombinator) shared his open-source "Personal AGI" project — a private GitHub repo with 70 proven Claude Code / Codex skills and the beginnings of a Karpathy-style personal knowledge wiki. MIT-licensed and free, it works with existing Claude Code or Codex subscriptions.
- <https://x.com/garrytan/status/2089438298540519821|Personal AGI open source project>
- <https://x.com/garrytan/status/2089425134339961173|What's included: 70 skills + knowledge wiki>

*Amjad Masad* (CEO, Replit) noted that scanning code for vulnerabilities isn't enough — you have to actively try to break it with pen testing. He also highlighted a lean, AI-native team achieving AI-growth-rate results without ever putting "AI" in their pitch.
- <https://x.com/amasad/status/2089435606338416884|Pen testing matters, not just scanning>
- <https://x.com/amasad/status/2089525819567739264|AI-pilled team, no "AI" in the pitch>

*Swyx* (affiliated with smol_ai, Cognition, AI Engineer, Latent Space) praised Trajectory for their work on continual learning — specifically highlighting a talk on why GRPO isn't sufficient and the team's journey to fully on-policy training, with all the problems that entails. His take: "tasteful execution on ambitious goals."
- <https://x.com/swyx/status/2089393073327653344|Trajectory's continual learning approach>

*Peter Yang* (AI newsletter, 110k+ subscribers) is looking for AI tools to handle YouTube talking-head editing — zoom ins, animated captions, logos, b-roll — and wants to drive the full edit via Codex or a harness. Mentions HyperFrames as a current test but soliciting alternatives.
- <https://x.com/petergyang/status/2089519732336787619|AI tools for YouTube editing via Codex>


*PODCASTS*

*No Priors — "Chasing Trillion-Dollar Companies, Founder Ambition, Token Budgets, and Regulatory Capture"*

*The Takeaway:* The next wave of trillion-dollar companies is probably further away and rarer than the hype suggests — and great founders going small out of fear of the labs is one of the quiet crises of this AI moment.

Investor Elad Gil (early Google, HiQ, former exec at Twitter and others) and Sarah Guo (Conviction VC) cover a lot of ground: from how many multi-trillion-dollar companies can realistically emerge in the next five years (Elad's answer: very few, maybe one), to why the best founders are increasingly chasing niche markets out of fear of labs rather than taking them on directly.

Elad's sharpest point: AI is running on a compressed timeline where "every year of AI time is like three to four years of normal cycle time." That compression means the standard startup exit calculus needs to be revisited every six months, not every few years. He frames it in terms of opportunity cost — specifically the cost of your best productive years, not just dilution math.

On token budgets and compute allocation: as models get better, labs are increasingly concentrating resources on the few dozen researchers driving 80% of results. The question of "return on invested tokens" — which people and projects deserve outsized compute — is the next management challenge coming to enterprises and labs alike.

The "18 months to AGI/RSI" belief comes up critically. Sarah points out that many brilliant researchers have held that belief for five consecutive years, so the predictive track record is poor. What she finds genuinely concerning is the psychological effect on researchers who act as if their contribution is irrelevant — a framing she calls "kind of tragic."

They close on regulatory capture: drawing parallels to pharma and nuclear energy (France generates 70% of power from nuclear; the US 18%, with no new reactors in 40 years), they argue that over-regulating AI carries real costs that rarely get counted in safety debates.

<https://www.youtube.com/watch?v=6l8oAO_LBx4|Watch on YouTube>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
