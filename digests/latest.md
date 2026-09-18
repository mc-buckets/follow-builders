AI Builders Digest — September 18, 2026

*X / TWITTER*

*Boris Cherny* (Claude Code, Anthropic)
Boris Cherny announced that Claude Code proved AI could do "real work" — developers hand Claude a feature and come back to shipped code — and that Cowork extended the same promise to knowledge workers. Now both are merging into one Claude, with context carrying across everything. He added that Claude Docs, Slides, and Design are embedded directly in conversations: "Ask Claude for a presentation and you get one you can open, edit, and export as PowerPoint or PDF. There's no separate tool to navigate to. They're just in the chat."
<https://x.com/bcherny/status/2100259951398789487|tweet 1> | <https://x.com/bcherny/status/2100260544087535639|tweet 2>

*Cat Wu* (Claude Code + Cowork, Anthropic)
Cat Wu announced the merge of Claude Cowork and chat, eliminating the need to choose which Claude product to use. Claude now handles routing — deciding whether to give a quick answer or do deeper agentic work, and what kind of output fits the task. Claude Design is now integrated directly into conversations. "You're in control the whole time: you can still stop, redirect, or exert finer control over Claude's effort or approach."
<https://x.com/_catwu/status/2100260655312089562|tweet>

*Alex Albert* (Research, Anthropic)
Alex Albert praised the chat/Cowork merge, saying the combined UX is "so much better than chat or Cowork did on their own" and that the new Slides, Docs, and Design integrations "work very well."
<https://x.com/alexalbert__/status/2100295757953917120|tweet>

*Thariq* (Claude Code, Anthropic)
Thariq shared evolving thinking on agentic tool design. Bash is no longer "all you need" for reliable tool calling — you're better off giving Claude tools shaped how you actually want them (e.g. a database API instead of a raw filesystem). That said, sandboxes + bash remain valuable for code generation and execution. Claude Managed Agents handles this well by keeping the sandbox optional and independent from the agent loop.
<https://x.com/trq212/status/2100315535758217422|tweet 1> | <https://x.com/trq212/status/2100315537251463523|tweet 2> | <https://x.com/trq212/status/2100315538472009897|tweet 3>

