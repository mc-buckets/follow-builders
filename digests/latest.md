AI Builders Digest — May 10, 2026

*X / TWITTER*

*Sam Altman* (CEO, OpenAI)

Sam Altman declared his preference for AI that helps developers "pokemon-evolve into superheroes" rather than replace them — noting that what one really good engineer can do with AI now is "insane." He also teased that OpenAI wants to help companies secure themselves, signaling urgency to act quickly. A separate observation worth watching: young people prefer interacting with AI via voice, older people prefer typing — he wonders if that will change.
- https://x.com/sama/status/2052558319940944256
- https://x.com/sama/status/2052485051812909530
- https://x.com/sama/status/2052462428663992564


*Alex Albert* (Research, Anthropic)

Alex Albert flagged a striking result: with help from Claude Mythos Preview, the Firefox team fixed more security bugs in April than in the previous 15 months combined. He also pulled a quote from a related blog post on the topic.
- https://x.com/alexalbert__/status/2052468573516513762
- https://x.com/alexalbert__/status/2052468575492088078


*Aaron Levie* (CEO, Box)

Box CEO Aaron Levie offered a sharp competitive take on the AI era: if AI makes any task equally easy for everyone, competitive advantage shifts elsewhere — specifically to sales, marketing, and customer success. "If you automate getting financial advice and insights, then the differentiation is in client engagement." His challenge to builders: if everyone does exactly what you're doing with AI, how will you stand out?
- https://x.com/levie/status/2052566788236509254


*Garry Tan* (CEO, Y Combinator)

YC CEO Garry Tan shipped GStack v1.28, his personal Claude Code setup for agentic workflows. New: GStack Browser can download items and run in headed configuration mode with anti-bot detection via Xvfb on headless Linux containers. He also added thin-client mode to GBrain, so Claude Code or secondary agents (like Hermes) can connect over MCP without spinning up their own server. An llms.txt was added so agents can use all skills with less guesswork.
- https://x.com/garrytan/status/2052588548126364028
- https://x.com/garrytan/status/2052629679572701455
- https://x.com/garrytan/status/2052588782076281324


*Dan Shipper* (CEO, Every)

Every CEO Dan Shipper is sounding the alarm: "the AI platform war is coming." He and Kieran Klaassen recorded a quick dispatch analyzing the xAI compute deal, managed agents, and why Anthropic is repositioning its API as full cloud infrastructure for developers.
- https://x.com/danshipper/status/2052501376195080381


*Madhu Guru* (Former Product Lead, Google Gemini)

Madhu Guru announced he's leaving Google after building the Gemini product from scratch. His retrospective is candid: three years ago OpenAI and Anthropic were clearly ahead. The Gemini team built the playbook, the customer feedback flywheel, and the enterprise business to compete — and he credits Gemini 3 as the moment those systems came together. He signs off with a nod to the real intelligence now demanding his attention: his toddler, "quietly shipping."
- https://x.com/realmadhuguru/status/2052490869320946037


*Claude* (Anthropic)

Claude for Microsoft Office is now generally available on all paid plans. Excel, PowerPoint, and Word are live; Outlook is in public beta. As Claude moves between apps, it carries the full context of the conversation.
- https://x.com/claudeai/status/2052445786651168849
- https://x.com/claudeai/status/2052445787930468704


*Amjad Masad* (CEO, Replit)

Replit CEO Amjad Masad noted that what's being called "the most viral petition in history" is hosted on Replit — a pointed flex about platform scale (and a disclaimer: Replit has no opinion on Mbappe).
- https://x.com/amasad/status/2052478595277467703


*Peter Steinberger* (OpenClaw + OpenAI)

Peter Steinberger is deep in multi-agent territory: his OpenClaw agents are now delegating cron jobs to each other. He's also enthusiastic about GPT 5.5 combined with the /goal command for planning large refactors with end-to-end tests. On the side, he mentored students in the ChatGPT Future Class of 2026, including a team that built Wi-Find — a system that detects disaster survivors through walls and debris using AI.
- https://x.com/steipete/status/2052630190346457301
- https://x.com/steipete/status/2052514752245481675
- https://x.com/steipete/status/2052486085226184742


*Ryo Lu* (Design, Cursor)

Cursor designer Ryo Lu shared a demo of the full software development loop — from idea to merged PR — all inside Cursor.
- https://x.com/ryolu_/status/2052496872586272802


*Nikunj Kothari* (Partner, FPV Ventures)

FPV partner Nikunj Kothari made a contrarian case against weekly 1:1s, calling them "a psy-op by mid-tier empire-building managers" who want to micromanage rather than trust their reports to excel. His urge: find a team that pushes your limits and shows what high performance actually demands.
- https://x.com/nikunj/status/2052626010332668278


*Swyx* (AI.engineer / Cognition / Temporal)

Swyx warned followers about a phishing attempt that nearly fooled him, urging caution.
- https://x.com/swyx/status/2052599553283813788


*Aditya Agarwal* (General Partner, South Park Commons)

South Park Commons GP Aditya Agarwal is hosting an Embodied AI Hackathon in SF, May 15–17. Applications close May 12th.
- https://x.com/adityaag/status/2052441427070861816
- https://x.com/adityaag/status/2052441425724514741


*PODCASTS*

*The MAD Podcast with Matt Turck*
_OpenAI Board Member Zico Kolter on the Real Risks of Frontier AI_

*The Takeaway:* Safety doesn't scale automatically with AI capabilities — waiting for a bigger model won't make it safer, and that's not just a warning, it's a research finding.

Zico Kolter chairs the Safety and Security Committee (SSC) at OpenAI's board while running the machine learning department at Carnegie Mellon. He's one of the rare people who actually does AI safety governance at the frontier lab level, not just writes about it.

The SSC functions like a corporate audit committee — it reviews every major model release, meets with safety and alignment teams, gets third-party evaluations, and has real authority to delay a release. But what Kolter makes clear is that the committee's power is limited if the underlying safety work isn't being done in training.

His sharpest point: across nearly every capability domain — math, coding, legal reasoning — the dominant strategy is to wait for the next model. It will be better. But that strategy fails completely for robustness. "So far, we have not seen that same thing happen when it comes to things like the robustness of models. You can't just sort of trust models to get safer by getting bigger." Safety requires explicit investment: monitors, substructures, usage tracking, and system-level filters layered on top of the model itself.

He ran the largest AI red-teaming competition ever — 1.8 million attack attempts through his startup GraceOne — and the results confirmed it: robustness doesn't come for free with scale. Meanwhile, the attack surface is growing fast as agentic systems gain real-world access and autonomy.

On jailbreaks and prompt injection: Kolter puts them at the "simpler mistakes" end of a four-category AI risk spectrum — the model being fooled because it doesn't fully understand context. Real, but addressable, and not where his deepest concern lies.

The most surprising moment: the full mathematical framework of an AI system fits in roughly 200–300 lines of Python. "The entire complexity of an AI system evolves from the data they're trained on." The actual engineering challenge — and the real complexity — is in the data pipelines and getting 10,000 GPUs to work efficiently together.

https://www.youtube.com/watch?v=DvyZcCfepeI


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
