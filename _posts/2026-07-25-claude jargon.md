---
title: incoherent claude jargon is not how smart people talk
tags: computers
---

There is a speech pattern where I like to call claude-jargon. If you don't know what that means, it's because I just made that word up, and now I expect you to derive the meaning from surrounding context.

A few more examples I found from my own chats and the internet for what I mean, emphasis mine:
- >concrete *unstuck-move*
  - this is meant to be "a more concrete thing you can do to stop getting stuck (on the current task)"
- >The eval code deduplicates positives; the training *path* doesn't
- >The *product lever* nobody's pulled
- >Sign-off is per-decision on the canonical structure; tiers are projections gated by an automated caveat-drop/entailment check at export.
  - from [here](https://www.reddit.com/r/ClaudeAI/comments/1uok58g/comment/ovsxo4i/). no emphasis needed. this is some late-stage claude-jargon syndrome.

The pattern is especially prevalent in Anthropic's larger models (like Opus and Fable), and after working for extended periods of time (AKA yapping to itself a lot). Some describe them less as jargons, but more weird metaphors.

Occasionally, you'll hear claims that it's "how smart people talk". It is not. If anything, it is "how people who _act_ smart talk". The whole point of jargon is clarity, something established in the field beforehand that two experts mutually understand. We can write research papers in layman terms, but you won't know "the repeated part of a song" actually means "chorus". If there is a need, jargon can be established by clearly defining it, not inserting it randomly in a sentence and expect the reader to go along.

Careful word choice is a skill, a failure to do so is usually a sign that the writer's understanding is not specific enough. This post was initially written with more complex words, but through effort of thinking about what i truly want to say, i was able to express it in simpler wording. In fact, my writing style starts resembling claude-jargon when I'm extremely tired, full of words that are semantically related to what I'm thinking, but I can't articulate it properly.

Claude-jargons are clear to neither experts nor laymen. You cannot just call a chorus "song's semantic home". Sometimes it gets extremely ambiguous - "home" to what? The real purpose seems to be sacrificing legibility to write in less tokens. Whether this is intentional on Anthropic's part or a training artifact is anyone's guess.

Fortunately, no real person makes that claims. The only people are Anthropic shills who are trying to sell the idea that Claude models are uniquely expert and human.

## Bonus
Here's an untested prompt that you can copy and past into your custom instructions, courtesy of Claude itself. Will it work? I don't know, I think it will to some extent, but I doubt it will fix the root cause.

```
Don't invent new compound terms, metaphors, or nicknames to describe a concept, if you can say it in simple terms. If a field already has a standard term for something, use that term correctly; don't stack it with other jargon or use it loosely to sound precise when it isn't. When you catch yourself reaching for a novel noun phrase (like "unstuck-move" or "product lever") to describe a fuzzy idea, stop and just say the idea directly in plain words, even if it takes more words.
```
