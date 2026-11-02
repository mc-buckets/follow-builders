*AI Builders Digest — November 2, 2026*


*X / TWITTER*

*Swyx* (smol.ai / Latent Space)
Swyx is pushing back on the trend of maxing out AI effort levels, arguing "low effort + critique loop > superultramaxhighwhatever" for throughput-constrained workflows — and pointing to his babysit-runs skill as a practical implementation. He notes that Andrej Karpathy is using medium effort on Claude Opus 5.5 for his newly launched Hackertube project, framing effort level debates as "the tabs vs spaces of our time."
- <https://x.com/swyx/status/2116642586387730593|low effort + critique loop thread>
- <https://x.com/swyx/status/2116773135668404286|on Karpathy's Hackertube effort choice>

*Aaron Levie* (Box CEO)
Box CEO Aaron Levie draws a sharp line: if you could have produced your AI output before AI existed, you're not using it right. He argues we've crossed a threshold where AI should unlock qualitatively different outcomes — products with meaningfully better features, research consuming "every single fact on the subject across every dimension of analysis possible," and business processes that learn from all past failures in ways no human team could. His litmus test: _"If you could have done what you're doing before AI, you're likely not pushing it enough."_
- <https://x.com/levie/status/2116652002830963114|full post>


*PODCASTS*

*Latent Space: "Using Agents for Long-Horizon Financial Work — Aman Singh, Arca"*

*The Takeaway:* The real unlock for AI in financial services isn't AI-assisted advisors — it's rebuilding the entire operational model so agents run the business proactively, 24/7, with humans in the loop only where it matters most.

Aman Singh leads the AI platform team at Arca, an AI-native wealth management firm that recently raised $64M. What separates Arca from incumbents adding AI tools isn't technology — it's structure. Arca IS the firm, not a SaaS layer on top of one. That distinction lets them standardize how wealth management work happens, which is what makes deep agent participation possible. As Singh puts it: _"Agents prompt people more than people prompt agents — and it is a proactive kind of service that is running for them twenty-four/seven."_

Clients never interact with AI directly. They just experience a higher level of service, delivered through human advisors backed by powerful AI machinery running in the background. Agents handle all analysis — which assets to liquidate for a $100K tax bill, what fees a client is unknowingly paying, who's at risk of missing a required minimum distribution — but strict guardrails prevent any autonomous money movement or direct client communication. A tiered model routing system assigns Opus/Sonnet-class models to complex tax analysis and lighter models to background monitoring tasks.

The architecture is built for long-horizon work spanning 10+ days. Memory is the backbone: a nightly "dreaming process" reflects on each client's full situation, updating persistent memory so any fresh agent can instantly orient on a new signal. Every agent action generates an immutable audit log — satisfying regulatory requirements while simultaneously powering the agentic loop. Human advisor edits and cancellations are captured as first-class evals and fed nightly to a meta-agent that proposes harness improvements.

Singh is explicitly skeptical of managed agent platforms: _"Letting them own that part of the business is kind of a risk — owning your intelligence gives you the ability to impact the business."_ Decision models (like Jev) catch agents applying outdated financial data (e.g., 2025 tax brackets with confidence) and redirect them to verified knowledge bases before they affect outputs.

https://www.youtube.com/@LatentSpacePod


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders

