AI Builders Digest — July 18, 2026

*X / TWITTER*

*Sam Altman* (OpenAI CEO)

Sam is feeling the shift to voice-first AI interaction and is optimistic about what's coming. He says he now talks to ChatGPT more than he types to it, calling the new voice model a genuine threshold moment. On the company: a candid admission that the last 12 months weren't OpenAI's best — "mostly my fault" — but he's bullish on the next 12. His framing: "AI has to be about giving lots of people more freedom, agency, and wealth." Not the usual CEO polish.

- <https://x.com/sama/status/2077842579232895286|On ChatGPT voice crossing a threshold>
- <https://x.com/sama/status/2077817060068057493|On the last 12 months and what's ahead>

*Boris Cherny* (Claude Code, Anthropic)

In a thread on enterprise AI adoption, Boris Cherny lays out a maturity framework for teams deploying Claude Code. The real ROI question isn't usage metrics — it's "would you have spent engineering effort on this anyway, and how many eng-hours would it have cost?" The unlock at higher maturity levels: giving Claude ways to verify its own work end-to-end, using auto mode permissions, automated code review and security review, and multi-agent interfaces. Once fixing and maintaining happens in the background, teams shift from maintaining to building things that weren't even in range before. He says Anthropic is at step 3 pushing toward 4, and he personally just hit level 4.

- <https://x.com/bcherny/status/2077929390806073807|On enabling Claude to automate entire classes of work>
- <https://x.com/bcherny/status/2077929397495959693|On measuring ROI correctly>
- <https://x.com/bcherny/status/2077929404219474148|On what becomes possible at higher maturity>

*Guillermo Rauch* (Vercel CEO)

Big news on two fronts. First, Kimi K3 is now the top performer on Vercel's comprehensive web engineering benchmark — beating Fable and all other proprietary models, the first time an open model has led this benchmark. It peaks at 92% (96% with help) and reaches comparable success rates in less time. Rauch notes benchmarks don't tell the full story but calls it "important signal" and "mounting evidence that this could be a breakthrough moment for open models." Second, Vercel welcomed two legends: Pete Hunt (a React pioneer at Meta who will lead Next.js and Frameworks) and Nick Schrock (GraphQL co-inventor who will lead Agentic Developer Experience, focused on enabling the next billion agents). Both are hiring.

- <https://x.com/rauchg/status/2077900518404321759|On Kimi K3 topping the web engineering benchmark>
- <https://x.com/rauchg/status/2077870043833229692|On welcoming Pete Hunt and Nick Schrock to Vercel>

*Dan Shipper* (Every CEO)

A skeptic on Kimi K3 hype ("extraordinarily skeptical of claims it's as good as Fable"), but the more compelling thread is his analysis of OpenAI's Codex comeback. His read: OpenAI bet on agentic coding in the browser and vibe coding in ChatGPT when Claude Code was already defining the new paradigm. A small internal team broke off to build Codex separately, unencumbered by ChatGPT's legacy. By late 2025 with 5.3 it was clearly working. The Codex desktop app launched in February as a clearly superior product. Then the hard part: merging it back into the main product without destroying it. "Most companies try to disrupt themselves and fail. OpenAI somehow figured out how to disrupt their main product, and then merge it back in seamlessly. Incredible aura."

- <https://x.com/danshipper/status/2077825318992429286|On OpenAI's Codex comeback story>
- <https://x.com/danshipper/status/2077839678636732809|On Kimi K3 skepticism>

*Aaron Levie* (Box CEO)

On Kimi K3's performance: every time frontier intelligence gets cheaper, the range of enterprise workflows worth deploying expands dramatically. His take is that the biggest beneficiaries aren't the model labs — it's the applied AI layer, which can now tune and route across a diverse model ecosystem to complete full tasks for customers. Separately, Box announced a Databricks integration: enterprise content like contracts, financial documents, and supply chain data can now feed directly into Databricks analytics without moving or reprocessing the underlying files. Connect it to your ERP, CRM, or product analytics from there.

- <https://x.com/levie/status/2077857617859535112|On what cheap open model intelligence means for enterprise>
- <https://x.com/levie/status/2077782120232350205|On the Box + Databricks integration>

*Matt Turck* (FirstMark VC, MAD Podcast)

Matt Turck published an interview with Sachin Katti, OpenAI's Head of Industrial Compute, covering Stargate, Jalapeno (OpenAI's custom AI chip), and the full infrastructure buildout story. Katti's framing: data centers are "factories turning electrons into tokens," and inference may now dominate AI compute. He's designing for tokens-per-watt as the new unit that matters. On nuclear: "Can't come soon enough." On whether OpenAI is overbuilding: the bigger risk is not building fast enough. Available on YouTube, Spotify, and Apple Podcasts.

- <https://x.com/mattturck/status/2077791541167268243|Full episode thread with timestamps>
- <https://x.com/mattturck/status/2077791545323864405|Podcast link>

*Thibault Sottiaux* (Codex & ChatGPT, OpenAI)

ChatGPT desktop app update: the team shipped three improvements based on user feedback after the initial launch fell short. Conversation history and projects are now visible in the sidebar. History syncs across web, mobile, and desktop (local tasks still stay local). Switching between Chat and Work modes is now consistent across all platforms. Codex mode is unchanged.

- <https://x.com/thsottiaux/status/2077928427936710901|On the ChatGPT desktop app improvements>

*Madhu Guru* (Sr Director of AI, Meta)

A practical enterprise playbook prompted by open-weight models like Kimi and GLM. His argument: these models will force a complete rethink of the enterprise AI stack, and the companies that respond correctly will maximize model optionality. Three concrete steps: (1) Build rigorous evals — both regression (things that must always work) and aspirational (harder use cases you're scaffolding toward); eval velocity is a competitive advantage. (2) Build your own model router — nobody understands your business and users like you do, and off-the-shelf routers aren't good enough yet. (3) Build a model-agnostic harness that normalizes prompt structure, context management, tool definitions, and output parsing so switching models is a one-line change once your evals pass.

- <https://x.com/realmadhuguru/status/2077885624607228018|On rethinking the enterprise AI stack with open-weight models>

*Josh Woodward* (VP, Google Labs)

NotebookLM is officially rebranding as Gemini Notebook. What started as a small internal experiment (originally called Project Tailwind) has grown to 30 million users and 600,000 organizations. Woodward says it still feels like it's just getting started.

- <https://x.com/joshwoodward/status/2077811657385079045|On NotebookLM becoming Gemini Notebook>

*Google Labs*

NotebookLM's rebranding to Gemini Notebook is now official externally, mirroring what the team has called it internally for a while.

- <https://x.com/GoogleLabs/status/2077832590132949268|On the NotebookLM to Gemini Notebook rebrand>

*Aditya Agarwal* (General Partner, South Park Commons)

Three distinct takes today. On Kimi K3: he's already switching systems off Fable — "why would you pay the price if there is a good and free alternative?" The sharpest take: "If you have something very valuable but letting people use it allows them to recreate it, then maybe it wasn't very valuable in the first place?" — a pointed question about proprietary model moats. On a less technical note, a counter-intuitive observation for founders: the more ambitious you're operating, the more you get told no. He got turned down five times today.

- <https://x.com/adityaag/status/2077983435000324125|On switching off Fable for Kimi K3>
- <https://x.com/adityaag/status/2077983583168278961|On what it means if your moat is easily replicated>
- <https://x.com/adityaag/status/2077885770048877034|On getting told No at high stakes>

*Amjad Masad* (Replit CEO)

Amjad is building a chess engine as a side project: fine-tuned on 2 million Stockfish-labeled positions, then run through a short GRPO RL pass. It apparently outperforms frontier models at chess already. The WIP is playable and he shared annotated code and a tutorial with all the experiments.

- <https://x.com/amasad/status/2077908032944779732|On his chess engine project>
- <https://x.com/amasad/status/2077989946565206267|On NVDA not reacting to K3 news>

*Peter Yang* (AI educator)

Two observations on Claude Code's gaps: no Google Workspace connectors beyond Drive (while ChatGPT has broader integrations), and browser use is still rough enough to be frustrating. Direct product feedback worth noting for anyone comparing the tools.

- <https://x.com/petergyang/status/2077968093406707970|On Claude Code's missing Google Workspace connectors>
- <https://x.com/petergyang/status/2077966904938127502|On Claude Code browser use struggles>

*Swyx* (AI engineer, AIE World)

At AIE this year, Garry Tan and Eve Bouff headlined for the startups and design engineer tracks respectively. Swyx highlighted the value of "raw high value perspectives" from YC's top AI companies.

- <https://x.com/swyx/status/2077938877407633857|On AIE featuring YC AI companies>

*Garry Tan* (YC CEO)

Tan is pushing people toward garryslist, a new effort to organize "common sense builders" — calling it "the defining fight for California and America."

- <https://x.com/garrytan/status/2077988898601369978|On garryslist and organizing builders>

*Zara Zhang* (Builder)

A quick highlight from Chinese hardware: a face mask that doubles as a mic, so you can use voice dictation in public without being overheard. Small form factor, interesting privacy-forward design.

- <https://x.com/zarazhangrui/status/2077953473535176772|On Chinese hardware ideas>

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
