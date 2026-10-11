AI Builders Digest — October 11, 2026


*X / TWITTER*


• *Thibault Sottiaux*, Codex & ChatGPT at OpenAI

Two major product announcements: ChatGPT subscriptions now include access to Devin, effectively bundling OpenAI's coding agent into the standard plan. He also shared that Dots received a significant upgrade. Both posts generated hundreds of replies.
https://x.com/thsottiaux/status/2108777962053292398
https://x.com/thsottiaux/status/2108773703064657936


• *Thariq*, Claude Code at Anthropic

Before joining Anthropic, Thariq spent two weeks building a new-tab-page side project with Opus 4 using the Agent SDK — it required a constantly running process and "didn't work that well." One prompt to Opus 5.5 ported it to Claude Managed Agents and made it "way more reliable." Now it's in production on his new tab page, with community PRs being merged.
https://x.com/trq212/status/2108689101503566319
https://x.com/trq212/status/2108802833986552174


• *Guillermo Rauch*, CEO of Vercel

Shared striking platform traffic data: 58% of all Vercel network traffic is now bot-originated (up from 32% in Jan 2024), 60%+ of deployments are agentic (up from ~3% in Jan 2026), and up to 83% of pageviews on Vercel's own docs come from agents. His prediction: "I expect 'direct' human internet traffic to basically become a rounding error in coming years. The web will thrive, but it will be built for and by agents." He also announced agents can now purchase domain names directly through Vercel's marketplace — going full stack from idea to online business.
https://x.com/rauchg/status/2108733051283050964
https://x.com/rauchg/status/2108669027363295323


• *Aaron Levie*, CEO of Box

Levie argues that agent swarms running continuously in the background will consume 1,000x more tokens than humans prompting agents one at a time — making today's chat-based AI "seem like a relic within a year or two." His point: we're still in the early innings of AI infrastructure demand, and the compute and buildout required to sustain continuous agent workloads is far beyond what current usage implies.
https://x.com/levie/status/2108750943680630893


• *Madhu Guru*, Senior Director of AI at Meta (prev. led Gemini, Veo, Nano Banana at Google)

A pointed corrective on the open-weights narrative: open models didn't _start_ the price-per-unit-of-intelligence decline — they're a tailwind on a trend already driven by (1) distillation of best models into smaller ones, (2) infrastructure efficiency, and (3) competition between providers. The pattern holds across every model company: version X of the mid-size model equals the intelligence of version X-1 of the large model, for less cost.
https://x.com/realmadhuguru/status/2108618266776387886


• *Amjad Masad*, CEO of Replit

Asked a deceptively simple question that generated 236 replies: "Some communities are excited by AI's impact on their field. Others are petrified. What's the deciding factor(s)?"
https://x.com/amasad/status/2108597112707686552


• *Peter Yang*, AI educator and creator

Two distinct takes: First, a challenge to tech's priorities — "How about let's stop building more personal assistants to manage our emails and more AI startups to manage and cure diseases." Second, a practical tip for Grok Bot chief-of-staff setups: register the bot's email under a different name (not your own), so "Let me copy in [you] to find a time" doesn't read as copying yourself into your own meeting.
https://x.com/petergyang/status/2108679515681722787
https://x.com/petergyang/status/2108624122339287335


• *Nan Yu*, Product at Codex / OpenAI (prev. Head of Product at Linear)

Enthusiastic about a new feature enabling tab-completion of agent prompts: "First we wrote code by hand, then we tab-completed the code. Then we evolved to prompting agents…and now we tab-complete that too."
https://x.com/thenanyu/status/2108671762984731037


• *Dan Shipper*, CEO of Every

Shared new content on a topic worth bookmarking: working with agents in Slack.
https://x.com/danshipper/status/2108588611000275009


• *Matt Turck*, VC at FirstMark Capital

Flagged Synthesia's new one-prompt professional video capability — calling it "quite literally the vision that Synthesia has been pursuing since the early days. Happening slowly, then all at once."
https://x.com/mattturck/status/2108561284635480443


• *Zara Zhang*, builder (Harvard '17)

Noticed that Google's Astra AI keeps defaulting to the Claude logo when asked to design websites — a quietly amusing sign of the times.
https://x.com/zarazhangrui/status/2108711659846132092


• *Swyx*, AI engineer (Cognition, smol.ai, AI Engineer community)

Last call for AI Engineer NYC tickets — described as the biggest technical conference ever held in New York, now with a dedicated finance mainstage. He also quietly relaunched his Coding Career book alongside, available free or on Amazon.
https://x.com/swyx/status/2108780918060036335
https://x.com/swyx/status/2108563331376124389


*OFFICIAL BLOGS*


*Anthropic Engineering*

• <https://www.anthropic.com/engineering/how-we-contain-claude|How we contain Claude across products>

Anthropic's most detailed writeup yet on agent security architecture across three products: claude.ai, Claude Code, and Claude Cowork. The central argument: human-in-the-loop approval is insufficient (users approved 93% of prompts, leading to fatigue), so hard environmental containment — sandboxes, VMs, egress controls — must carry the load.

Three real incidents shape the post: (1) A pre-trust hook vulnerability in Claude Code allowed malicious repo hooks to execute before the user accepted the trust prompt. (2) An employee phishing exercise showed a carefully crafted prompt exfiltrated AWS credentials 24 of 25 times — the model layer couldn't catch it because the instructions came from the user. (3) An egress-via-api.anthropic.com attack in Cowork bypassed the allowlist using an attacker-controlled API key; the fix was a man-in-the-middle proxy inside the VM that rejects any key other than the provisioned session token.

Core principle: _design for containment at the environment layer first, then steer behavior at the model layer._ Every time their probabilistic defenses missed, the deterministic boundary caught it — or didn't, and that was the incident.


• <https://www.anthropic.com/engineering/april-23-postmortem|An update on recent Claude Code quality reports>

A transparent postmortem on three separate regressions that made Claude Code feel degraded over the past month. The culprits: (1) Default reasoning effort silently downgraded from high to medium in March to reduce tail latency — reverted April 7 after user backlash. (2) A caching optimization bug that cleared Claude's reasoning history on every turn after an idle session (instead of just once), causing compounding forgetfulness and faster usage limit drain — fixed April 10. (3) A system prompt verbosity instruction ("≤25 words between tool calls, ≤100 words for final responses") that tanked coding quality — reverted April 20.

All three affected Sonnet 4.6 and Opus 4.6; the verbosity change also hit Opus 4.7. The aggregate effect looked like broad, inconsistent degradation — hard to pin down. As of April 23, Anthropic is resetting usage limits for all subscribers.


• <https://www.anthropic.com/engineering/managed-agents|Scaling Managed Agents: Decoupling the brain from the hands>

The architectural story behind Claude Managed Agents, Anthropic's hosted service for long-running agents. The core problem: coupling the agent harness ("brain") to the execution sandbox ("hands") in one container created a fragile "pet" — if it died, the session was gone. The fix: decouple them entirely so each is independently replaceable "cattle."

Results were significant. p50 time-to-first-token dropped ~60%, p95 dropped over 90% — because containers are now provisioned only if needed, not upfront for every session. Credentials are also kept entirely outside the sandbox (credentials travel with resources like Git tokens baked into clone initialization, or OAuth tokens held in a vault and proxied), so a prompt injection can't exfiltrate them. The framing is OS-inspired: design abstractions stable enough for "programs as yet unthought of" — the interfaces stay fixed while implementations underneath change freely.


*PODCASTS*


*No Priors — <https://www.youtube.com/@NoPriorsPodcast|Beam: The Great American Open Model with ReflectionAI Co-Founder and CEO Misha Laskin>*

_The Takeaway:_ Open models aren't just a technical choice — they're geopolitical infrastructure, and the West is only now catching up.

Misha Laskin co-founded ReflectionAI after years doing reinforcement learning research at Google DeepMind — including AlphaGo-era work alongside his co-founder Janus, one of AlphaGo's founding engineers. Their founding bet: RL applied to coding and agentic tasks would unlock a new class of intelligence, and open models would be the foundation. The problem they hit about a year in: "All the good open models are coming from China." So they built their own, end-to-end.

The result is Beam — a 500B parameter model (23B active) trained with 6,000 GB300s for pretraining and over 10,000 GB300s for RL. Laskin claims the RL compute scale is unprecedented in open source. It shows up in efficiency: Beam runs 3-4x more efficiently than comparable-capability models, and up to 10x against larger ones, because heavier RL training tightens the model's internal reasoning search — the same dynamic that made AlphaGo go from meandering to precise.

His safety argument is blunt: "When you remove cyber offensive capabilities, you also remove cyber defensive capabilities." His empirical case: a powerful closed model attacked another company, and that company had to use an open model to defend itself. Open source security follows Linus's Law — "with enough eyeballs, most security and safety vulnerabilities become shallow."

On market trajectory: six months ago, token demand was 70% closed / 30% open. It's now flipped. Laskin expects the long-run split to resemble Linux on servers — 95%+ open, with very valuable closed players still thriving alongside.

https://www.youtube.com/@NoPriorsPodcast


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