*Claude* (Anthropic's official account)
The official Claude account detailed what's new: Docs, Slides, and Design are in beta on all paid plans. You can draft a one-pager in Claude Docs, turn it into a deck with Slides, and mock up a visual in Design — all from one conversation. Cowork users' chats, projects, artifacts, connectors, and skills are fully preserved. You can edit directly, present from Claude, or download as PowerPoint or PDF, then share everything at one link.
<https://x.com/claudeai/status/2100258492590207079|tweet 1> | <https://x.com/claudeai/status/2100258494221812123|tweet 2> | <https://x.com/claudeai/status/2100258495543071016|tweet 3>

*Dan Shipper* (Every, CEO)
Dan Shipper greeted the Claude chat/Cowork merge with full enthusiasm — "THEY DID IT / THE END OF THE TABS ERA IS UPON US" — and threw in a pointed quip about LLM skepticism: "LLMs are just autocomplete / jev is just a JSON classifier 🤝 🚩."
<https://x.com/danshipper/status/2100269017977987341|tweet 1> | <https://x.com/danshipper/status/2100284086703046903|tweet 2> | <https://x.com/danshipper/status/2100251499443998766|tweet 3>

*Guillermo Rauch* (Vercel, CEO)
Guillermo Rauch shared early results from typesafeai's safety reviewer running on GPT Luna inside Vercel's fx tool: 18x faster at p95 and more accurate. He expects this to come to Vercel AI Gateway as the likely new default.
<https://x.com/rauchg/status/2100307962262872105|tweet>

*Sam Altman* (OpenAI, CEO)
Sam Altman teased a delayed launch: "the main thing I was excited about launching this week will be next week instead, but imo worth the wait!" No further details.
<https://x.com/sama/status/2100351958167220547|tweet>

*Thibault Sottiaux* (Codex & ChatGPT, OpenAI)
Thibault Sottiaux posted about a new model called "Astra" — fast, frontier, efficient, and for everyone — and commented "sometimes physics can't be cheated" in response to Altman's delayed announcement, suggesting real engineering constraints are still in play even at the frontier.
<https://x.com/thsottiaux/status/2100297380968997327|tweet 1> | <https://x.com/thsottiaux/status/2100363668051603608|tweet 2>

*Aaron Levie* (Box, CEO)
Aaron Levie is bullish on fast, low-cost, high-capability AI models for the enterprise. He sees the biggest wins in what he calls "gate functions" — data classification, routing decisions, domain-specific judgment calls, and safety/security checks — that sit inside large numbers of enterprise workflows. "This model and approach could be quite cool in agentic workflows in the enterprise."
<https://x.com/levie/status/2100448648672993540|tweet>

*Madhu Guru* (Sr Director of AI, Meta)
Madhu Guru made the case that safety and security should be *features* of your AI product — not external guardrails imposed from outside. A pointed framing as AI companies navigate regulatory and policy pressure.
<https://x.com/realmadhuguru/status/2100312717739667963|tweet>

*Peter Yang* (AI tutorials creator)
Peter Yang shared his full podcast production workflow built on 8 custom Claude skills: /podcast-prep for guest research and interview guides, /podcast-edit for transcript review and quote selection, and /podcast-production to turn the episode into 6 different assets. His take: custom skills remain indispensable for getting AI to follow specific editing and browser-use instructions, even with the latest models. Demo video linked in the tweet.
<https://x.com/petergyang/status/2100328939034128856|tweet>

*Zara Zhang* (Builder)
Zara Zhang flagged growing frustration with Claude's communication style: "it's constantly trying to showcase how smart/sophisticated it is, rather than actually communicating a point across." The critique resonated — 1,800+ likes and 300+ replies — and lands as useful signal for anyone tuning AI communication.
<https://x.com/zarazhangrui/status/2100278750776824115|tweet>

*Nikunj Kothari* (FPV Ventures, partner)
Nikunj Kothari shared progress on a "Home" NousResearch agent he and his wife have been building together for months. What makes it work: granular control — reading only specific emails, converting inline attachments to structured data, maintaining logged-in browser sessions. He couldn't replicate this level of control with Grok Bot or similar alternatives.
<https://x.com/nikunj/status/2100212813625196917|tweet>

*Garry Tan* (Y Combinator, President & CEO)
Garry Tan highlighted the appeal of a personal AI with consistent personality and full memory across any interface or harness. No specific product announced, but the framing signals what he thinks matters most in AI UX.
<https://x.com/garrytan/status/2100339347669279149|tweet>


*OFFICIAL BLOGS*

*Claude Blog*
<https://claude.com/blog/cowork-is-now-claude|Claude Cowork and chat are now one Claude>

Anthropic is merging Claude Cowork and chat into a single Claude, rolling out to Pro and Max plans over the coming weeks. The pitch: bring a quick question or hand over a complex deliverable — Claude decides how much effort to apply and what output format fits best.

Three new tools launch alongside: *Claude Docs* and *Claude Slides* are new, and *Claude Design* is now available inside any conversation (in addition to its standalone version). All three are in beta on paid plans. You can draft a one-pager in Docs, turn it into a slide deck, and mock up a visual in Design — all from one thread. Edit directly, present from Claude, or export as PowerPoint or PDF.

Key quote from a user: "I could have Claude pull up [my legal research database], and it would pull all the cases, read them, figure out which other cases I might need, download them, and store them in a folder for my personal review."

Cowork users keep everything: chats, projects, artifacts, connectors, and skills. Enterprise admins get at least 30 days notice before any changes. Team and Free plans follow after Pro and Max.

<https://claude.com/blog/cowork-is-now-claude|Read the full post>


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
