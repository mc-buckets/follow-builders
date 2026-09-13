AI Builders Digest — September 13, 2026

*X / TWITTER*

*Thibault Sottiaux* (Codex & ChatGPT at OpenAI)

It was a massive product week at OpenAI — Sottiaux listed five Astra-powered launches: Images 2.5, GPT-Live-1, the Agents API, Data Agent, and ChatGPT for Financial Services, with more still to come before DevDay. <https://x.com/thsottiaux/status/2098639827084480864|tweet>

He also posted a detailed rollback/fix notice for Astra users, identifying three root causes behind recently-reported quality issues: overly-aggressive skill triggers from old model configs, an opt-in context management experiment that caused early stops or replies to stale messages (disabled; ~4–5k users affected), and misconfigured engines degrading a long tail of traffic. All three are now fixed, and a model reset landed by midnight. <https://x.com/thsottiaux/status/2098612714704891959|tweet>

OpenAI also acquired the Git AI team (Aidan and Sasha), who built an open-source tool that helps developers understand how coding agents contribute to their codebase. The tool will stay open source and be integrated into Codex. <https://x.com/thsottiaux/status/2098569976143806918|tweet>

*Peter Yang* (AI educator and content creator)

Yang is skeptical of the "software factory" framing. He argues AI can't self-improve a product or build features end-to-end without a human in the loop — one wrong assumption overnight ruins the whole run. He's asking for concrete examples of features built end-to-end with no human defining requirements or checking work. <https://x.com/petergyang/status/2098565668241334366|tweet>

On tooling, he's making a clean split: all local scheduled tasks go to Codex, all cloud tasks porting over to Grok Bot. <https://x.com/petergyang/status/2098614492066435228|tweet>

*Madhu Guru* (Sr. Director of AI at Meta; previously led Gemini, Veo, and Nano at Google)

Guru laid out why most enterprise AI efforts fail: leaders reuse old playbooks (the trusted lieutenant + central platform team model), under-invest in evals, and build AI for the business from the outside rather than embedding builders inside the functions they're trying to transform. His prescription: hire leaders who have shipped AI products, make evals a first-class citizen, and embed your best AI builders directly inside finance, sales, and support. <https://x.com/realmadhuguru/status/2098448235048378456|tweet>

*Thariq* (Claude Code at Anthropic)

Anthropic's Claude Code team shipped plugin evals — a way to test whether your skills still work correctly after new model releases. Run `claude plugin eval init` in your plugin folder to get started. <https://x.com/trq212/status/2098531560643539440|tweet>

Separately, Thariq pushed back on benchmark culture: pass/fail eval scores are increasingly hard to interpret because many failures stem from overly strict hidden tests, and in some cases the model's answer is actually better than the expected eval result. <https://x.com/trq212/status/2098490139798655427|tweet>

*Amjad Masad* (CEO at Replit)

Replit announced it acquired a business that was itself entirely built on Replit — Masad calls it the first of many. <https://x.com/amasad/status/2098548464452055437|tweet>

Also shipping: Routines with budgets — giving scheduled agents spending limits. <https://x.com/amasad/status/2098317466682179643|tweet>

*Guillermo Rauch* (CEO at Vercel)

Tailscale's model router runs on Vercel AI Gateway as its underlying infrastructure. Rauch's take: "AI Gateways are the new CDNs. You could go direct to origin, but it's brittle. You could DIY, but it's painful and costly." <https://x.com/rauchg/status/2098531157230969062|tweet>

*Aaron Levie* (CEO at Box)

Box can now be mounted to agent sandboxes, letting AI agents read and write files directly — no human proxy needed. Levie frames this as a key enterprise primitive: "As AI agents execute critical workflows in the enterprise, they're going to need the same primitives that people have had." <https://x.com/levie/status/2098478938003841123|tweet>

*Ryo Lu* (Designer at Cursor; previously Notion, Stripe)

Cursor shipped long-lived agents for big ideas, and Lu (who just moved to Taipei) flagged it. <https://x.com/ryolu_/status/2098324260867772806|tweet>

*Zara Zhang* (Builder, Harvard '17)

Zhang thinks the "one-person company" idea is overrated. AI dramatically amplifies individual leverage, but building something new is profoundly lonely — you need co-founders to brainstorm with, suffer with, and celebrate with. "It is extremely easy to lose motivation when you don't tie yourself to the mast together with somebody else." <https://x.com/zarazhangrui/status/2098483800456179923|tweet>

*Peter Steinberger* (OpenClaw + OpenAI)

Steinberger demoed Astra running in a cloud session playing Doom via CUA (Computer Use Agent) — "not quite AGI yet, but probably beats fly brain." Also submitted a patch to the @trycua framework to fix key handling on Linux. <https://x.com/steipete/status/2098527519213604889|tweet>

*Dan Shipper* (CEO at Every)

Every is moving beyond vibe checks on new models. Shipper's team built an internal platform for all staff to create personal benchmarks based on their real day-to-day work — starting to get quantitative alongside the qualitative. <https://x.com/danshipper/status/2098481799047647715|tweet>


*PODCASTS*

*No Priors — "Coinbase's Everything Exchange: Agentic Finance, Stablecoins, and Tokenization with CEO Brian Armstrong"*

_The Takeaway:_ Crypto rails aren't just for humans — they may be the essential financial infrastructure for the AI agent economy, and Coinbase is betting its future on that.

Brian Armstrong, Coinbase co-founder and CEO, makes a case that most people haven't fully internalized: AI agents are going to need bank accounts. Seventy-six percent of agentic e-commerce transactions are under $0.30 — far too small for credit card rails that start at a flat $0.30 fee. Stablecoin micropayments aren't a nice-to-have; for an agent economy to function, they're structurally necessary. "We don't want the AIs to be unbanked." Coinbase has released a simple tool — a single-prompt paste — that lets any AI agent spin up its own self-custodial financial account using crypto rails, no KYC required.

Beyond agent wallets, Armstrong walked through three big bets: the Everything Exchange (stocks, crypto, derivatives, prediction markets, all tokenized and cross-margined in one place — 88% of Coinbase revenue now comes from non-Bitcoin products), stablecoin payments growing even when Bitcoin is down, and Agentic Finance (AIFi), which includes an AI advisor in the Coinbase app and an X402 micropayment protocol now supported by Google, Cloudflare, and AWS.

Internally, Coinbase is pursuing recursive self-improvement: every time an agent touches a service, it ingests that service's "brain" — a structured memory of incidents, AB tests, financial controls, and PR history. When a human corrects an agent's output, that correction feeds back into the brain, so future agents start with richer context. Armstrong says one-shotted PR acceptance rates have been rising as a result. Their internal agent harness, called Toshi, can now orchestrate parallel agent swarms — he described spinning up 10 agents in parallel to execute phase one of a complex feature plan, all completing within two minutes.

On his longevity company New Limit: the first phase 1 clinical trial (targeting alcoholic liver disease with epigenetic reprogramming) is launching next year. The underlying platform aims eventually to let healthy people restore the cellular function they had in their 20s — liver, vasculature, immune system, potentially brain.

<https://www.youtube.com/watch?v=uLDK4l_-gUE>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
