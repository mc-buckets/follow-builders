AI Builders Digest — May 29, 2026

*OFFICIAL BLOGS*

*Anthropic Engineering*

*<https://www.anthropic.com/engineering/april-23-postmortem|An update on recent Claude Code quality reports>*

Three separate bugs degraded Claude Code quality over the past month — all fixed as of April 20 (v2.1.116). The API was not impacted.

- *Reasoning effort downgrade (March 4):* Default reasoning effort was changed from high to medium to reduce latency. Users noticed Claude felt less intelligent. Reverted April 7; all users now default to xhigh effort for Opus 4.7 and high for other models.
- *Caching bug (March 26):* A bug meant to clear old thinking blocks from idle sessions instead cleared them on _every_ subsequent turn, making Claude seem forgetful and repetitive — and causing extra cache misses that drained usage limits faster. Fixed April 10.
- *Verbosity prompt change (April 16):* A system prompt addition ("keep text between tool calls to ≤25 words") caused a 3% drop in coding quality. Reverted April 20.

Because the bugs hit different traffic slices on different schedules, they looked like broad inconsistent degradation. Going forward: tighter eval suites for every system prompt change, per-model ablations, broader soak periods, and gradual rollouts. Usage limits reset for all subscribers as of April 23.

*<https://www.anthropic.com/engineering/managed-agents|Scaling Managed Agents: Decoupling the brain from the hands>*

Anthropic's engineering team details the architecture behind Managed Agents — a hosted service for long-horizon agents — built around one core principle: decouple the "brain" (Claude + harness) from the "hands" (sandboxes, tools) and the session (the durable event log).

The original single-container design was fragile — one failure lost the entire session. The new architecture treats every component as replaceable: if a container fails, the harness catches it as a tool error and Claude can retry with a fresh one. If the harness itself crashes, a new one boots and resumes from the last logged event via `wake(sessionId)`.

Key results: p50 time-to-first-token dropped ~60%, p95 dropped over 90%. Security improved because Claude's generated code never touches credentials — auth tokens live in a vault or are wired in at sandbox init, never passed through the harness.

The session log — stored outside Claude's context window — provides durable, queryable context without forcing irreversible compaction decisions. The `getEvents()` interface lets the brain select positional slices of the event stream, rewind, or re-read context before a specific action.

*Claude Blog*

*<https://claude.com/blog/claude-managed-agents-updates|New in Claude Managed Agents: self-hosted sandboxes and MCP tunnels>* _(May 19, 2026)_

Two new enterprise capabilities for Managed Agents: self-hosted sandboxes (public beta) and MCP tunnels (research preview).

- *Self-hosted sandboxes:* Anthropic's orchestration layer handles the agent loop; tool execution runs in your own infrastructure or with managed providers (Cloudflare, Daytona, Modal, Vercel). Sensitive files and repos never leave your perimeter. You control compute sizing and the runtime image.
- *MCP tunnels:* Agents reach private MCP servers (internal databases, APIs, knowledge bases) via a single outbound connection — no inbound firewall rules, no public endpoints, fully encrypted. Available in Managed Agents and the Messages API.

Real deployments: Amplitude is using Managed Agents + Cloudflare for an internal design agent. Clay's GTM engineering agent (Sculptor) runs on Daytona. Rogo is building an institutional finance analyst agent on Vercel Sandbox.

*<https://claude.com/blog/connectors-for-everyday-life|New connectors in Claude for everyday life>* _(Apr 23, 2026)_

Claude's connector directory now includes consumer and lifestyle apps alongside work tools. New additions: AllTrails, Audible, Booking.com, Instacart, Intuit Credit Karma, Intuit TurboTax, Resy, Spotify, StubHub, Taskrabbit, Thumbtack, Tripadvisor, Uber, Uber Eats, and Viator.

Claude now proactively suggests relevant connectors mid-conversation based on what you're doing. When multiple connected apps could help, it surfaces all of them and lets you choose. Claude is ad-free with no paid placements. Data from connected apps isn't used for model training. Actions like bookings or purchases require your approval before Claude proceeds.

*PODCASTS*

*AI & I by Every — <https://www.youtube.com/watch?v=dCmOTURRf1Y|We Automated Everything With AI and Tripled Our Headcount>*

*The Takeaway:* More automation creates more human work, not less — and companies publicly crediting AI for mass layoffs are mostly just covering for bad business performance.

Dan Shipper, CEO of Every (an AI-native media company), makes a counterintuitive case from direct experience: Every grew from 4 to 30 people _while_ becoming as agent-native as any company out there. Everyone uses Claude Code and Codex daily. And yet there's more human work than ever.

His explanation: AI makes "yesterday's expert competence cheap." Non-experts can now generate code, essays, and designs with a prompt — which floods the zone with output that's close but not quite right. That actually creates _more_ demand for experts: to build systems that shepherd near-miss output into something actually good, and to build things that simply couldn't have been built before.

_"The further away an agent gets from a human, the less valuable it is."_

On benchmarks: yes, models improve exponentially. But once you saturate a benchmark, it's easy to reframe the problem and zero it back out. More fundamentally, AI is built to look back at you and ask "what should I do next?" — and that design intent isn't going away, because we wouldn't build it otherwise.

On the ClickUp CEO who fired 20%+ of his workforce and bragged about it: Shipper is skeptical. When companies claim AI let them cut dramatically while performing better than ever, look closer — they're usually a struggling SaaS business that needed to cut costs anyway, and AI makes a convenient narrative.

The practical call to action: _"If you just ride the models — when new models come out, learn to use them for what you do — you're going to be fine."_

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
