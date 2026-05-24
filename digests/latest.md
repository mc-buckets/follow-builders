AI Builders Digest — May 24, 2026

*X / TWITTER*

*Swyx* — Builder and writer, affiliated with Cognition, Temporal, and the AI Engineer community

Swyx co-signed a mental framework arguing that transformers are fundamentally limited learners, and that brute-force scaling will eventually be outclassed: "throwing more params, more power, more everything at a demonstrably inefficient paradigm will be outclassed by the simple solution that can hypothesize and seek truth rather than backfit a house of cards — although the bitter lesson is it is simpler to scale and we may hit AGI anyway because human intelligence just isn't that smart nor plentiful." <https://x.com/swyx/status/2058073815301972368|tweet>

He also introduced "Kakuna" — a subagent-parallelism-focused coding tool with strong opinions on AI engineering app design. The key concept: a "mullet factory" — "party in front (ship unique lovable features), dark in the back (timeless production principles)." Essentially the antientropy/antislop component of a larger agentic system. <https://x.com/swyx/status/2057876022553690327|tweet>


*Kevin Weil* — Former CPO and Head of Science at OpenAI, now board member at Cisco and The Nature Conservancy

Brief but pointed: Weil shared something a friend sent him with just the note "Make no little plans." A fitting sentiment for the current AI moment. <https://x.com/kevinweil/status/2057987544663364045|tweet>


*Peter Yang* — Product at Roblox, AI newsletter for 140K+ readers

Yang is building an interview series on how the best solo founders and engineers use agents to 10x their output — covering AI stacks, end-to-end build workflows, and multi-agent coordination, with an episode featuring Ryan dropping Sunday. <https://x.com/petergyang/status/2057989910125310459|tweet>

He also published a practical thread for employees navigating layoffs: six concrete steps — learn Codex or Claude Code, build side projects, develop a public GitHub history, and become top 10% at one craft. His contrarian take: "entrepreneurship is the safest job in the AI era." <https://x.com/petergyang/status/2057830781352034322|tweet>


*Google Labs* — Google's home for latest AI tools and experiments

Google Labs refreshed their website post-I/O, making it easier to explore their full portfolio and test new experiments from recent announcements. <https://x.com/GoogleLabs/status/2057884277384360416|tweet>

The team also shared picks for the most underrated or surprising features across their products. <https://x.com/GoogleLabs/status/2057863565328134604|tweet>


*Aaron Levie* — CEO at Box

Levie had a sharp take on AI and cybersecurity in response to a Mythos update: AI is making it far easier to both create and find security issues, which shifts the bottleneck to human review and response. "Far from AI magically solving all of this, there still is major triage work and human judgment required to do the follow on work to actually protect systems." His call: we're entering a security engineer boom — Jevons paradox all over again. <https://x.com/levie/status/2058006473620463985|tweet>


*Garry Tan* — President and CEO at Y Combinator

Tan shipped GBrain v0.40.0, adding a voice agent powered by Gemini Live to his open-source personal AI stack. "Mars is a friend, Venus is your EA." MIT-licensed and available now. <https://x.com/garrytan/status/2058053659527913566|tweet> <https://x.com/garrytan/status/2058053854026191170|tweet>

He also wrote a sharp analysis of Geoffrey Moore's chasm theory — arguing it breaks down entirely in "bar is zero" markets where customers have no viable alternative. "Buyers start acting like visionaries instead of skeptics, because they have to buy." His advice for founders in such markets: stop worrying about whole product and crossing the chasm, and ship the 60% solution. They're begging for it. <https://x.com/garrytan/status/2058043367704195271|tweet>


*Matt Turck* — VC at FirstMark Capital, host of the MAD Podcast

Turck highlighted that despite wild public-facing AI progress, behind the scenes at OpenAI it's "continuous progress compounding" — the internal pace is even faster than what's visible externally. <https://x.com/mattturck/status/2057913362608972256|tweet>


*Nikunj Kothari* — Partner at FPV Ventures

