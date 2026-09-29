AI Builders Digest — September 29, 2026

*X / TWITTER*

*Thibault Sottiaux* — Codex & ChatGPT at OpenAI

The concept of a code freeze before releases is becoming obsolete. Sottiaux argues that in the near future, code itself might be generated dynamically per request according to constraints — making traditional release-gating practices increasingly irrelevant.

- <https://x.com/thsottiaux/status/2104108167806550046|View tweet>

*Guillermo Rauch* — Vercel CEO

Rauch ported his Mini web browser from Electron to Rust & Swift using Claude Opus 5.5, and says the result is faster, more secure, and easier to iterate on. He used the `cef` Rust crate to bundle Chromium, embedded an agent via the `fx acp` protocol talking to a local CLI over ACP, and gained Liquid Glass, faster boot times, and Mac-native behavior. His broader thesis: "Native is the future, both on the desktop and in the cloud. I suspect the entire software world will 'nativify' faster than people realize."

- <https://x.com/rauchg/status/2104428800134013205|View tweet>

*Aaron Levie* — Box CEO

Levie sketched a framework for how agents will reshape markets. Some sectors benefit from friction (switching costs create moats) — agents will erode those advantages and spike competition. But many markets suffer from friction — healthcare, travel, local services — and agents will unlock entirely new economic activity there. "A future meaningfully mediated by agents that work tirelessly for us and our goals can't possibly function exactly the same as today."

- <https://x.com/levie/status/2104350592290406849|View tweet>

*Garry Tan* — President & CEO at Y Combinator

Tan is bullish on AI agents navigating the web, pushing back on the anti-bot status quo. He called anti-bot measures "for losers" and noted that CDP-based automation hits a wall against real anti-bot systems. His pro-builder/pro-AI stance extends to SF civic politics: "Do not nerf. Made in San Francisco."

- <https://x.com/garrytan/status/2104402742517420517|Anti-bot tweet>
- <https://x.com/garrytan/status/2104231083701420282|Do not nerf>

*Matt Turck* — VC at FirstMark Capital

A pointed observation: AI researchers — the people who actually understand how the technology works — tend to hold nuanced views, believing in neither doom nor runaway acceleration. Non-researchers, by contrast, hold the most certain and extreme opinions. Worth sitting with.

- <https://x.com/mattturck/status/2104331402385002831|View tweet>

*Thariq* — Claude Code at Anthropic

A sobering productivity concern: "I am most afraid of us eating the productivity gains of agents by just becoming lazier." The worry isn't that agents won't work — it's that humans will adjust their baseline expectations downward rather than doing more with the freed capacity.

- <https://x.com/trq212/status/2104273243599405395|View tweet>

*Amjad Masad* — CEO at Replit

Replit is showing up in unexpected places. Masad shared that Replit is gaining traction in the Chan-Zuckerberg household, a small signal that developer tools built for accessibility are crossing into the broader culture.

- <https://x.com/amasad/status/2104428789417857436|View tweet>

*Peter Yang* — AI tutorials creator

A cultural observation on software staying power: nobody has fond memories of the SaaS tools they used at work, but everyone remembers their favorite games. Games win the long-term memory test. LLM models, Yang suggests, might be the inverse — highly memorable and personal in a way business software never was.

- <https://x.com/petergyang/status/2104414495376564517|View tweet>

*Zara Zhang* — Builder

Two sharp takes. On posting without monetization: "Self-expression is an innate human instinct that requires no justification or utilitarian motive. Influence is so much more valuable than money." On tech hype: "New technology can be so dazzling and flashy that it blinds us to the ways in which it's not working — and sometimes makes you feel that if something is not working, it's probably your fault."

- <https://x.com/zarazhangrui/status/2104253882025341231|On posting>
- <https://x.com/zarazhangrui/status/2104112917264126195|On tech hype>

*Nikunj Kothari* — Partner at FPV Ventures

Kothari is impressed with Google's Astra: "Give it decently hard verifiable end to end tasks with the right tools and watch it just fly." He's watching closely as multi-modal, tool-using agents move from demos into real workflows.

- <https://x.com/nikunj/status/2104444216017637575|View tweet>

*Peter Steinberger* — OpenClaw + OpenAI

Steinberger is rethinking CI from the ground up. His plan: let Codex decide which tests actually need to run based on the change, "drastically nix CI," and move to hourly test runs instead. Using AI to triage the test suite rather than running everything on every commit.

- <https://x.com/steipete/status/2104305554760114488|View tweet>

*Dan Shipper* — CEO at Every

A single sharp line that landed: "industry built on modeling humans as rational agents panics as humans adopt rational agents." Behavioral economics meets the AI moment.

- <https://x.com/danshipper/status/2104302924251951553|View tweet>


*PODCASTS*

*Training Data: Box's Aaron Levie — On Reinventing Yourself in the AI Age and Enterprise Diffusion*

*The Takeaway:* The bridge between AI models and real enterprise workflows is where the next trillion dollars of software value will be created — and it won't be built by the model labs.

Aaron Levie has been running Box for nearly two decades, sitting on hundreds of billions of enterprise files for some of the largest companies in the world. That vantage point gives him an unusually grounded read on where AI actually lands versus where the hype says it should.

His central argument: everyone in the AI world is "research pilled" — obsessed with model intelligence as the only thing that matters. But when you go into a real bank, hospital, or law firm, you hit five to ten blocking problems that have nothing to do with intelligence: legacy data systems, human-in-the-loop requirements, change management, idle agents waiting on approvals, decades of unmodernized process. "The model could be the most intelligent, super intelligence in the world, but that workflow still requires you to connect up to other data systems."

Levie's historical comparison is clarifying: "If you were to go back ten years ago and look at what AWS was building, I guarantee you would not have predicted Snowflake or Databricks existing. You would have been like, the infrastructure just already does that. The same thing is going to be true for intelligence."

On the strategic tension between model labs and the application layer, he's direct: the fox-guarding-the-henhouse problem means enterprises don't want the token seller deciding which model runs their most critical workflows. He expects token subsidization to end when the big labs go public and face real gross margin pressure.

He's also candid about "work slop" — AI-generated content that reads like a Claude prompt. His take is that we're in a transitional moment where content is still a proxy for the person's judgment, and when AI writes it, that signal breaks down. "I'm reading it once for the substance, and I'm also reading it for the calculation of: did the person write it, or am I just literally reading a Claude prompt?" He doesn't think this lasts — pointing to financial models as the precedent: nobody cares if a spreadsheet formula wrote your numbers, but they still want to discuss the analysis.

Box is now deploying agents against that unstructured data at scale — contract extraction, document Q&A, workflow automation — and running evals across every major model. His current read on the frontier: Fable 5.1 is the best he's seen, Gemini overperforms on certain enterprise document tasks, and "it's a total race right now."

<https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8|Watch on YouTube>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
