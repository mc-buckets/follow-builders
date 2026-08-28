AI Builders Digest — August 28, 2026

*X / TWITTER*

---

*Anthropic (claudeai on X)*
Claude shipped two major browser features yesterday. Claude now has its own built-in browser inside Cowork — when a task involves a website, a browser opens in the side panel and Claude navigates, fills forms, and gets it done without touching your personal browser or logins. <https://x.com/claudeai/status/2092755571455758427|Tweet> Separately, Claude in Chrome is now generally available on all paid plans, with a new autonomous action mode (a safety classifier validates each step before running). <https://x.com/claudeai/status/2092755574563741871|Tweet>

---

*Thariq Shihipar (Claude Code at Anthropic)*
Thariq shipped a quality-of-life improvement to Claude Code: Claude now has a `SendFeedback` tool, so instead of running `/feedback` and writing a report yourself, you can just tell Claude to draft and approve it. He noted this feedback directly helps improve the product. <https://x.com/trq212/status/2092696449616376140|Tweet> He also flagged that Anthropic customers are being targeted by fraudulent API requests and gave credit to Stripe for their work combating it — describing the attacks as hurting legitimate users' ability to get usage. <https://x.com/trq212/status/2092729394565657010|Tweet>

---

*Thibault Sottiaux (Codex & ChatGPT at OpenAI)*
Sottiaux posted a pair of cryptic-but-punchy observations. First: "A few weeks at OpenAI feel like years at other companies in terms of how much gets done. Crazy how much you can age in a few days." <https://x.com/thsottiaux/status/2092756702349398036|Tweet> Then, a teaser: "A good thing about having aged is that I feel that it's been 20 years since I've pressed the reset button. Intrigued to see if I can find it tomorrow and dust it up" — suggesting something new is imminent. <https://x.com/thsottiaux/status/2092862554632826968|Tweet>

---

*Sam Altman (OpenAI CEO)*
Altman is planning a party for OpenAI's next model release, noting the 5.5 launch event was fun and crowd-sourcing ideas to make the next one better. <https://x.com/sama/status/2092733018838290817|Tweet> He also pointed to what he described as "a good report about a bad thing" — linking to external coverage of an OpenAI/Hugging Face incident involving enterprise data exposure. <https://x.com/sama/status/2092712656096358527|Tweet>

---

*Peter Steinberger (OpenClaw / OpenAI)*
Steinberger highlighted that Codex's visualization feature has gotten "really good," sharing a demo. <https://x.com/steipete/status/2092822007843061823|Tweet> He also quote-tweeted commentary questioning whether AI is in a bubble, adding a wry "maybe it is a bubble?" <https://x.com/steipete/status/2092756010280853815|Tweet>

---

*Guillermo Rauch (Vercel CEO)*
Rauch announced two infrastructure moves. First, Vercel Sandboxes now support global compute for agents — multiple regions, failover, up to 10,000 concurrent sandboxes, and 5,000 vCPUs/min ramp by default. <https://x.com/rauchg/status/2092735785460277627|Tweet> Second, Vercel is shipping a security dashboard alongside a `vercel security check` CLI — letting agents audit and improve your security posture with human-in-the-loop or on a cron schedule, similar to `is-agentic`. <https://x.com/rauchg/status/2092621371914482026|Tweet>

---

*Aaron Levie (Box CEO)*
Levie published a long post on Box's Q2: $321.1M in revenue (up 9%, 11% in constant currency — the highest constant-currency growth in 14 quarters), raising their full-year target to $1.290B. The core argument: enterprises need a secure, governed AI platform to unlock value from unstructured data (contracts, research, financial docs), swap models across providers as the market evolves, and protect against incidents like the recent OpenAI/Hugging Face data exposure. Box is positioning itself as that applied AI layer. <https://x.com/levie/status/2092702955292230100|Tweet>

---

*Matt Turck (FirstMark Capital VC)*
Turck called NVIDIA's acquisition of Hugging Face a "win-win-win": NVIDIA becomes the undisputed center of open source AI (adding HF to Nemotron), Hugging Face gets the resources and validation it needed, and open source AI broadly wins. <https://x.com/mattturck/status/2092808287280329097|Tweet> He also appeared on Dan Nathan's podcast as a guest, covering why NVIDIA might be the best venture firm in the world, the "hyper power law," why apps are becoming labs faster than labs are becoming apps, and why he's stopped underestimating China. <https://x.com/mattturck/status/2092688916969095587|Tweet>

---

*Aditya Agarwal (General Partner, SPC)*
Agarwal announced SPC's investment in DeepCogito's $43M Series A. DeepCogito is a post-training research lab focused on large-scale reinforcement learning and recursive self-improvement via iterated distillation and amplification (IDA) — a method they've demonstrated on models from 3B to 600B+ parameters. SPC met the founders as Founder Fellows in March 2024. <https://x.com/adityaag/status/2092679288869019700|Tweet>

