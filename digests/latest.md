AI Builders Digest — November 15, 2026

*X / TWITTER*

*Peter Yang* (petergyang on X) — AI tutorials and interviews creator
Peter Yang shared a practical tool for a devastating situation: a /fuck-cancer skill for Claude and ChatGPT that lets anyone upload a loved one's medical records, create a one-page brief, and research clinical trials. He also weighed in on the WSJ's reporting on Alice Huang, sharing a Singapore government statement that casts doubt on whether she's actually a spy — calling the reporting questionable and urging people to do their own research.
- https://x.com/petergyang/status/2121430386685395022
- https://x.com/petergyang/status/2121430819667579031

*Amjad Masad* (amasad on X) — Replit CEO
Amjad Masad is rallying behind Jensen Huang: he signed the #StandWithJensen letter and personally worked with the page owner to raise rate limits on the Replit-hosted petition site so it could scale to the surge in traffic. He also highlighted Replit's expanding partnership with Visa on agentic commerce, with more features coming.
- https://x.com/amasad/status/2121377395244749097
- https://x.com/amasad/status/2121389001546567837
- https://x.com/amasad/status/2121428406764204199

*Guillermo Rauch* (rauchg on X) — Vercel CEO
Vercel CEO Guillermo Rauch called Workflow SDK 5 and Vercel Workflows a "monumental step forward for agents" — highlighting dramatically faster step execution, improved encryption and security, battle-tested reliability at scale, and a new open-source `durable-harness` library that makes the underlying durability log reusable for any agent harness. He also teased Vercel Sandbox and co-signed the Stand with Jensen letter.
- https://x.com/rauchg/status/2121277727940776114
- https://x.com/rauchg/status/2121347136965210286
- https://x.com/rauchg/status/2121351007615811799

*Garry Tan* (garrytan on X) — YCombinator President & CEO
YCombinator's Garry Tan ran a real benchmark on 52 coding tasks in Claude Code and found Opus 5.5 is the better deal: Fable 5.2 solved roughly the same percentage of tasks (82.7% vs 84.6%) but costs 2.80x more per solved task. His recommendation: keep Opus 5.5 as your coding default. He shared his open-source harness eval repo. He also signed the #StandWithJensen letter, calling for due process.
- https://x.com/garrytan/status/2121464508225053153
- https://x.com/garrytan/status/2121463161069228382
- https://x.com/garrytan/status/2121462697787342932

*Matt Turck* (mattturck on X) — VC at FirstMark Capital
One dry observation: VCs were about to opine on the FAA nationwide airport ground stop.
- https://x.com/mattturck/status/2121358328169132503

*Nikunj Kothari* (nikunj on X) — Partner at FPV Ventures
Nikunj Kothari noted the FAA ground stop was only the third in modern history — after 9/11 and the 2023 NOTAM outage. He also pushed back on AI benchmark-maxxing, arguing the field should know better by now: the only benchmarks that matter are the ones that reflect your actual workflow, and the rest is marketing posturing that won't last.
- https://x.com/nikunj/status/2121366466905981435
- https://x.com/nikunj/status/2121320899161010360

*Dan Shipper* (danshipper on X) — Every CEO
Dan Shipper shared two thought-provoking posts: a piece on why teams still pay for software even when Fable 5.2 can "vibe code anything," and a musing on what he calls "the most important formula in AI." He also flagged something he described as an increasingly common problem in AI that's "extremely important to get fixed."
- https://x.com/danshipper/status/2121248233510818003
- https://x.com/danshipper/status/2121243400293007866
- https://x.com/danshipper/status/2121367890095960507

*Aditya Agarwal* (adityaag on X) — General Partner at SPC, Co-Founder of Bevel Health
Aditya Agarwal highlighted seven SPC portfolio companies named to the AI 100: Baseten, Render, Profound, Replit, Gamma, Cog, and Density.
- https://x.com/adityaag/status/2121281677238604148


*PODCASTS*

*Training Data — A Model For Everyone: How Ronak From Trajectory Is Building Products For Continual Learning*

_The Takeaway:_ Continual learning — AI models that improve continuously from real-world use, the way humans do — is the missing layer between today's powerful but static foundation models and tomorrow's AI that actually gets better on the job.

Ronak (Founder & CEO of Trajectory) makes the case that most companies are stuck renting intelligence from closed-source frontier models instead of owning it. Trajectory's platform changes that: AI-native companies bring their production traces and define what "good" looks like, and get a one-click training interface that handles the rest. The results are concrete — Harvey used it to train a model that's 6x cheaper than the frontier and jumped from 4% to 18% accuracy on a legal benchmark. Rogo used it to train a model that handles finance tasks at a fraction of the token cost.

The technical unlock worth understanding: today's dominant training algorithm (gRPO) requires replaying the same task up to 16 times in a simulation to learn from it. Trajectory has pushed toward "group size one" — learning from a single real-world trajectory — which eliminates the need for a replay environment entirely and dramatically lowers the infrastructure bar. They're also working on reducing the labeling burden: rather than hand-labeling all 10,000 traces, they smartly select 100 representative ones, have users label those densely, and train a meta-grader that propagates reward across the full set.

The philosophical bet: continual learning, not recursive self-improvement (RSI), is the safer path to increasingly capable agents. RSI is a black box that improves itself without humans in the loop. Continual learning improves from actual interaction with humans — keeping alignment baked in by design.

> "I want this paradigm to propagate, where the unit of work that we think about is a trajectory... the tasks of economic value that are happening."

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
