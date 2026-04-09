AI Builders Digest — April 8, 2026

*X / TWITTER*

*Alex Albert — Research at Anthropic*
The biggest news of the day: Anthropic unveiled *Claude Mythos Preview*, their most consequential new model. Alex announced that Mythos is now available to launch partners in Project Glasswing and described the moment as "possibly the most consequential event in the AI industry I've seen up close since joining Anthropic almost 3 years ago." He called it a "turning point in history." The announcement sent ripples across every corner of AI Twitter.
- https://x.com/alexalbert__/status/2041579938537775160
- https://x.com/alexalbert__/status/2041579950332113155
- https://x.com/alexalbert__/status/2041578743769280811

*Sam Altman — CEO at OpenAI*
Celebrated hitting 3 million weekly Codex users by resetting usage limits — and promised to repeat the gesture every million users up to 10 million. A simple, clever milestone celebration that doubled as a product signal: Codex is growing fast.
- https://x.com/sama/status/2041658719839383945

*Aaron Levie — CEO at Box*
Levie wrote the longest and most substantive take on Mythos, arguing that "there's absolutely no wall in model capability progress right now." He also shared a detailed demo of the Box Agent autonomously filling out an RFP response from an existing knowledge base — a task that used to take hours. His broader point: agents can now do long-horizon work that was impossible six months ago, thanks to models like GPT-5.4, Opus 4.6, and Gemini 3, and the window to build for this shift is now.
- https://x.com/levie/status/2041732610179703100
- https://x.com/levie/status/2041512156693201176

*Kevin Weil — VP Science at OpenAI*
Shared the launch of Paper Review inside Prism — an AI technical reviewer built on Codex that checks math, derivations, notation, units, structure, and consistency across sections, figures, and appendices. The review outputs as an editable LaTeX file directly in the paper's workspace. It was built by teammate Hemal in a few hours as a Prism skill.
- https://x.com/kevinweil/status/2041573802212303053
- https://x.com/kevinweil/status/2041592093718749659

*Thariq — Claude Code at Anthropic*
After reviewing ~10 user session transcripts, Thariq surfaced a key efficiency insight: it's very easy to burn tokens on open-ended verification that doesn't actually improve output quality. He promised to write more on how to verify efficiently. He's also hosting a technical writing workshop in SF in two weeks, co-hosted with Swyx.
- https://x.com/trq212/status/2041722125510377705
- https://x.com/trq212/status/2041677067117588871

*Cat Wu — Claude Code at Anthropic*
Shared a thread on the Claude Code team's favorite CLI features, available via the `/powerup` command in the CLI. Short and useful for anyone using Claude Code regularly.
- https://x.com/_catwu/status/2041655441864978552

*Zara Zhang — Builder*
Launched the *Personalized Podcast skill*: turn anything into a podcast with two AI hosts, publish it as an RSS feed, and listen on any podcast app. She's been using it to remix meeting transcripts into podcasts where the AIs "eavesdrop" on her conversations. She calls it the age of "content for one."
- https://x.com/zarazhangrui/status/2041736869998948528
- https://x.com/zarazhangrui/status/2041736976630739000

*Peter Steinberger — Co-founder at OpenClaw*
Released CodexBar 0.20 — the macOS menu bar app that tracks AI coding provider usage and costs. New in this version: Perplexity and OpenCode Go providers, the ability to switch Codex accounts without re-login, and a fix for Claude token/cost inflation from duplicates. Now tracking 16 providers. Was trending on Hacker News.
- https://x.com/steipete/status/2041731875241066517
- https://x.com/steipete/status/2041719008953606148

*Swyx — AI Engineer and podcaster (latentspacepod, aiDotengineer)*
Shared Simon Willison's argument about why "prompt injection" is self-evident naming while "lethal trifecta" isn't — a riff on the naming debate around AI security terminology. Also teased something interesting from Amazon that he was going to try.
- https://x.com/swyx/status/2041739250421436591
- https://x.com/swyx/status/2041675995665612954

*Garry Tan — President and CEO at Y Combinator*
Two sharp takes: first, that Claude Code's bash access creates a sandbox escape (agents can't write files outside the workspace but can use `cat >>` to any path in the filesystem). Second, a one-liner that's been circulating: "We live in LISPy times for a specific reason: code is data and data is code again. But the weird thing? It's Markdown."
- https://x.com/garrytan/status/2041654662764609735
- https://x.com/garrytan/status/2041653129020936328

