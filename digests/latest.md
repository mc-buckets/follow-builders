*AI Builders Digest — June 11, 2026*

Today's digest is dominated by one story: the launch of Claude Fable 5, which shipped yesterday and generated some of the most enthusiastic reactions the builder community has seen from a model release.


*X / TWITTER*

*Andrej Karpathy* (AI researcher and deep learning practitioner)
Karpathy called Fable 5 a "major-version-bump-deserving step change forward" on par with Claude 4.5 in November — especially for long, difficult problem-solving sessions. His key observation: Jevons paradox is kicking in. As models get better at software, his own demand for software keeps growing. "Free your mind — you can ask for anything: explainers, visualizers, dashboards, bespoke single-use apps, giant research projects with custom HTML for the results." He also flagged that the safety triggers are configured a bit aggressively for launch but should be tunable over time.
<https://x.com/karpathy/status/2064409694761054332|Tweet>

*Boris Cherny* (Claude Code lead at Anthropic)
Cherny described Fable 5 as a bigger step up than Opus 4.5 — the model "stepped up from being a coding agent to a thought and design partner in building the product." His standout moment: asking Fable to debug something. "It is the first model I have used that was so methodical and precise, taking measurements and adding logs then verifying that it truly fixed the issue before declaring victory. There's nothing in Claude Code's prompting telling the model to do that, it's just part of its personality." He calls it "big model smell." He also shared a post on why self-verification loops matter — a critical pattern for letting models run longer without constant check-ins.
<https://x.com/bcherny/status/2064431111154053187|Fable 5 take> • <https://x.com/bcherny/status/2064426115255730578|Self-verification loops>

*Alex Albert* (Research at Anthropic)
Albert, who has been at Anthropic through every model launch, put Fable 5 in the same tier as Opus 3, Sonnet 3.5, and Opus 4.5 — the launches that actually changed how models get used. "With Fable, the model stopped feeling like a tool I direct and started feeling more like something I collaborate with." His four tips: (1) give it bigger, more ambitious tasks; (2) use xhigh/high effort as default; (3) rewrite your CLAUDE.mds — instructions written for prior models anchor Fable to stale patterns; (4) shift from providing tasks to providing objectives — describe what done looks like and let Fable find the path using /loop and /goal.
<https://x.com/alexalbert__/status/2064394410004304003|Launch reflection> • <https://x.com/alexalbert__/status/2064467657483829441|Tips for Fable>

*Aaron Levie* (CEO Box)
Three substantive takes. First: amplified a post arguing that the real moat for applied AI companies is the unglamorous translation work — "arranging a company's private reality so a model can act on it, handing the model the tools to act, working with the customer to change the reality of its workforce." The translation never ends, which is why domain-specialized engineering is hard to copy. Second: dismissed the AI-progress-is-slowing narrative — Fable's benchmark numbers settle that debate. Third: made the case for compute-normalized benchmarks, noting that models behave very differently across compute thresholds and today's comparisons are often apples-to-oranges.
<https://x.com/levie/status/2064569513023328268|Applied AI moats> • <https://x.com/levie/status/2064396746953023647|On AI progress> • <https://x.com/levie/status/2064379199629181139|Compute-normalized benchmarks>

*Guillermo Rauch* (CEO Vercel)
Announced that Vercel CLI now supports AI Gateway API keys with per-key spend budgets and quota refresh periods — "virtual credit cards for AI tokens." Also noted a compelling two-model workflow: Opus wrote a VM, Mythos verified it.
<https://x.com/rauchg/status/2064551967461114111|Vercel AI Gateway CLI> • <https://x.com/rauchg/status/2064419055726215438|Opus + Mythos workflow>

*Swyx* (AI engineer; affiliated with Cognition, Temporal, and the Latent Space Podcast)
Practical tip while Fable is not pay-per-use: tell Claude Code to "review my code for issues" on your whole codebase. Swyx says you'll be "in abject horror that you shipped anything to prod without a Fable Check™ first." Also clocked the shipping pace: 34 days between signing an NVIDIA compute deal and getting a Mythos-class model GA to the world — "building on the NVIDIA stack means you can just do things™."
<https://x.com/swyx/status/2064492823781789969|Fable code review tip> • <https://x.com/swyx/status/2064421542503797186|34-day shipping pace>

*Thariq* (Claude Code team at Anthropic)
Checking in from Code with Claude Tokyo. His message on Fable: "It's time to be more ambitious." Plans a series of posts on how the model has reshaped how the team works.
<https://x.com/trq212/status/2064437561930682672|Fable take> • <https://x.com/trq212/status/2064521202622960058|Tokyo event>

*Garry Tan* (President and CEO YCombinator)
Declared Fable 5 "the biggest model energy I've ever seen" — then immediately ran into usage limits while trying to use it on his GStack project.
<https://x.com/garrytan/status/2064573857911152710|Fable reaction> • <https://x.com/garrytan/status/2064559225859416186|Usage limits pain>

