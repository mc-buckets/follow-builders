AI Builders Digest — May 16, 2026

*X / TWITTER*

*Peter Yang* — Roblox product manager and creator of Practical AI, a newsletter for 140K+ readers — wrote a pointed rant on the wave of tech layoffs. Over 80,000 tech employees were laid off in Q1, the highest since 2022–23. His argument: companies overhired during the zero-interest era and are now using AI as a convenient scapegoat. He breaks down 6 ways employees can take back control.
<https://x.com/petergyang/status/2054569893060809151|Read the thread>

*Garry Tan* — President & CEO of Y Combinator — posted on SF drug policy, calling out legacy media for platforming voices that "personally benefit from more fentanyl tourism." He advocates defunding nonprofits that enable drug use and redirecting that funding toward recovery and treatment on the West Coast.
<https://x.com/garrytan/status/2054778575988093249|See tweet>

*Nikunj Kothari* — seed/Series A partner at FPV Ventures — pushed back on the idea that broad VC rejection should deter a determined founder. Responding to a post suggesting VC has become purely consensus capital, he argues that founders who are truly obsessed treat each rejection as potential learning — not a verdict. The implicit warning: founders who need capital validation to believe in themselves may be in it for the wrong reasons.
<https://x.com/nikunj/status/2054599845214650442|See tweet>


*OFFICIAL BLOGS*

*Claude Blog*

*<https://claude.com/blog/new-in-claude-managed-agents|New in Claude Managed Agents: dreaming, outcomes, and multiagent orchestration>*

Anthropic launched three major additions to Claude Managed Agents.

_Dreaming_ (research preview) is a scheduled process that reviews past agent sessions, extracts patterns, and updates memory stores so agents self-improve over time. Developers can let it run automatically or require human review before changes land. Harvey, the legal AI company, saw ~6x completion rates on complex long-form drafting tasks after enabling dreaming.

_Outcomes_ lets developers write a success rubric; a separate grader evaluates agent output against that bar and the agent self-corrects until it passes — no human in the loop required. In benchmarks, outcomes improved task success by up to 10 points, with the largest gains on the hardest problems, and boosted file generation quality by +8.4% on docx and +10.1% on pptx.

_Multiagent orchestration_ lets a lead agent break complex jobs into pieces and delegate each to specialist subagents running in parallel on a shared filesystem. Every step is traceable in the Claude Console. Netflix is already using it to analyze logs across hundreds of builds simultaneously. Webhooks are now available too — define an outcome, let the agent run, and get notified when it's done.


*PODCASTS*

*Training Data — <https://www.youtube.com/watch?v=Jq3BIGz4vXQ|Suno's Mikey Shulman: Everyone Can Make Music Now>*

*The Takeaway:* Music isn't a scale problem — it's a taste problem — and building from that insight let Suno unlock something no benchmark could have predicted.

Mikey Schulman is the founder and CEO of Suno, the AI music platform that has reached $300M ARR and produced chart-topping hits. His path is improbable: quantum computing PhD at Harvard, then an early leadership role at Kensho (where he also met LangChain founder Harrison Chase), then accidental music company founder — he originally thought generative audio was orders of magnitude away from being viable.

The most counterintuitive technical choice: Suno deliberately avoided teaching the model anything about music theory. No 12-tone scale, no instrument taxonomy, nothing. They model everything as raw sound — 48,000 samples per second of continuous float values. "If you tell the model there are 12 tones, it will only ever produce those 12 tones. You will be forever limited." Building from scratch is how you eventually get trap with a sitar, country with 808s, or genres that don't have names yet.

The product bets were equally contrarian. When competitors were making 10-second crisp audio clips, Suno went all-in on full songs — even though the audio quality was noticeably worse — because a story matters more than production value. They also moved off Discord fast (90% of traffic migrated to their web app within five days of launch). On scale: unlike LLMs, throwing more compute at music models doesn't help much. "There are no right answers. There are no benchmarks." Preference data and novel research are what actually move the needle.

On the "slop" question: "I made two songs with my five year old yesterday. Is that slop? In the sense that 99.999% of the planet has no interest in hearing that? Sure. But that's really meaningful to me, and so if you call that slop — I'm not sure I care."

What's ahead: social co-creation (sharing song templates to riff on together), deeper personal voice integration (hearing your own voice in a song dramatically increases attachment), and music video generation (currently in beta). Suno also recently settled and partnered with Warner Music to build new interactive artist–fan experiences — a sign the company is moving from scrappy to structural.

<https://www.youtube.com/watch?v=Jq3BIGz4vXQ|Watch on YouTube>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