*Nan Yu — Head of Product at Linear*
Made an observation that resonated widely: designers and engineers can reason well about product in the abstract, but the moment they open Figma or an IDE, they jump straight to execution. His conclusion: more designers should become PMs — they'd be good at it.
- https://x.com/thenanyu/status/2041495924682244275

*Ryo Lu — Design at Cursor*
Shared a demo of Cursor's new interaction model: no extra buttons, just click, draw, and chat — fully in flow. Short and visual.
- https://x.com/ryolu_/status/2041564082034372956

*Nikunj Kothari — Partner at FPV Ventures*
Shared a profile on the Varanasi brothers as "Silicon Valley's greatest secret." Also pushed back on founders optimizing for viral launches over actual customer retention: "the VCs follow" the founders who focus on customers.
- https://x.com/nikunj/status/2041513787245949110
- https://x.com/nikunj/status/2041757065354293760

*Peter Yang — Product at Roblox*
Reacted to the Anthropic Mythos announcement with curiosity about whether Anthropic has been using Mythos internally to ship at their recent velocity. No notable original content beyond that.
- https://x.com/petergyang/status/2041678988318543908

*Aditya Agarwal — General Partner at SouthPark Commons*
Called the Mythos model "absurd" and added a broader framing: the 2009 conversation was about making the web read/write and malleable — "we are living through that today but for all software." What if all software could be forked, remixed, and customized?
- https://x.com/adityaag/status/2041771160359375001
- https://x.com/adityaag/status/2041658196813869414

*Guillermo Rauch — CEO at Vercel*
Spoke at Y Combinator and expressed strong conviction: "More bullish than ever. Exceptional founders. Best city, best time, best opportunity to build in generations."
- https://x.com/rauchg/status/2041720266154504351

*Dan Shipper — CEO at Every*
Posted a short prompt to "be a model manager" and shared some behind-the-scenes build progress updates. Light on substance today.
- https://x.com/danshipper/status/2041624900046106907

*PODCASTS*

*Latent Space — Extreme Harness Engineering for Token Billionaires: 1M LOC, 1B toks/day, 0% human code, 0% human review — Ryan Lopopolo, OpenAI Frontier & Symphony*

_The Takeaway:_ If you want agents to truly replace human engineers, you have to design your entire codebase and toolchain around agent behavior — not human convenience.

Ryan Lopopolo is a senior engineer on OpenAI's Frontier team, the enterprise platform for deploying agents at scale. Over five months, his small team built a 1M+ line-of-code internal product using zero human-written code. The codebase processes roughly 1 billion tokens per day. No code was written by humans. No code was reviewed by humans. This wasn't a demo or a proof-of-concept — it's in production.

The path to get there was painful. The first month and a half was ten times _slower_ than writing code by hand. But by paying that upfront cost to build "the assembly station for the agent," the team eventually outpaced what any individual engineer could do alone.

A few counterintuitive lessons that came out of this:

First, repo architecture matters more than ever — but not for the reasons you'd expect. The repo is structured like a 10,000-person engineering org, with 500 npm packages and rigid interface boundaries. Why? Because each engineer is effectively running 10-50 parallel agents. You need the surface area to avoid trampling.

Second, the inner loop has to be fast. When OpenAI shipped Codex with background shells (the ability to spawn commands asynchronously), the model became less patient with blocking builds. The team redesigned the entire build system to complete in under a minute — cycling through Make, Bazel, Turbo, and NX in weeks — because the goal was agent productivity, not human preferences.

Third, agent behavior is shaped by your skill library. The team maintains just six skills. Every new capability gets encoded into an existing skill rather than creating a new one. This lets them change agent behavior without retraining humans.

Finally, Lopopolo's team runs agent loops daily across all Codex session logs from the entire team, feeding insights back into the repository so everyone benefits from everyone else's behavior automatically.

"You can just codex things," Lopopolo said. "You can just prompt things. It's a glorious future to live in."

https://www.youtube.com/@LatentSpacePod

Generated through the Follow Builders skill: https://github.com/zarazhangrui/follow-builders