---

*Dan Shipper (Every CEO)*
Shipper's reaction to Claude's Cowork browser launch was simply "THEY DID IT FOLKS" — his most-liked post of the day. <https://x.com/danshipper/status/2092756144447983619|Tweet> He also flagged that Codex native apps have launched <https://x.com/danshipper/status/2092686463859126492|Tweet> and described the current moment as "a definite golden age for polymaths and philosophers." <https://x.com/danshipper/status/2092636264902148262|Tweet>

---

*Josh Woodward (VP, Google Labs / GeminiApp / GoogleAIStudio)*
Woodward shared that he's experimenting with multiplayer AI — a quote tweet suggesting collaborative or multi-agent AI interactions is an active area of exploration at Google Labs. <https://x.com/joshwoodward/status/2092614266818064389|Tweet>

---

*Zara Zhang (Builder)*
Zhang posted a pointed observation on AI writing double standards: "When it comes to AI writing, many people seem to apply a double standard to the effect of 'it's fine if I use it; it's not fine if YOU use it'." <https://x.com/zarazhangrui/status/2092773720112988366|Tweet> She also noted that most PR teams at large companies end up blocking the real marketing and branding they were hired to protect. <https://x.com/zarazhangrui/status/2092774923320369394|Tweet>

---

*OFFICIAL BLOGS*

*Claude Blog: Claude in Chrome is generally available*
<https://claude.com/blog/claude-in-chrome-generally-available>

Claude in Chrome is now generally available on every paid plan. The headline addition beyond the pilot: Claude can now automatically approve actions it determines are safe, using the same classifier mechanism as Claude Code's auto mode. A safety classifier reviews each action (navigating, typing, clicking) against what you originally asked for before it runs. Anthropic's latest prompt injection evaluation shows 0% successful attacks against Sonnet 5 and Opus 5 with probes plus the safety classifier active; Fable 5 showed a 0.3% success rate, all in low-severity scenarios. The pilot phase was used specifically to harden defenses before broader release. Enterprise admins can now restrict Claude in Chrome to approved domains via Organization Settings.

---

*Claude Blog: Claude gets its own browser in Cowork*
<https://claude.com/blog/cowork-built-in-browser>

Claude now has a browser built directly into the Cowork desktop app. The key distinction from Claude in Chrome: the built-in browser is Claude's browser, not yours — it never sees your tabs, bookmarks, or passwords. It's designed for delegating web tasks (pulling numbers from a dashboard, collecting invoices from a vendor portal, filling a form) while you keep working. You can optionally bring over logins from Chrome, Edge, or Firefox site-by-site, with banking, email, and SSO sites excluded by default. Rolling out this week to Pro, Max, and Team plans; Enterprise can enable it today. The same prompt injection safeguards used by Claude in Chrome are in place.

---

*PODCASTS*

*AI & I by Every — A $10B Hedge Fund's AI Playbook (Best of the Pod)*
<https://www.youtube.com/playlist?list=PLuMcoKK9mKgHtW_o9h5sGO2vXrffKHwJL>

*The Takeaway:* The most underrated AI adoption lever isn't the technology — it's a leader willing to mandate it, model it publicly, and make "not using AI" feel riskier than using it imperfectly.

Will, CEO/CIO/Managing Partner of Walleye, a ~$10B AUM multi-strategy hedge fund, sat down with Every's Dan Shipper to lay out how he turned his firm all-in on AI — and why he felt it would be irresponsible not to. His background matters here: he's an Oxford math PhD who started his career writing algorithmic strategies, so this isn't a tech-curious executive cosplaying as a builder. He's been running quant models powered by AI for over a decade.

The most striking thing he did was send an all-firm email with the subject "AI at Walleye — a challenge to all of us." He opened it with: _"Using ChatGPT is not cheating. That's a non-applicable idea from academia. I use ChatGPT to write this email. You should be using it too and be proud of it."_ He explicitly told managers that AI adoption is now part of their job evaluation.

The concrete results: 75% of the firm uses ChatGPT or similar tools daily; about a third use AI coding tools like Windsurf; their internal fundamental investing tool "Current" (which ingests analyst notes, broker PDFs, earnings transcripts) is now considered indispensable by every PM, with 50+ external firms requesting beta access.

His most counterintuitive take: the insecurity people feel about using AI ("am I cheating if this was too easy?") is actively harmful. He compares AI to Excel — if you can't use it, you're professionally obsolete. The goal isn't to replace thinking; it's to recapture the hours wasted on the "tying your shoes" part of writing so you can spend more time on the actual concepts.

On the data strategy front, he's building toward what he calls "the Borg" — recording all internal Zoom calls and Slack messages and eventually connecting them to numerical market data, so LLMs can help surface patterns humans wouldn't catch. Right now that capability lives mostly in the "Current" product, but the vision is firm-wide.

---

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