Kothari announced leading a Series A for a company he's excited about — notably, not an AI company. Also reshared a timely sentiment: "This time is too important to NOT be doing your life's best work." <https://x.com/nikunj/status/2057947701762019751|tweet> <https://x.com/nikunj/status/2057819563258216957|tweet>


*Peter Steinberger* — Builder at OpenClaw and OpenAI

Steinberger noted that GitHub is now natively shipping a 10-PR-per-person limit — something his team previously had to enforce manually with bots. A small but meaningful signal of how AI-assisted contribution patterns are reshaping platform tooling. <https://x.com/steipete/status/2057946259709628781|tweet>


*Dan Shipper* — CEO at Every

Shipper teased an upcoming talk on his piece "After Automation," exploring what work and creativity look like on the other side of the automation wave. <https://x.com/danshipper/status/2057885219936473195|tweet>


*Claude* — AI assistant by Anthropic

Anthropic's Claude account spotlighted Kay Zhu, co-founder and CTO of Genspark AI — an all-in-one AI workspace built on Claude. His take in a market where anyone can build: the team is what makes the difference. Part of The Problem Solvers series featuring founders tackling hard problems with Claude. <https://x.com/claudeai/status/2057854403558653983|tweet> <https://x.com/claudeai/status/2057854405118922884|tweet>


*OFFICIAL BLOGS*

*Claude Blog — New in Claude Managed Agents: dreaming, outcomes, and multiagent orchestration*
<https://claude.com/blog/new-in-claude-managed-agents>

Anthropic launched three major additions to Claude Managed Agents:

- *Dreaming* (research preview): A scheduled background process that reviews past agent sessions, extracts patterns, and curates memory so agents self-improve over time. You control how much autonomy it has — automatic updates or human-reviewed. Harvey used it to bring task completion rates up ~6x in testing.

- *Outcomes*: Define a success rubric and a separate grader evaluates outputs against it in its own context window — independent from the agent's reasoning — then sends the agent back for another pass if needed. Improved task success by up to 10 points in testing, with +8.4% on docx and +10.1% on pptx generation.

- *Multiagent orchestration*: A lead agent breaks complex jobs into pieces and delegates each to a specialist with its own model, prompt, and tools. Netflix used this to analyze logs from hundreds of builds in parallel. Spiral by Every uses it to run parallel draft generation with Opus subagents, with each draft scored against editorial rubrics before returning to users. Full trace visibility is available in the Claude Console.


*PODCASTS*

*Unsupervised Learning — Ep 87: Gemini Co-Lead on World Models, RL's Next Domains & Continual Learning*

*The Takeaway:* The researcher co-leading Gemini thinks we've already hit something like "digital AGI" — but what's still missing is the ability for models to genuinely learn from experience.

Oriol Vinyals is co-lead of Gemini at Google DeepMind alongside Noam Shazir and Jeff Dean, and one of the most cited deep learning researchers of the past decade. This conversation happened the day after Google I/O.

His most counterintuitive admission: narrow RL training on math and coding generalizes far more broadly than he expected. "That is not something I quite predicted to work as well as it did." He now sees reasoning models handling completely unrelated tasks — like moving logistics and tax questions — with strikingly strong inference, seemingly transferred from coding and math training.

On world models: Vinyals draws a sharp line between the current impressive multimodal output (Omni generating and editing video from images) and the harder unsolved goal — extracting the laws of physics from video alone, without language labels. The "GPT moment" for pure visual understanding hasn't happened yet.

On memory: He describes a near-term paradigm shift around file-system-style episodic memory for agents — not per-user weight fine-tuning, but rich updatable knowledge bases. "I think that's probably paradigm shifting as well in a way, similar to how we saw reasoning, you know, a year and a half or so ago."

On AGI: "In some way, AGI is here. I don't think it is here in the way I want to see it, but it is fairly close." His personal remaining gap: models that can truly learn from experience, not just retrieve it.

https://www.youtube.com/watch?v=NQczevdpxq0

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