*Zara Zhang* (builder; 30K GitHub stars as a non-technical founder)
Sharp observation on why non-technical people struggle with coding agents: "The barrier for non-technical people using coding agents was never the interface. Chatting is the easiest UI ever invented. The barrier is that they don't know what to ask for. The blank chat box assumes you already know what's possible. Most people don't." She was impressed by an agent called Town that proactively suggested workflows rather than waiting for instructions. Also announced a free virtual talk this Friday on her vibe coding process — how she gets product ideas, works with coding agents, and designs things that aren't AI slop.
<https://x.com/zarazhangrui/status/2064587398529606082|Blank chat box problem> • <https://x.com/zarazhangrui/status/2064486120386379950|Friday talk RSVP>

*Nikunj Kothari* (Partner at FPV Ventures)
Used Fable to one-shot a full website about S-curves throughout history. Process: dumped a podcast transcript into Claude's research mode, had it identify all the historical S-curves and their inflection points, then generated a Claude Code prompt that built the whole site in one shot. Site is live at escurves.com.
<https://x.com/nikunj/status/2064506504888373758|S-curves demo> • <https://x.com/nikunj/status/2064508462034501997|How the prompt was built>

*Peter Yang* (AI educator, 150K+ newsletter readers)
Mixed Fable experience: browser use is slowing things down noticeably. Also pushed back publicly on Boris Cherny's "big model smell" phrase. On the fun side, shared the exact prompt he used to one-shot a fully functional F-Zero-style racing game — neon cyberpunk visuals, pseudo-3D track, 3 AI opponents, boost mechanics, and a sense of speed at 400-800 km/h.
<https://x.com/petergyang/status/2064577126385459265|Browser use slowdown> • <https://x.com/petergyang/status/2064550073594446059|F-Zero prompt>

*Dan Shipper* (CEO Every)
Enthusiastic about the Fable launch — Every has been testing for a week and published a vibe check.
<https://x.com/danshipper/status/2064395167658860859|Every's vibe check>

*Thibault Sottiaux* (Codex and ChatGPT at OpenAI)
Playfully claimed 1% royalty fees on the Fable launch. Also polling followers on how they use `codex /goal` — occasional use vs. primary workflow. Separately shared a demo framed as "playing codex like an orchestra. One /goal at a time."
<https://x.com/thsottiaux/status/2064572276180484475|Royalty joke> • <https://x.com/thsottiaux/status/2064308436133716008|/goal usage poll> • <https://x.com/thsottiaux/status/2064307859903447396|Codex orchestration>

*Amjad Masad* (CEO Replit)
Claude Mythos is now available on Replit at 25% off.
<https://x.com/amasad/status/2064411791015432466|Replit Mythos deal>

*Josh Woodward* (VP at Google Labs, Gemini App, and Google AI Studio)
One-liner on the Fable launch: "The demand for software is going to be off the charts."
<https://x.com/joshwoodward/status/2064509357216428171|Tweet>

*Claude* (Official Anthropic account)
The official rollout: Fable 5 is available everywhere. Mythos 5 — the same underlying model with safeguards lifted in specific areas — is currently restricted to Glasswing partners (cyber defenders and critical infrastructure providers), with plans to expand through a broader trusted access program for defensive cybersecurity and biomedical research.
<https://x.com/claudeai/status/2064394160522559632|Fable 5 announcement> • <https://x.com/claudeai/status/2064394158056386684|Mythos 5 details> • <https://x.com/claudeai/status/2064394159318782217|Trusted access expansion>


*PODCASTS*

*AI & I by Every — "We Automated Everything With AI and Tripled Our Headcount"*

_The Takeaway:_ Automation doesn't eliminate the need for human experts — it actually increases demand for them.

Dan Shipper, CEO of Every, makes a counterintuitive case. Despite building one of the most AI-native companies around — where, as he puts it, "if you swing a stick around in our Slack, you're as likely to hit a human as you are an agent" — Every has grown from 4 to 30 people since the GPT-3 days, and is still hiring.

His explanation: AI makes "yesterday's expert competence cheap," flooding every workplace with output that's close but not quite right. That flood creates new demand in two ways. First, experts are needed to build systems that transform the glut of okay work into something actually good. Second, experts can now build things that were simply impossible before — like an engineer who shipped an entire inbox product end-to-end in a month or two.

The deeper argument is structural. "The further away an agent gets from a human, the less valuable it is." Models are built to act on behalf of someone — they execute tasks brilliantly, but they don't have agency. They always look back for direction. That gap between "autonomous execution" and "genuine agency" is what keeps human judgment irreplaceable, even as benchmarks improve exponentially.

On the ClickUp-style mass layoffs done in the name of AI efficiency, Shipper is skeptical: when a company announces it's performing great while firing 20% of its workforce, he suggests the real story is often poor strategy or company decline, with AI as the convenient excuse.

His bottom line: "If you just ride the models — when new models come out, learn to use them for the stuff that you do — you're going to be fine."

<https://www.youtube.com/playlist?list=PLuMcoKK9mKgHtW_o9h5sGO2vXrffKHwJL|Watch on YouTube>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
