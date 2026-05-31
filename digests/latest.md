*AI Builders Digest — May 31, 2026*


*X / TWITTER*

*Boris Cherny — Claude Code at Anthropic*

Boris Cherny shared a detailed thread on Salesforce's results after going fully agentic with Claude Code, and the numbers are hard to ignore. A migration scoped at 231 days shipped in 13. One PR delivered 21 endpoints at 100% test coverage. Even as more PRs shipped, total incidents dropped 5% — security guardrails and quality standards were baked directly into the agentic workflow. His broader point: the teams seeing the biggest wins aren't just speeding up existing work, they're deleting steps, eliminating handoffs, and letting agents own entire workflows end to end.

- https://x.com/bcherny/status/2060390852619272526
- https://x.com/bcherny/status/2060390853835726946
- https://x.com/bcherny/status/2060390855383400729

*Thibault Sottiaux — Codex & ChatGPT at OpenAI*

The Codex team lead teased strong growth with a cryptic but enthusiastic post: "I looked at a number today on a codex dashboard and it made me happy. More news about the number soon." He also posed a pointed question to the community: do you still trust AI benchmarks, or do you rely on word-of-mouth from friends when deciding to try a new model? With 545 replies, it clearly struck a nerve.

- https://x.com/thsottiaux/status/2060565265906290786
- https://x.com/thsottiaux/status/2060563528596287874

*Aaron Levie — CEO at Box*

Aaron Levie spotted a bullish signal for the app layer: a company reportedly spending $500M to build their own version of it. His read — "The app layer couldn't get a better advertisement than a company spending $500M to build their own version of it." He acknowledged nuance gets lost in headlines, but the bottom line is you should be very bullish on software.

- https://x.com/levie/status/2060525104384418271

*Josh Woodward — VP at Google Labs / Gemini App / Google AI Studio*

Josh Woodward shared two quote tweets highlighting AI capability jumps: one framing AI as something that can radically transform everyday experiences ("Turn your car into a Lamborghini"), and another declaring multilingual support is now "ridiculously easy." The tone is celebratory of how fast the bar has moved.

- https://x.com/joshwoodward/status/2060443095527989413
- https://x.com/joshwoodward/status/2060443093825094091

*Garry Tan — President & CEO at Y Combinator*

Garry Tan delivered a sharp piece of founder wisdom: "Money is not the fire. Money is gasoline you pour on a fire that already exists. You don't have a funding problem. You have a 'people don't want it yet' problem. Go make the first fire." A clean reframe for anyone conflating early traction problems with fundraising problems.

- https://x.com/garrytan/status/2060600088079356292

*Peter Steinberger — OpenClaw / OpenAI*

Peter Steinberger (self-described "ClawFather" at OpenClaw) expressed genuine excitement about a new hire named Vince joining the team: "Very few people understand the new ways how software is built. He gets it." A rare public signal about who's being recruited into the agentic software space.

- https://x.com/steipete/status/2060306947035832628


*PODCASTS*

*No Priors: Building an AI Guardian for Enterprise with Onyx Security CEO Maxim Bar Kogan*

_The Takeaway:_ AI agents have proliferated so fast inside enterprises that human oversight no longer scales — the only practical answer is AI watching AI, and the company best positioned to do it may not be the one selling you the agent in the first place.

Maxim Bar Kogan co-founded Onyx Security two years ago in Tel Aviv, betting early that autonomous agents would become a major enterprise liability before anyone had controls for them. He was nearly too early. The pivot point came when Claude Code and similar tools proved that truly unleashed agents — not the cautious, connector-based "low code" automations everyone was building — delivered the real productivity gains. Enterprises rushed to adopt them without guardrails, and Onyx's moment arrived.

The company's approach is worth understanding. Rather than simply proxying agent traffic, Onyx trains small, task-specific models whose only job is to recognize when a smarter agent should take a closer look: "You want to train very small models that are just good at one thing — to say, should I have a smarter agent look at this?" It's an analogy to blitz chess: most moves are intuitive pattern recognition; you only burn deep computation on genuinely critical moments.

The data moat is real but counterintuitive. Enterprises won't share historical agent behavior with Anthropic or OpenAI — they fear it will be used for training. A neutral third party like Onyx can access that behavioral history and build detection models the labs themselves cannot.

On the threat of AI-assisted vulnerability research (what he calls "Mythos-level" models): he thinks the market is not overreacting. The speed of automated vulnerability finding has arrived a decade ahead of schedule. His advice — don't wait for the perfect solution. Invest in foundational security controls now, the same way you locked down identity and endpoints before.

_"As you're exponentially doing more things with AIs, you're going to start having really bad actions happen."_

https://www.youtube.com/watch?v=QDsbFLEt9ro


Generated through the Follow Builders skill: https://github.com/mc-buckets/follow-builders
