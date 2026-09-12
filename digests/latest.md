AI Builders Digest — September 12, 2026

*X / TWITTER*

*Boris Cherny* — Claude Code at Anthropic

Boris Cherny shared two high-signal posts. First, he flagged Anthropic's latest Threat Intelligence report as "absolutely terrifying and important": as models grow more capable, dual-use risks scale with them — a model that codes well can hack critical infrastructure; one that assists biology research can engineer pandemics. He called these issues "complex, thorny, and increasingly important for everyone to understand."
<https://x.com/bcherny/status/2098281805770309686|Threat Intelligence report post>

He also wrote a detailed response to a common question about AI code quality, distinguishing throw-away code (black box is fine if the blast radius is low) from production code (should meet a higher bar than human-written code). At Anthropic, guardrails include lint rules, Claude-driven end-to-end tests, Claude-powered daily fuzzers, and automated code and security reviews. His advice for when Claude's output doesn't meet the bar: use the latest frontier model (Opus 5 or Fable 5.1), increase effort to high or xhigh, invest in your CLAUDE.md, or steer more actively. "Your job is to hold the bar on code quality."
<https://x.com/bcherny/status/2098217573276131577|Code quality response>
<https://x.com/bcherny/status/2098217571153838124|Original question thread>

*Thibault Sottiaux* — Codex & ChatGPT at OpenAI

OpenAI has paused new subscriptions to their $200/month "Astra" Pro plan due to overwhelming demand — existing accounts are unaffected and all other plans and the API remain available. The company said it's "the smallest step that allows us to continue giving the broadest access possible" while adding capacity.
<https://x.com/thsottiaux/status/2098113585683808624|Astra subscription pause>

He also revealed the infrastructure under ChatGPT Work: "scaled agents on demand," now available as an API so developers can get started in under a minute.
<https://x.com/thsottiaux/status/2098238138334548260|Scaled agents on demand API>

And promoted the internal OpenAI dashboard tool — the way everyone at OpenAI makes dashboards and learns about the business.
<https://x.com/thsottiaux/status/2098165551554240764|Internal dashboard tool>

*Josh Woodward* — VP at Google Labs, Gemini App, Google AI Studio

Gemini is now available on Windows.
<https://x.com/joshwoodward/status/2098131750660772342|Gemini on Windows announcement>

*Peter Yang* — Practical AI content creator

One concise take on the Astra vs. Sol debate: "In my humble opinion, for getting shit done Sol > Astra."
<https://x.com/petergyang/status/2098215935467544604|Sol vs Astra>

*Nan Yu* — Incoming product staff at OpenAI, formerly head of product at Linear

Nan posted a sharp reminder about AI's growth ceiling: normies use Google, Instagram, Zillow, and DoorDash all day — yet barely touch AI. "Still. Early." Separately, offered a euphemism for a down-round acquisition: "Don't call it a private equity acquisition for a huge discount from peak valuation. Call it an Italian goodbye."
<https://x.com/thenanyu/status/2098216215525331353|Still early>
<https://x.com/thenanyu/status/2098094411465048497|Italian goodbye>

*Madhu Guru* — Sr. Director of AI at Meta (previously led Gemini, Veo, Nano Banana at Google)

Part 10 of his series on building great evals: measure the steps, not just the result. Two agent trajectories might both produce the correct answer, but one makes 4 clean tool calls while the other makes 17 redundant ones, searches the same thing 3 times, and recovers from 2 errors. The better process is obvious — and your evals should reflect it. Practical advice: define your whole workflow, define tasks per step, measure each step separately, define median and hard tasks, and study steps before final results.
<https://x.com/realmadhuguru/status/2098064969464217720|Evals tip #10>

*Thariq* — Claude Code at Anthropic (prev YC W20, MIT Media Lab)

