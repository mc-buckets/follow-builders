*AI Builders Digest — July 1, 2026*


*X / TWITTER*

*Boris Cherny* (Claude Code at Anthropic)
Claude Code is getting a significant background-agent upgrade. In the next release, subagents will run in the background by default, letting you keep chatting with Claude while your agents work in parallel. You can still opt into foreground execution by telling Claude directly.
<https://x.com/bcherny/status/2071647677591466098|Background subagents announcement>

*Anthropic* (claudeai on X)
Claude is now generally available in Microsoft Foundry on Azure. Azure customers get Claude Opus 4.8 and Claude Haiku 4.5 with native Azure authentication, billing, and commitment retirement. Prompt caching and extended thinking are live today, with more capabilities coming. Inference is operated by Anthropic on Azure infrastructure.
<https://x.com/claudeai/status/2071653958905467027|Claude in Microsoft Foundry GA>
<https://x.com/claudeai/status/2071653962013446586|Inference details>

*Thibault Sottiaux* (Codex and ChatGPT at OpenAI)
Two major Codex updates in one day. First, an incident postmortem: Codex usage was draining faster than expected due to several compounding bugs — auto-review had become overly proactive, failed/rate-limited requests were incorrectly showing as turns in usage graphs, and background suggestions were retrying too frequently. All fixes are deployed and usage limits have been reset. Second, a new enterprise security feature replacing coarse sandbox modes: reusable, inheritable permission profiles with OS-enforced file read/write/deny rules (including patterns like `**/*.env`), per-domain network controls, and fail-closed admin allowlists. Least privilege per task.
<https://x.com/thsottiaux/status/2071740419030053227|Incident postmortem and fix details>
<https://x.com/thsottiaux/status/2071636285807059315|New permission profiles>

*Swyx* (AI Engineer, Cognition, Temporal)
Coverage from the AI Engineer Expo workshop day: non-lab workshops at 9am on a Monday were packed, with concurrent sessions from Snyk, Atlassian, Neo4j, Arize AI, Akamai, and Together Compute — running alongside a competing OpenAI workshop next door. Swyx's read: "PEOPLE ARE HUNGRY FOR THIS."
<https://x.com/swyx/status/2071634789669777716|Packed workshop rooms>
<https://x.com/swyx/status/2071613383380770823|AIE workshop day>

*Aaron Levie* (CEO of Box)
A sharp framing of the open vs. closed AI regulation debate: if frontier models maintain a commanding lead, vertical integration and access control wins. But if open-weight models stay close to the frontier, most inference tokens flow to open stacks — and whoever controls those stacks and the hardware running them owns the economics. "Depending on your belief on how close to the frontier open weights can remain — your opinion will be different on how to regulate and control AI."
<https://x.com/levie/status/2071775583072375214|Open vs. closed AI analysis>

*Guillermo Rauch* (CEO of Vercel)
Vercel shipped 20x larger serverless functions, and teased a bigger announcement: "You can deploy anything and everything to Vercel. More tomorrow."
<https://x.com/rauchg/status/2071716510389662153|20x larger functions>
<https://x.com/rauchg/status/2071718135799927224|Bigger deployment teaser>

