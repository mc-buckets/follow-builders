*AI Builders Digest — August 25, 2026*

*X / TWITTER*

*Thibault Sottiaux (Codex & ChatGPT, OpenAI)*
Sottiaux shared two notable updates. He confirmed a reset has been propagated to user accounts, with usage fixes rolling out and more improvements promised for Monday: <https://x.com/thsottiaux/status/2091688655828246890|tweet>. He also offered a broader industry take: "2026 is the year companies start seriously caring about model efficiency and reliability as it becomes critical infrastructure." <https://x.com/thsottiaux/status/2091581575108653374|tweet>

*Madhu Guru (Sr. Director AI, Meta)*
Guru posted part 7 of his "how to build great evals" series, introducing the Goldilocks Principle: measure at the level of each intermediate job-to-be-done, not just the final answer. Using a financial analysis agent as an example, he breaks down how to eval each stage — client understanding, evidence gathering, data analysis, recommendation — separately. "If the final recommendation is wrong, a well designed eval set would tell you: Client understanding: 92%, Evidence extraction: 92%, Data analysis: 70%, Recommendation: 75%. Now you know where to go dig." Don't make evals too granular or too coarse — just granular enough to diagnose and act. <https://x.com/realmadhuguru/status/2091684812012875981|tweet>

*Guillermo Rauch (CEO, Vercel)*
Two posts from Rauch. On pricing dynamics: OpenAI Sol's price reductions paired with Vercel AI Gateway discounts have made Sol their fastest-growing frontier model. His takeaway — AI demand is highly elastic, and gateways are now essential infrastructure for capturing price volatility to protect margins. "It's no wonder the router space has heated up... gateways are inevitable." <https://x.com/rauchg/status/2091671326897713424|tweet>

On extensibility: Vercel's philosophy for extending `fx` is open protocols — MCP, Skills, and Plugins — alongside the Unix principle of small composable programs. They're releasing `libfx` to enable embeddability into CLIs, background agents, and software factories, both local and cloud. <https://x.com/rauchg/status/2091583525661384813|tweet>

*Peter Yang (AI tutorials and interviews)*
Yang highlighted a sharp distinction from an interview with Shreya Rajpal on AI evals. Top-down evals (designed from the task description) are something Claude helps with well. Bottom-up evals — the ones that emerge from reviewing real outputs with human intuition — are a different story: "Claude is very, very bad at coming up with bottom-up evals. That's all you." <https://x.com/petergyang/status/2091586298779955512|tweet>

*Garry Tan (President & CEO, Y Combinator)*
A sharp prediction: "Systems of record will need to become AI harnesses or face replacement by agents." <https://x.com/garrytan/status/2091742825042030681|tweet>

*Peter Steinberger (OpenClaw / OpenAI)*
Two updates on his ClawFather project. On tooling philosophy: "cli is nice, having UI visualizations and your team where you work is nicer" — arguing that team-integrated UI beats pure CLI for agentic work. <https://x.com/steipete/status/2091650136506327253|tweet> He also added the USB rotation protocol to OpenClaw, letting the robot arm explore its environment using a 360° webcam. <https://x.com/steipete/status/2091639468935831910|tweet>

*OFFICIAL BLOGS*

*Claude Blog*
*<https://claude.com/blog/claude-for-foundation-models|Building intelligent apps for Apple platforms with Claude in the Foundation Models framework>*

Anthropic is releasing a Swift package that lets Apple developers call Claude directly through Apple's Foundation Models framework. Developers can use Apple's on-device models for fast local tasks — summarization, extraction — and hand off to Claude for multi-step reasoning, code generation, web search, and code execution, all in one seamless user experience.

The integration leverages `@Generable` annotations that return typed Swift values, so inputs arrive at the Claude API call already structured rather than as raw text. Apps on iOS 27, iPadOS 27, macOS 27, visionOS 27, and watchOS 27 can build hybrid on-device + Claude experiences. A journaling app can generate daily prompts locally, then ask Claude to surface patterns across months of entries. Available starting June 9, 2026.

Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
