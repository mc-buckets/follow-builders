*AI Builders Digest — July 5, 2026*


*X / TWITTER*

*Swyx* (AI engineer, Latent Space / Cognition / dx.tips)
The tools-for-thought crowd spent a decade building beautiful, polished canvas UIs — and got completely beaten by low-contrast, barely designed CLIs that actually do the thinking for you. The irony is sharp and his take is blunt. <https://x.com/swyx/status/2073220591684096087|tweet>

*Nan Yu, head of product at Linear*
Three observations landed in quick succession. Tailwind being adopted by the company that created Bootstrap is being called a decisive win for utility-first CSS. <https://x.com/thenanyu/status/2073194274435317767|tweet> More contrarian: "if your field doesn't produce good training data it was probably full of crap to begin with" — a pointed take on which industries AI will actually transform. <https://x.com/thenanyu/status/2073070255031615877|tweet> On AI in healthcare: the best scenario isn't AI replacing doctors, it's a doctor who spends real time with you while using LLMs to do it better. <https://x.com/thenanyu/status/2073066919200956793|tweet>

*Cat Wu, Claude Code & Cowork at Anthropic*
A useful tip: you can use Claude Code with computer use to automatically set up Claude Tag — just point it at the Claude Tag docs and it will connect your team's GitHub repo, data warehouse, Google Drive, and other data sources for you. <https://x.com/_catwu/status/2073149354412822738|tweet> She's also collecting Fable 5 weekend demo builds from the community. <https://x.com/_catwu/status/2073147672106873001|tweet>

*Thariq, Claude Code at Anthropic*
Shared a thread from his AI Engineer (AIE) talk on working effectively with Fable. His core insight: the most important part of working with an AI model is discovering your own unknowns so you can prompt it better. He shared examples of HTML artifacts purpose-built to surface what you don't know you don't know. <https://x.com/trq212/status/2073101078145724589|thread> See examples here: <https://x.com/trq212/status/2073101079877943683|tweet>

*Replit CEO Amjad Masad*
Video generation is now live on Replit. <https://x.com/amasad/status/2073003971287863717|tweet>

*Vercel CEO Guillermo Rauch*
Pushing the concept of agentic self-improvement: give your agent the ability to introspect its own past runs, spot inefficiencies, errors, and redundant tool calls, and generate improved prompts and skills from that analysis. He notes that built-in agent observability on Vercel is designed for exactly this feedback loop. <https://x.com/rauchg/status/2073132174958841887|tweet>

*Box CEO Aaron Levie*
A long and substantive thread: the AI wars are becoming a battle for context. The real moats aren't at the model layer — they're in the applied AI layer that organizes domain knowledge, governs access, routes intelligently between frontier and lower-cost models, and handles the change management that actually gets agents into customer workflows. "The applied AI layer has a lot more value than just being an LLM wrapper. The ability to organize the critical knowledge for the work being done, and maintain this knowledge in a governed way... is critical." Domain-specific post-training of near-frontier base models also gets a mention as a cost and performance play for specific task types. <https://x.com/levie/status/2073138135014502777|thread>

*YC President & CEO Garry Tan*
Specialist wait times are going up at exactly the moment AI is about to change everything in healthcare. His expectation: AI will bring quality of care up 100x, and not a moment too soon. <https://x.com/garrytan/status/2073053799791710301|tweet>

*Zara Zhang, builder*
A sharp market observation: people are getting less willing to pay for tools now that they can build them with coding agents. What they'll still pay for is "the feeling of hiring expertise they don't have." <https://x.com/zarazhangrui/status/2073295900395606401|tweet>

*Nikunj Kothari, partner at FPV Ventures*
A rare positive take on Gemini from one of its vocal critics: it remains the only place where a single API key covers Flash (fast/cheap/long-context), Nano (world-class images), real-time audio/video, search with grounding, and more — making it the default for many of his side projects. <https://x.com/nikunj/status/2073151491557478883|tweet> Also floated a pattern worth noticing: Anthropic seems to drop major models right before long weekends — Opus 4.5 before Thanksgiving, Fable 5 before July 4th — giving the masses time to tinker and go deep into "token anxiety." <https://x.com/nikunj/status/2073071325644816440|tweet>

*Peter Steinberger, OpenClaw*
Practical tip: if you think Codex falls short on design work, try prompting it with "use imagegen to re-imagine this design and implement that." <https://x.com/steipete/status/2073277317464682723|tweet> Also fed Fable 80,000 of his own tweets so it could roast him even harder. <https://x.com/steipete/status/2073295890857758810|tweet>

*Dan Shipper, CEO of Every*
Pushed back on claims that Fable 5 is a different model than Claude: it's the same model, but falls back to Opus 4.8 slightly more often, so benchmarks are measuring a blend of both. "Skill issue." <https://x.com/danshipper/status/2073097796941484486|tweet> Also shared Every's Fable 5 prompt library. <https://x.com/danshipper/status/2073077325520838993|tweet> And put context window scale in perspective: "A new personal iOS app working end to end: 5M tokens / Your whole prod bug backlog cleared: 20M tokens / Unnecessarily detailed responses to every single unread email, Slack, and text message: 30M tokens / Fable working for you while you're at the pool: Priceless." <https://x.com/danshipper/status/2073076447992746379|tweet>


*PODCASTS*

*The MAD Podcast with Matt Turck — Why NVIDIA Is Giving Away AI Models | Bryan Catanzaro*

_The Takeaway:_ NVIDIA doesn't build frontier AI models to compete with Anthropic or OpenAI. It builds them because the only way to design chips that run AI well is to understand AI deeply from the inside — and giving those models away is simply good ecosystem strategy.

Bryan Catanzaro leads Nemotron, NVIDIA's family of open foundation models. He's been at this since 2008, when he published the first paper on training neural networks on GPUs at ICML and was told his work didn't belong there. He briefly ran NVIDIA's Silicon Valley AI Lab at Baidu alongside Andrew Ng — and was on the interview panel when a young Dario Amodei came in. "It was very clear that he learned extremely quickly and thought extremely deeply. The thing I admire most about Dario is the strength of his conviction." Today Catanzaro leads the applied research team behind Nemotron three Ultra, which just became the number one US open weights model.

His case for open AI: every company is built around a secret — proprietary data, business models, regulatory constraints. Open models let companies build AI that's tightly integrated with those secrets in a way closed APIs can't fully support. "The value of AI is greater when it can be more tightly connected with those secrets."

On Moore's Law: "It's been dead for years." When you can't shrink your way to performance anymore, you have to think from first principles. That's the whole point of accelerated computing, and why NVIDIA needs Nemotron — not as a commercial AI product, but as a research vehicle that informs Blackwell chip design. The team's work on hybrid SSM/attention architectures, mixture of experts, and multi-token prediction feeds directly back into hardware decisions. The NVL 72 interconnect — 72 GPUs reading and writing each other's memory at high speed — exists specifically because MoE routing is unpredictable and needs low-latency cross-GPU communication.

Multi-token prediction is the most counterintuitive piece: the model speculatively generates several tokens at once, checks them on the next pass, and accepts the correct ones. The result is an accuracy-speed flywheel: "The more accurate your model is, the faster the inference is, the cheaper the inference is." That's not usually how compute-bound systems work.

"A GPU is whatever NVIDIA says it is. We make them. A GPU is a thing that we make in order to accelerate the world's most important computations, which in 1995 was graphics. And for a long time now, it's been AI."

https://www.youtube.com/watch?v=Oojrfdl42LI


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
