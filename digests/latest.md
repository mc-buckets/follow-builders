AI Builders Digest — August 22, 2026

*X / TWITTER*

*Swyx* (AI builder, affiliated with smol.ai, Cognition, AI Engineer Foundation)
Had a genuine shift of conviction around simulation as an AI scaling law. Midway through a podcast interview he went "from somewhat shitposting to very very serious" about Simile — the team behind the original Smallville social simulation paper, backed by Karpathy and Fei-Fei Li. His take: if recursive self-improvement is real, the last barrier before full automation of ML research is simulating humans and human feedback. Simile is already finding PMF at Fortune 100 companies at an early stage. "I've never been so happy to be so wrong." He's also running a second "Kill My SaaS" project and will share results from the first one next week.
- <https://x.com/swyx/status/2090948945753076141|Simulation as a scaling law thread>
- <https://x.com/swyx/status/2090908959590740033|Kill My SaaS 2>

*Thibault Sottiaux* (Codex & ChatGPT product at OpenAI)
Two updates for Codex subscribers: the banked reset landed for all paid ChatGPT Work and Codex users — a long-requested feature. Separately, Sottiaux flagged that cache hit rates have been worse this week for some users, causing usage limits to drain faster than normal. Investigation is ongoing with a promised update.
- <https://x.com/thsottiaux/status/2090964822422949999|Banked reset confirmed>
- <https://x.com/thsottiaux/status/2091033630147854385|Cache hit rate issue update>

*Peter Yang* (AI tutorials and interviews creator)
Two takes on Instinct, a new AI assistant. The good: smooth onboarding for connecting iMessages, Google Workspace, and MCPs; proactively suggests actions right after connecting a tool. The bad: single-thread UX limits it for real work (he's staying on ChatGPT Work and Codex). The concerning: Instinct indexes and retains emails without explicit permission and doesn't let users delete their data — he flagged this publicly and says he can't recommend the product until it's resolved.
- <https://x.com/petergyang/status/2090814910720835633|Instinct review>
- <https://x.com/petergyang/status/2090936583814025417|Privacy flag on email indexing>

*Madhu Guru* (Sr. Director of AI at Meta; formerly led Gemini, Veo, and Nano at Google)
Part 5 of his "How to build great evals" series: resist the pressure to collapse your eval suite into one number. He calls it "the tyranny of the average" — a model that improves on easy tasks while degrading on your hardest use case looks fine in aggregate. A weighted score doesn't fix this; it just adds false precision around a judgment call. His advice: keep a prioritized eval ladder, find stakeholders who engage with complexity, and understand all critical results in depth before making a model decision.
- <https://x.com/realmadhuguru/status/2090930137885774324|Evals thread part 5>

*Thariq* (Claude Code engineer at Anthropic)
Sharing an internal skill that's caught on at Anthropic: `/eli5`. Run `/eli5 <topic>` and Claude explains it "like I'm someone who knows nothing about this topic, using an HTML artifact with big pictures and few words." Now installable via the plugin marketplace:

`claude plugin marketplace add anthropics/claude-plugins-community`
`claude plugin install eli5@claude-community`

Example uses: `/eli5 how does this module work`, `/eli5 why did we make this tradeoff`, `/eli5 what caused this incident`
- <https://x.com/trq212/status/2090884854590382515|ELI5 skill announcement>
- <https://x.com/trq212/status/2090884855798407576|Install instructions>
- <https://x.com/trq212/status/2090890394880155888|Example use cases>

*Guillermo Rauch* (Vercel CEO)
v0, Vercel's AI frontend builder, now accepts Grok and Codex subscriptions — testable instantly in a sandbox. Rauch also shared that the team ran the `is-agentic` benchmark in a loop against their own product until it hit 100/100, using the process to close real capability gaps. "We worked hard to make sure the criteria is high quality and worth your time & tokens."
- <https://x.com/rauchg/status/2090953806624489501|v0 supports Grok & Codex subs>
- <https://x.com/rauchg/status/2090858571613470919|is-agentic 100/100>

*Aaron Levie* (Box CEO)
"The rate of progress in AI right now is unlike any other period in tech history." As intelligence becomes too cheap to meter, Levie argues the real opportunity shifts to driving AI diffusion across the broader economy. He frames this as a structural tailwind for applied AI startups — not just foundation model builders — and calls it a huge moment for companies that can take advantage.
- <https://x.com/levie/status/2091038566260539574|On AI diffusion and startups>

*Nikunj Kothari* (Partner at FPV Ventures)
Built a practical home automation tool using Claude Code: his daughter's school posts daily meals on a poorly structured website. He had Claude Code trace network requests to find an unauthenticated API, format the data, and pipe it into their existing home bot ("Hermes"). Now every morning the bot announces what's for breakfast and lunch so the family can pack food accordingly. A clean example of Claude Code as a personal engineering tool.
- <https://x.com/nikunj/status/2090884422178627624|School lunch tracker built with Claude Code>

*Peter Steinberger* (OpenClaw / OpenAI)
Spoke at the Agentic AI Summit in Berkeley on "No Doors for Agents" and teased a new Claude Code skill he's dropping. Limited detail yet on the skill's content.
- <https://x.com/steipete/status/2090898421108605078|Agentic AI Summit talk>
- <https://x.com/steipete/status/2090946181564440727|New skill teaser>

*Claude AI* (Anthropic's official account)
Anthropic launched Claude Security, powered by a new model called Mythos 5. Point it at a GitHub repo and it scans for vulnerabilities by tracing data flow across files and reasoning about how components interact. Each finding includes a CWE category, confidence rating, severity, and a suggested fix. Fixes surface directly in Claude Code on the web, billed as standard token usage under your existing plan. Alongside: a $35M Defender Advantage Fund in credits for open-source security projects, and an expanding Cyber Verification Program for the coming weeks.
- <https://x.com/claudeai/status/2090852316328902930|Mythos 5 security scanning>
- <https://x.com/claudeai/status/2090852318527033804|Fixes open in Claude Code>
- <https://x.com/claudeai/status/2090852320128938319|Defender Advantage Fund & Cyber Verification>

*PODCASTS*

*No Priors — "What Chess.com Teaches US About Superhuman Capabilities, with CEO Erik Allebest"*

_The Takeaway:_ Machines becoming superhuman at a game doesn't kill human interest in it — if anything, it deepens engagement. Chess.com is the thirty-year proof.

Erik Allebest bought the chess.com domain out of a bankruptcy auction in 2005 for $56,000 after every investor told him it was uninvestable. Two decades later: 250 million registered members, 10 million daily active users, over $200M in annual revenue — and zero external capital raised until private equity came in later to buy secondary shares, not inject growth funding.

The most counterintuitive thread: AI made chess more exciting, not obsolete. Early chess engines made the game briefly boring as grandmasters tried to imitate perfect computer play. Then neural nets arrived and started beating those engines with aggressive, unconventional moves nobody had seen before — and chess became richer than ever. Allebest draws the obvious parallel to what's happening now across knowledge work.

On what chess.com's dataset reveals about human learning: "It's just repetition of the small building blocks... there are no shortcuts to the process." Younger players are reaching elite performance faster than any previous generation — but it still requires reps, not just information access.

He also walked through launching Gambit (gambit.com), their poker product applying the chess playbook: ratings over chip counts. The bet is that players will care about their poker rating more than money. "Losing $100 at a table, it's not my favorite thing, but I don't care that much. But honestly, losing 100 rating points on poker — that just really bothers me."

On AGI: more optimistic than pessimistic, but worried that "too much money is flowing into the hands of too few." His framing: it's a cultural problem, not a technological one.

https://www.youtube.com/@NoPriorsPodcast

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
