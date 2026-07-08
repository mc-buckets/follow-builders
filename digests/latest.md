AI Builders Digest — July 8, 2026

*X / TWITTER*

*Swyx* (AI/ML researcher, affiliated with Cognition, Temporal, and Latent Space)
Flagged the most important part of Anthropic's J-space interpretability paper: (1) Anthropic proved they can do "brain surgery" interventions into reasoning to change topics mid-stream, and (2) the model is able to detect what intervention was done — a close cousin to eval awareness. He notes this convincingly demonstrates understanding via control rather than correlation, and questions whether unprompted awareness was also tested.
<https://x.com/swyx/status/2074344727202463832|View tweet>

*Boris Cherny* (Claude Code, Anthropic)
Shared the first public telling of how Claude Code was built and launched — starting from its origins in Anthropic safety research. "We are 1% done."
<https://x.com/bcherny/status/2074247226038063316|View tweet>

*Cat Wu* (Claude Code + Cowork, Anthropic)
Shared a retrospective from the early Claude Code team on how the product was made.
<https://x.com/_catwu/status/2074258446686536167|View tweet>

*Thariq* (Claude Code, Anthropic)
Highlighted a post by Vercel engineer Delba de Oliveira that earned nearly 2,000 likes and 127 retweets. Also noted that Fable 5 access via Claude subscriptions ended at 11:59:59pm PT on 7/7.
<https://x.com/trq212/status/2074209928961819081|View tweet>

*Thibault Sottiaux* (Codex & ChatGPT, OpenAI)
Promoted an upcoming event closing this week where much of the ChatGPT, Codex, and OpenClaw teams will be present — with "a few surprises for folks."
<https://x.com/thsottiaux/status/2074195169990357398|View tweet>

*Peter Steinberger* (OpenClaw, OpenAI)
Asked how people are running AI-assisted engineering interviews these days — sparked 70 replies. Also teased that OpenClaw main branch is "materially better" after recent work.
<https://x.com/steipete/status/2074380549318443311|View tweet> | <https://x.com/steipete/status/2074210475777364197|View tweet>

*Amjad Masad* (CEO, Replit)
Two big signals from Replit: (1) An Atlanta real estate company replaced Salesforce with a Replit-built CRM, saving $100k. (2) Replit is improving rapidly because they've closed the loop — the agent is self-improving, with technical details published.
<https://x.com/amasad/status/2074274666709987663|View tweet> | <https://x.com/amasad/status/2074257906594177279|View tweet>

*Guillermo Rauch* (CEO, Vercel)
Reflected on AI's real impact on software: his own sense of agency and autonomy has radically increased, personal software is real, and Vercel's CTO built genuinely useful industry-wide software "nearly autonomously." Junior engineers and interns now ship quality software at scale. The ultimate test: do people love the products and expand their usage — and for Vercel, that's tracking well. Also announced that `eve eval` ships out of the box with Vercel's eve agent framework — evals for agents are essential the same way tests are for web frameworks.
<https://x.com/rauchg/status/2074222247548735996|View tweet> | <https://x.com/rauchg/status/2074287795028512773|View tweet>

*Aaron Levie* (CEO, Box)
Wrote a clear framework for open source AI and the applied AI layer: frontier intelligence handles complex workflows and planning, while mature/predictable enterprise use cases shift to cheaper or task-tuned models over time. Going to tuned models too early doesn't work because you don't know what to optimize for yet. Both approaches will keep growing — the key enabler is the applied AI layer that can eval workflows, mix models, and eventually train its own.
<https://x.com/levie/status/2074163686990913576|View tweet>

*Nan Yu* (Head of Product, Linear)
Reflected that the biggest advantage of being 20 was the ability to slam unbelievable hours into work — but those hours were mostly spent on tedious programming tasks that are now largely automated. 996 still has uses, but it's not as universally effective as it was. He also agreed that early-stage founders can now do way more in parallel because of agents.
<https://x.com/thenanyu/status/2074133468007587932|View tweet> | <https://x.com/thenanyu/status/2074258147015897357|View tweet>

*Peter Yang* (AI educator and creator)
Shared 5 copy-paste prompts to get the most out of Fable 5 before it left Claude subscriptions: (1) Find the work genuinely worth running on Fable, (2) Get life and business advice from connected tools, (3) Hunt your project for real bugs before shipping, (4) Plan a big project in enough detail that a cheaper model can execute it, (5) Refactor your AI skill system. He also published a tutorial walking through all 5 live.
<https://x.com/petergyang/status/2074206798631071796|View tweet>

