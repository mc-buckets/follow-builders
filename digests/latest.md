AI Builders Digest — September 2, 2026

*X / TWITTER*

*Thibault Sottiaux* (Codex & ChatGPT at OpenAI) posted a question to gauge what's keeping potential users away from Codex — asking what the single biggest barrier has been for those who've considered it but haven't tried it yet. With 1,800+ replies, it's clearly generating real user research signals.
<https://x.com/thsottiaux/status/2094588317245509959|Tweet>

*Peter Yang* (AI educator and tutorials creator) made a sharp point: trust is going to be the biggest barrier — and driver — of personal AI agent adoption. Separately, he surfaced some AI advice worth reading (via a quote tweet with 1,300+ likes).
<https://x.com/petergyang/status/2094639655258091792|On trust and personal agents> | <https://x.com/petergyang/status/2094529713524117596|Great advice (quote tweet)>

*Nan Yu* (former Head of Product at Linear, now joining OpenAI) announced a major career move: joining OpenAI to work on Codex and ChatGPT. After four years helping build Linear into a beloved developer tool, they're bringing that craft into AI product. This is a notable addition to OpenAI's product team.
<https://x.com/thenanyu/status/2094427243565269107|Announcement tweet>

*Madhu Guru* (Sr. Director of AI at Meta, previously led Gemini, Veo, and Nano at Google) laid out a framework for PMs in the AI era: you should know your product's model frontier better than the frontier labs themselves. That means tracking what models can and can't do per size tier, knowing the workarounds, and projecting the roadmap 2–3 months out based on capability trajectory. "This is a core part of the PM job now."
<https://x.com/realmadhuguru/status/2094591503981281503|Full thread>

*Guillermo Rauch* (CEO of Vercel) had two notable posts. First: your next design system might be Markdown. Vercel wrote about how DESIGN.md is helping teams solve "AI slop" by encoding design taste at scale — so AI generates on-brand output instead of generic mush. Second: coding tokens are infrastructure and need governance. Without per-user and per-key budgets, companies are handing out AWS keys with no guardrails. Vercel's AI Gateway now enforces this.
<https://x.com/rauchg/status/2094541309579235680|On DESIGN.md> | <https://x.com/rauchg/status/2094523399280435630|On AI Gateway token governance>

*Aaron Levie* (CEO of Box) made two connected observations. With open-weight models improving fast and post-training infrastructure maturing, companies sitting on large proprietary datasets now have a real option to train their own domain-specific models — not just license data to labs. Separately: as AI-related security events pick up, the case for sophisticated AI security agents grows. Frontier models still lead in cyber, but open models are closing the gap fast.
<https://x.com/levie/status/2094650992818274514|On domain-specific models> | <https://x.com/levie/status/2094545525102235844|On AI and cybersecurity>

*Garry Tan* (President & CEO of Y Combinator) has a hot take on AI meeting tools: Circleback is significantly better than Granola — Granola still doesn't support multi-speaker disambiguation. He also dropped receipts on GBrain, his open-source memory retrieval layer for AI agents: new evals show it's state-of-the-art for reading memory back without an LLM in the loop, and he's added evals for memory-save from agent transcripts.
<https://x.com/garrytan/status/2094465505142960443|On Circleback vs Granola> | <https://x.com/garrytan/status/2094462971598754010|GBrain evals>

*Dan Shipper* (CEO of Every) pushed back on reflexive anti-anthropomorphism: attributing human-like traits to AI is useful when it helps you use and predict AI better. It only becomes a problem when it's weaponized to sow panic or inflate moral status claims. Most critics of anthropomorphism are reacting to its misuse — but that doesn't mean the tool itself is bad. He also dropped a one-liner worth saving: "Pragmatists stay winning in the age of AI."
<https://x.com/danshipper/status/2094406185109647580|On anthropomorphization> | <https://x.com/danshipper/status/2094397684186481057|Pragmatists stay winning>


*PODCASTS*

*Training Data: Rich Sutton and Khurram Javed — Why AI Models Stop Learning, and How to Start It Again*

_The Takeaway:_ The most fundamental problem in AI today isn't capability — it's that our best models stop learning the moment they ship.

Rich Sutton is one of the most important figures in the history of AI. He invented reinforcement learning, wrote the field's canonical textbook, and authored _The Bitter Lesson_ — the essay arguing that AI researchers keep losing to brute-force computation because they can't resist encoding human knowledge into systems that would learn better without it. Now he's founding Oak Lab with former student Khurram Javed to tackle the thing he believes is genuinely missing: continual learning.

Sutton's read on large language models is characteristically blunt. LLMs are, simultaneously, both a positive and negative example of the Bitter Lesson. They validated massive scaling with computation — you could drink in the internet and the system got dramatically more capable. But then the weights freeze. "They claim PhD-level expertise out of something that doesn't learn at all anymore," Sutton says. "I'm not the weird one. It's you guys."

Synthetic data, in his view, won't save us. The "Big World Hypothesis" — developed with Javed — holds that the world is infinitely more complex than any simulation: a synthetic dataset can't model what's going on in other people's minds, the wear in a drone's motors, or the specific physical context an agent encounters. Any simulation is microscopic. The real bottleneck is removing humans from the loop entirely and letting agents learn from their own experience.

The technical villain blocking continual learning is catastrophic forgetting: when a model updates on new data, it overwrites what it already knew. Sutton and Javed believe this is solvable via two mechanisms: per-weight step-size optimization (so most weights move slowly and only the relevant ones update) and "continual backprop," which continuously injects freshly-initialized units — seeds of new learning — into the network. They published early results in Nature.

Oak Lab's ambition is to train a new foundation model from scratch with these algorithms baked in — not retrofit an existing one — so the model learns how to learn as it learns. Target: a trillion-parameter model running on 20 watts within 5–10 years, as Moore's Law provides two orders of magnitude of efficiency gains.

https://www.youtube.com/playlist?list=PLOhHNjZItNnMm5tdW61JpnyxeYH5NDDx8


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