Shared a useful prompt for giving Claude deep personal context through an in-depth interview saved to memory: "Interview me in depth using free text, or askuserquestion tool when multiple choice works, about relevant parts of my life you don't know about yet and save it all to memory."
<https://x.com/trq212/status/2098157600361861579|Claude memory interview prompt>

*Google Labs* — Google's home for latest AI tools and experiments

Dreambeans, Google's AI-powered daily story generator, is now free for all US users 18+ on iOS and Android — no subscription required. New: connect it to Gemini for even more personalized stories that build on the nuance from your chats.
<https://x.com/GoogleLabs/status/2098110018289803558|Dreambeans launch>

*Amjad Masad* — CEO of Replit

Pushed back firmly on AI extinction narratives: "Lots of risk with AI. I worry a lot about cybersecurity for example. However, 'extinction risk' — literally 100% of humans die — is not remotely one of them." Also promoted Replit's new AI chat experiences including conversations with various personalities.
<https://x.com/amasad/status/2098171265924116732|AI extinction risk take>
<https://x.com/amasad/status/2098171773413929322|ETN bros chat>
<https://x.com/amasad/status/2098171501505581559|PG in London chat>

*Guillermo Rauch* — CEO of Vercel

Major infrastructure milestone: Vercel's CDN global metadata store is now 91% faster at p99 — handling ~10 million daily deployments (2.35 billion total to date) under growing pressure from agentic workloads. The improvement covers the build→deploy pipeline end to end. He also teased an upcoming product direction: "A computer for every agent, in every region."
<https://x.com/rauchg/status/2098091056302833837|CDN 91% faster at p99>
<https://x.com/rauchg/status/2098158541932794222|Computer for every agent>
<https://x.com/rauchg/status/2098066258155708851|Deployments faster again>

*Aaron Levie* — CEO of Box

Posted a detailed enterprise AI field report after meeting with dozens of technology leaders across banking, media, insurance, and consulting. Top trends:

- *Cyber anxiety*: Everyone is nervous about growing AI-driven vulnerabilities, especially following the OpenAI/Hugging Face incident. Conversation is pragmatic, not existential.
- *Multi-model reality*: Most enterprises deploy multiple frontier models. Standardizing on one is too hard; open weights still in infancy at enterprise scale.
- *Agent identity & security*: New challenge — agents need controlled identities to access systems, but sometimes need to act exactly as the user.
- *Process reengineering = real ROI*: Companies that restructure workflows around agents get far more value than those who just layer agents onto existing flows.
- *Rapid vendor switching*: Innovation is moving so fast that no one waits for a vendor to fix something — they just move on.
- *Evals still early*: Very few companies have a good grasp of how to measure AI performance against their actual workflows.

He also announced Box is partnering more deeply with OpenAI for secure access to enterprise Box content from within ChatGPT.
<https://x.com/levie/status/2098218284139311615|Enterprise AI field report>
<https://x.com/levie/status/2098135659714085281|Box x OpenAI partnership>

*Matt Turck* — VC at FirstMark Capital, MAD Podcast host

Promoted his new episode with Richard Socher on recursive self-improvement and scientific progress. (See Podcasts section below.)
<https://x.com/mattturck/status/2098081448330674182|Podcast episode breakdown>
<https://x.com/mattturck/status/2098081452839637480|Listen on Spotify/Apple/YouTube>

*Zara Zhang* — Builder

One blunt frustration: "Why is computer use still so painfully slow??"
<https://x.com/zarazhangrui/status/2098136119154254287|Computer use frustration>

*Nikunj Kothari* — Partner at FPV Ventures

Shared a wry venture capital reality check: "Three truths in early stage venture right now: 1) everyone wants to raise a $50 million seed, 2) everyone thinks they will hit $30 million ARR next year, 3) every hot tranched seed round magically ends up at the ~$300 million valuation." Also shared a behind-the-scenes look at a fast-turnaround post: voice memo while driving → more voice memos throughout the day → 30 minutes of furious writing → quick read-through and publish.
<https://x.com/nikunj/status/2098078391065018816|Venture truths>
<https://x.com/nikunj/status/2098255116751257663|Fast publishing behind the scenes>