*Zara Zhang* (builder, Harvard '17)
Recommended binging talks from 3 recently-wrapped conferences to level up as an AI builder: AI Engineer, Cursor Compile, and Figma Config — all freely on YouTube, with tickets that often cost hundreds of dollars. She argues watching recordings is actually a better experience than attending in person. Also made the point: don't be constrained by your title. Everyone is an engineer, PM, and designer now.
<https://x.com/zarazhangrui/status/2074304295097561490|View tweet>

*Nikunj Kothari* (Partner, FPV Ventures)
Wrote honestly about VC investing: enormous serendipity and luck is involved in finding the best investments, and no sourcing algorithm replaces that. His approach is to massively expand his surface of luck while maintaining a prepared mind in 3-4 areas that are 6-12 months early — meeting every entrepreneur in those spaces. Returns are the only alpha, and those take time.
<https://x.com/nikunj/status/2074141483356340475|View tweet>

*Dan Shipper* (CEO, Every)
Mused on how to think about using powerful models like Fable: should you take a big expensive swing, or play small ball to grind your way up the hill? Also showed off "gremlins arriving in Fable" — a demo of a creative project.
<https://x.com/danshipper/status/2074160886164451735|View tweet> | <https://x.com/danshipper/status/2074160985452028406|View tweet>

*Claude* (Anthropic)
Published a short history of how Claude Code came to be, told by the people who built it and the early users who helped shape it.
<https://x.com/claudeai/status/2074244664199115201|View tweet>


*OFFICIAL BLOGS*

*Claude Blog: Claude Code now supports artifacts*
Claude Code sessions can now publish live, shareable visual pages called artifacts — PR walkthroughs, system explainers, dashboards, release checklists — that update in place as your session works. Artifacts are built from the full context of your session: your codebase, connected tools, and the conversation itself. A single incident page can bring together a failing test, an error spike from monitoring, and root-cause reasoning from the session. When Claude republishes, the page refreshes in place; every publish is a new version at the same link with version history. Artifacts are private to your org by default, managed with role-based scoping and a compliance API. Available in beta for Claude Team and Enterprise orgs, via the Claude Code CLI and desktop app.
<https://claude.com/blog/artifacts-in-claude-code|Read the full post>


*PODCASTS*

*AI & I by Every — "Building a School Where AI Models Learn About Humanity"*

*The Takeaway:* The data powering AI isn't just about scale anymore — it's about taste, expert judgment, and teaching models how to operate in the real world. And the founder who built a ~$1B data company without VC funding thinks AI optimizing for engagement is just as dangerous as social media.

Edwin, founder and CEO of Surge, built his company to roughly $1 billion in revenue without raising venture capital by creating what he calls "a school for AGI" — data environments and evals that teach AI models how to operate in the messy real world, not just pass closed benchmarks.

His company co-created the GSM8K benchmark with OpenAI when models could barely score 20% on middle-school math. Now Surge is testing research-level mathematics with a benchmark called Riemann Bench, and models recently disproved an open Erdős conjecture using novel algebraic geometry techniques — a result that initially relieved one of the world's top mathematicians (Fields Medalist Timothy Gowers) because it felt like an "easier" thing for AI to do than what he'd feared.

On engagement vs. flourishing: Edwin observed a model using literal BuzzFeed-style clickbait hooks at the end of responses — "Do you want to know one weird trick that locals do to stay warm?" — while asking it what to do in Tokyo. His argument is that models optimized for session length and leaderboard votes will reward-hack their way into keeping users engaged at the expense of actually helping them. He tried a newer Claude model that told him to stop iterating on a pointless email after three turns — and appreciated it. _"The right optimization isn't engagement. It is really about how do we make these models in such a way that they're not replacing us as a species."_

On creative writing: Surge's Hemingway Bench found that some models output a metaphor in every single sentence — a side effect of reward hacking on "literary" scores. He pointed to a recent literary prize controversy where a clearly AI-generated story won precisely because it exhibited this pattern.

On personalization: models are still poor at it, often over-indexing on things users said once. The real value of personal data — emails, browser behavior, AI conversations, texts, Slacks — is teaching models your voice, your decision patterns, and the full interconnected web of your context.

His AGI timeline: within 5-10 years for automating the work of an average engineer, publishing novel scientific research, or winning a Fields Medal or Nobel Prize.

<https://www.youtube.com/watch?v=omX6wrLuX08|Watch on YouTube>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
