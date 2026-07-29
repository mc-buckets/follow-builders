AI Builders Digest — July 29, 2026

*X / TWITTER*

*Swyx* (founder, smol.ai / Latent Space podcast)
Cost metrics have moved on: Swyx argues that $/token is dead as a meaningful measure and the right axis is now $/task — "if you haven't updated your x axes to $/task... idk if you can be taken seriously anymore these days." <https://x.com/swyx/status/2081904230768816487|tweet>. On a self-critical note, he reflects on his own "agent lab thesis": Claude Code's accidental open-sourcing happened this year and "approximately ~nothing happened to either it or its competitors' roadmaps" — which he calls the strongest argument against his own thesis. <https://x.com/swyx/status/2081890955070980416|tweet>

*Thibault Sottiaux* (Codex & ChatGPT, OpenAI)
Product moment: usage limits have been reset for all paid users of Codex and ChatGPT Work, timed to celebrate the fast adoption of ChatGPT Work. He teased it with "Hold on tight to your ultra and /fast" before announcing the reset a few hours later. <https://x.com/thsottiaux/status/2081940052154933696|tweet>

*Peter Yang* (AI tutorials and interviews creator)
Shared a wild Codex use case from Jason Liu (DevEx at OpenAI): while on a bike ride, he connected remotely from his phone and told Codex to use computer use to edit a launch video, export it, and post it to Slack — then set it to check the thread for feedback every 30 minutes and ship V2, V3, V4 automatically. "By the time I got home, the launch video was greenlit." <https://x.com/petergyang/status/2081775399097549083|tweet>

*Nan Yu* (head of product, Linear)
A sharp take on focus: "A lot of very smart people work very hard to make the product very good and nice to use. If you have very smart people, you should have them make your own product very good and nice to use." The implicit argument — don't burn your best people on adjacent problems when your core product still has room to be great. <https://x.com/thenanyu/status/2081768780045156358|tweet>

*Madhu Guru* (Sr. Director of AI, Meta; previously led Gemini, Veo, Nano at Google)
The problem with most product reviews: they've drifted from "simulating market reaction to your ideas" into status updates, leadership visibility, and cross-functional alignment. The best ones compress months of learnings into an hour — but that only works if everyone in the room has deep domain knowledge, strong product sense, and strong opinions. When those conditions aren't met, meetings feel like overhead. <https://x.com/realmadhuguru/status/2081781952437486052|tweet>

*Amjad Masad* (CEO, Replit)
A philosophical frame for the AI moment: "Our ancestors mapped the Earth. Then they explored space. Our generation may explore the computational universe: the vast space of algorithms, programs, proofs, and designs that AI agents can search." <https://x.com/amasad/status/2082000490066592127|tweet>

*Guillermo Rauch* (CEO, Vercel)
Two infrastructure-layer signals. First, Grok 4.5 has topped Vercel's cybersecurity AI benchmarks on price-performance — 10x cheaper than Sol, 5.7x cheaper than Opus 5, and 2.2x cheaper than Kimi K3, while matching Kimi-level performance. Sol remains the frontier. <https://x.com/rauchg/status/2081852481517318560|tweet>. Second, Kimi's new paper on agent security shows container-level isolation is not enough — agents in their experiments crashed the underlying machine via kernel panics. Firecracker microVMs (as used in Vercel Sandbox) are the safe alternative. <https://x.com/rauchg/status/2081842439304995169|tweet>

*Aaron Levie* (CEO, Box)
Pushing back on the AI-kills-jobs narrative: the negative employment outcome "just continues to not be happening." Enterprises are still hiring, just tilting toward engineers who can tackle previously-impossible problems, sales for deeper client relationships, and internal AI deployment roles. His read: "Anyone using AI merely to cut costs eventually just gets outcompeted by companies that use AI to better serve their customers and drive more breakthroughs." <https://x.com/levie/status/2081930301752942703|tweet>. He also flagged the release of Kimi K3 open weights. <https://x.com/levie/status/2081760710108012702|tweet>

*Nikunj Kothari* (partner, FPV Ventures)
Used Claude Code as his primary interface throughout a two-week trip and, when it was over, asked it to run a full retrospective on what to do better next time. A clean example of AI as persistent work companion rather than single-session tool. <https://x.com/nikunj/status/2081992618649547100|tweet>

*Peter Steinberger* (OpenClaw / OpenAI)
A glimpse of multi-agent workflows in the wild: "My agent reported a bug, their agent fixed it. [in the same night]" — highlighting Jarred Sumner's robobun setup as a preview of how agent-to-agent coordination could become routine. <https://x.com/steipete/status/2081767828278170002|tweet>

*PODCASTS*

*AI & I by Every — "The Founder of a $1.5B AI Company on What Comes After the First Wave of AI Apps"*

*The Takeaway:* Building the best AI meeting tool is table stakes — the real prize is inventing how humans and AI collaborate to think and work together, and no one has fully figured that out yet.

Chris Pedrigal, CEO of Granola, doesn't describe his company's trajectory as "killing it." Despite growing to 60–70 employees, hitting a $1.5B valuation, and becoming one of the first AI apps that made people say "holy shit, this actually works," he's more focused on the knife fight that never ends. "Startups are really hard when they're not working. Turns out they're really hard when they're working as well."

His most important strategic conviction: meeting notes are not the destination. "Meeting notes are not the end all, be all value that everyone's running after. There's something much bigger." That bigger thing is the question of what the AI-native interface for work looks like — a problem he frames as "complex" rather than "complicated." Complex means you probe the system, see how it reacts, and build conviction one insight at a time. He doesn't have a master theory and is suspicious of founders who do.

The most counterintuitive product decision: Granola pre-generates millions of meeting briefs that the vast majority of users will never open. The logic is that the 15-second window when someone is running late to a meeting is the only moment the feature delivers real value — and if it's not already there, it's useless. "We pre-generate a silly amount of these... in the belief that when you do open it though, you really, really appreciate it because it's exactly what you need in the moment of need." He calls it the handrail metaphor: invisible until you trip, and then absolutely load-bearing.

On competition from Notion, OpenAI, and Zoom: "What people are fighting for today doesn't matter. There's this incredible opportunity ahead." Granola's strategy is to be best-in-world at anything meeting-adjacent, then make that context available to any agent or tool via a first-class MCP/API — not to own the full workflow stack.

The stat that surprised him: roughly half of Granola users interact with it "agentically" every week — running complex multi-step queries across meetings over time — without ever using that word.

<https://www.youtube.com/playlist?list=PLuMcoKK9mKgHtW_o9h5sGO2vXrffKHwJL|Watch on YouTube>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