*Peter Steinberger* — OpenClaw and OpenAI

Highlighted a widely-resonant observation about AI-era coding: "Duplicating logic is no longer painful. Abstractions still are." (2,293 likes.) Also noted that Astra demand is growing fast — flagging the capacity crunch before the subscription pause announcement.
<https://x.com/steipete/status/2098089196800098798|Duplicating logic vs abstractions>
<https://x.com/steipete/status/2098088917782413740|Astra demand growing>

*Dan Shipper* — CEO of Every

Reacted to OpenAI pausing Astra Pro subscriptions with "I'm so sorry" and expressed excitement about an upcoming capability he's eager to experiment with.
<https://x.com/danshipper/status/2098120649701204416|Reaction to Astra pause>
<https://x.com/danshipper/status/2098116268671025210|Excited to experiment>

*Aditya Agarwal* — General Partner at SPC, ex-CTO of Dropbox

Posed a high-stakes framing for AI investment: "If you had a machine capable of doing only 1 thing: Finding cures to our most pressing diseases. How much of your GDP would you devote to this machine? I think the answer is: very high. This is the world we live in now."
<https://x.com/adityaag/status/2098112281267843264|GDP for disease-curing machine>

*Claude* (claudeai by Anthropic)

Fable 5.1 Build Days kick off this week — the Claude community is hosting buildathons in cities worldwide from September 11–25. Bring a problem, an idea, or just show up.
<https://x.com/claudeai/status/2098138736642933143|Fable 5.1 Build Days>

*PODCASTS*

*The MAD Podcast with Matt Turck — "When AI Improves Itself | Richard Socher (Recursive)"*

_The Takeaway:_ Anything that can be simulated, AI will solve — and recursive self-improvement means we're entering a loop where AI making better AI will unlock scientific discovery at a pace no human institution can match.

Richard Socher, one of the most cited AI researchers in history, just raised $650M for Recursive, a company explicitly built to create AI that improves AI. His new book _The Eureka Machine_ argues that scientific progress has slowed not from lack of talent or funding, but from fragmentation: knowledge has become a "labyrinth" of 34,000 specialized journals with "no trespassing signs." No one can be the Renaissance generalist anymore — a biology PhD studying proteins may know nothing about the tissue or cell levels of the same field.

His solution is not just faster AI — it's a four-pillar "Eureka Machine": (1) LLMs that ingest the world's knowledge, (2) models trained on scientific measurements humans can't perceive directly (gravitational waves, gamma rays), (3) simulation environments where AI can experiment endlessly, and (4) robotic lab automation to collect real-world data and verify hypotheses. On top sits an agent swarm that explores ideas the way evolution does — in parallel, with open-ended recombination.

One genuinely counterintuitive claim: hallucination is sometimes a _feature_, not a bug. "How reasonable or just outside of the distribution in some interesting way are your predictions?" is exactly what you want to ask when generating novel proteins. Temperature-dialing a model is conceptually similar to how psychedelic states have historically produced scientific leaps — Socher points out that history's great scientists sometimes made breakthroughs in altered states.

He pushed back hard on "hard takeoff" narratives: biology will still take time because clinical trials require real-world data you can't simulate away. But the structural economics of drug discovery are already changing — companies now enter late-stage trials with 8+ drug candidates in 18 months instead of 1 candidate after 8 years.

At Recursive, $410M of the $650M raise is committed to compute (Amazon). His view: compute is civilization's resource allocation question. "Before you know it, you're in this recursive self improvement loop and we believe that that will be a great unlock."

"Boy, are we far away from the true upper bounds of any of the spaces of intelligence. And there is still so much further that AI can go."

https://www.youtube.com/@DataDrivenNYC/videos

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