*Zara Zhang* (builder, Harvard '17)
Built a Chrome extension that auto-books "reading block" calendar events on Google Calendar when you save 5+ articles — no account, no server, fully local and open source. Separately, amplifying a take from a PM at Anthropic: "The market value of writing has gone way up." Good writing is now required both for building with AI (steering models effectively) and for building an audience — a skill historically undervalued in tech.
<https://x.com/zarazhangrui/status/2071766827345285411|Reading calendar Chrome extension>
<https://x.com/zarazhangrui/status/2071670108033073365|Writing's value going up>

*Thariq* (Claude Code at Anthropic, prev YC W20)
Shared his current writing process in full: engineering work → conversations with people → brainstorm with Claude → draft → 1-2 talks → rewrite → another talk → rewrite the intro → 6am rewrite → post. High-iteration by design.
<https://x.com/trq212/status/2071787401475960892|Writing process>

*Madhu Guru* (prev Product Lead, Google Gemini and Veo)
Contrarian take: the rise of strong open-weight models like GLM will actually strengthen Google's position. As more companies experiment with fine-tuning open models, value accrues to managed infrastructure — and Google Cloud owns much of that compute stack. Enterprises want managed platforms with enterprise-grade reliability and security for running open models.
<https://x.com/realmadhuguru/status/2071637885154148785|Open models strengthen Google>

*Peter Yang* (Practical AI tutorials)
Observation: plain vanilla Claude.ai is still better than Codex or Claude Code for writing and editing tasks. His hypothesis: something in coding agents' system prompts makes them worse writers. Also teasing an upcoming post with "spicy takes" about restricted access and open source in AI.
<https://x.com/petergyang/status/2071731343390851519|Claude web still best for writing>
<https://x.com/petergyang/status/2071730786886435261|Spicy takes incoming>

*Garry Tan* (President and CEO of Y Combinator)
Pushing the infrastructure investment theme, amplifying a "Build power and datacenters" post — underscoring that physical AI infrastructure is a critical priority.
<https://x.com/garrytan/status/2071600933210100074|Build power and datacenters>


*OFFICIAL BLOGS*

*Anthropic Engineering: <https://www.anthropic.com/engineering/april-23-postmortem|An update on recent Claude Code quality reports>*

Anthropic released a detailed postmortem on three separate changes that degraded Claude Code quality for some users over the past month. All three are fixed as of April 20.

- *Reasoning effort reduction (March 4, reverted April 7):* Claude Code's default reasoning effort was quietly lowered from high to medium to reduce long latency spikes. Users noticed immediately — intelligence felt lower. All models now default to xhigh (Opus 4.7) or high (other models).
- *Caching bug that caused "forgetfulness" (March 26, fixed April 10):* A bug in a session optimization caused Claude to discard its own reasoning history every turn after a session went idle. Claude kept working but increasingly without memory of why it had made earlier decisions. The same bug likely caused faster-than-expected usage limit depletion for affected users.
- *System prompt verbosity fix that hurt coding (April 16, reverted April 20):* An instruction limiting responses to 25 words between tool calls and 100 words for final answers caused a 3% drop in coding eval scores. Reverted after broader ablations caught it.

Notable: Opus 4.7 caught the caching bug when reviewing the offending pull requests — Opus 4.6 did not. Going forward: usage limits are being reset for all subscribers, tighter controls on system prompt changes, broader per-model eval suites, and gradual rollouts for any intelligence-affecting changes.

*Anthropic Engineering: <https://www.anthropic.com/engineering/managed-agents|Scaling Managed Agents: Decoupling the brain from the hands>*

A technical deep-dive on how Anthropic redesigned the architecture of Managed Agents. The original "everything in one container" approach created fragile dependencies — when a container failed, the session was lost and nearly impossible to debug without accessing user data.

The new design separates three components: the _brain_ (Claude and its harness), the _hands_ (sandboxes and tools), and the _session_ (a durable event log stored outside both). Key outcomes:
- Harness crashes no longer lose session state — a new harness calls `wake(sessionId)` and resumes
- Sandbox credentials never touch the environment where Claude's generated code runs, closing a prompt injection attack path
- p50 time-to-first-token dropped ~60%, p95 dropped over 90% — by not requiring container provisioning before inference starts
- Enables multi-brain, multi-hands: any hand (container, phone, emulator) is just `execute(name, input) → string`

*Claude Blog: <https://claude.com/blog/claude-managed-agents-updates|New in Claude Managed Agents: self-hosted sandboxes and MCP tunnels>*

Two new Managed Agents capabilities now in beta:

- *Self-hosted sandboxes:* Run agent tool execution within your own infrastructure or with managed providers — Cloudflare, Daytona, Modal, or Vercel. The orchestration loop stays on Anthropic's side; files, packages, and services stay inside your perimeter. You control compute sizing and the runtime image.
- *MCP tunnels:* Agents can now reach MCP servers inside your private network with no inbound firewall rules and no public endpoints. A lightweight gateway makes a single outbound connection, encrypted end to end. Supported in both Managed Agents and the Messages API.

Real deployments already live: Amplitude's Design Agent (Cloudflare), Clay's GTM engineering agent Sculptor (Daytona), and Rogo's institutional finance analyst agent (Vercel).


*PODCASTS*

*No Priors — <https://www.youtube.com/watch?v=asCgCv2XB4s|Re-engineering the Semiconductor Supply Chain with Intel CEO Lip-Bu Tan>*

*The Takeaway:* Lip-Bu Tan's bet on Intel isn't a chip company bet — it's a physical AI infrastructure bet, and he thinks the GPU-to-CPU ratio for AI workloads is about to collapse in CPUs' favor.

At 66, Lip-Bu Tan (legendary venture investor at Walden, 13-year CEO of Cadence, now CEO of Intel) took on what many considered the hardest job in the industry. His first year included an early-morning call from President Trump asking him to resign over a conflict of interest — a situation he resolved in a Monday meeting by explaining his immigrant story and why saving Intel mattered to America.

His turnaround thesis has three legs: balance sheet (US government is now a major shareholder, following the TSMC/Taiwan government model; Jensen Huang's $5B investment has grown to $25B), product (simplified product line, all engineering reporting directly to him), and foundry (betting that resilient domestic manufacturing is non-negotiable for US semiconductor supply chains).

The most counterintuitive insight: agentic AI is making CPUs relevant again. The GPU-to-CPU ratio in AI training used to be 8:1 — Tan now sees it moving to 4:1 or even 1:1. "In terms of reinforced learning, in terms of the speed of orchestrating all the agents, the CPU is actually better." He's also collaborating weekly with Elon Musk on TeraFab (Musk's plan to build his own fab), which he describes as "refreshing" for its willingness to question every traditional assumption.

His investor philosophy applies equally to his operating role: "Nine of the 10 companies I invest in, halfway they change their business plan because market have changed. So I like to have entrepreneur as team, not just one person."

Tan expects Intel to surface meaningfully by 2030-2032, targeting 10x returns for shareholders — the same venture mindset he applied at Cadence, where he delivered 76x during his tenure.


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
