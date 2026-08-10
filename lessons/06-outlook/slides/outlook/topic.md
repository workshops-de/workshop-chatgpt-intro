---
layout: cover
---

# Making Sense of It

Where this came from, and where it is going

---
layout: section
---

# How We Got Here

---
layout: why
---

# You have used it all day. Language models existed for decades — why did everyone notice in November 2022?

---
layout: little-what
---

# One architectural idea from 2017 made it possible to train on internet-scale text, and scale turned out to be the deciding factor.

---
layout: two-cols-header
layoutClass: gap-x-8
---

# The problem before 2017

::left::

Models read a sentence strictly word by word, carrying a summary of everything so far.

By the end of a long paragraph, the beginning had faded.

::right::

Worse, reading in order cannot be split across many machines.

Word two waits for word one. Training stayed slow no matter how much hardware you bought.

::bottom::
<Callout type="warning">
Two ceilings at once: the model forgot too quickly, and training could not be made faster.
</Callout>

---

# 2017: attention

The paper was called *Attention Is All You Need*. The idea: let the model look at every word at once and decide which ones matter.

> The trophy did not fit into the suitcase because it was **too big**.

What does "it" refer to? Now swap two words:

> The trophy did not fit into the suitcase because it was **too small**.

The answer flips, and nothing but the relationship between distant words tells you that.

---

# From experiment to product

| Year | Model | What was new |
|---|---|---|
| 2018 | GPT-1 | Proof that the approach works at all |
| 2019 | GPT-2 | Coherent paragraphs, held back over misuse fears |
| 2020 | GPT-3 | Useful without retraining, just by asking |
| 2022 | ChatGPT | The chat window — a million users in five days |

The models were already there. What changed in 2022 was that someone put a text box in front of one.

---

# From product to everyday tool

| Year | Model | What was new |
|---|---|---|
| 2023 | GPT-4 | Far fewer errors, understands images |
| 2024 | GPT-4o | Voice and vision in real time |
| 2025 | GPT-5 family | Reasoning becomes a standard setting |
| 2026 | GPT-5.6 family | Longer autonomous work across tools |

---

# The shift you are living through

For years the answer to every weakness was a bigger model.

Now a second lever matters just as much: letting the model think longer before it answers. That is the reasoning control you used this morning.

<Callout type="info">
Quality has become something you buy with time per question, not only with a better subscription.
</Callout>

---

# Two minutes: what did you give up on?

- When did you last try a tool like this and abandon it as useless?
- Which of the improvements above was missing back then?
- Does that one exist now?

<!--
A short discussion, not a written exercise. Around five minutes, one sentence per person, then move on.

Two things to watch for. The room can tip into venting about bad chatbot experiences — redirect with the diagnostic question about which capability was actually missing. And someone may claim nothing has really changed; take the example seriously and hold it against what they built in Lesson 5 this afternoon.

People routinely confuse a missing product feature with a weaker model. "It could not read my PDF" was usually a missing feature, not a dumber model. They saw the difference themselves in Lesson 1, with the model-versus-product distinction.

Whatever surfaces here feeds directly into the retry candidate in the closing exercise. Note the examples on the board.
-->

---
layout: section
---

# What Comes Next

---
layout: two-cols-header
layoutClass: gap-x-8
---

# From chat to agents

::left::

**The idea**

You describe a goal instead of a single task. The assistant plans the steps, uses tools and files, and comes back when it needs a decision.

::right::

**Today's reality**

Impressive on well-defined, repetitive work. Still unreliable when a step goes wrong halfway through.

Useful now, supervised, on tasks you could check yourself.

::bottom::
<Callout type="warning">
The demos are honest about what worked. They are quieter about how many attempts it took.
</Callout>

---

# The three directions worth watching

- **More senses** — voice, images, screens. The assistant sees what you see instead of only reading about it
- **More patience** — models that work a problem for minutes, so quality becomes something you buy with time
- **More connection** — access to your calendar, your documents, your systems, where the real context lives

The third one is what turns a clever text tool into something that knows your business.

---

# What stays your job

- Deciding what is worth doing at all
- Judging whether an answer is good, which needs your expertise, not its confidence
- Carrying the responsibility for what goes out with your name on it
- Knowing which questions should never be asked of a machine

<Callout type="important">
Everything the machine got better at raised the value of judgement. That part has not moved.
</Callout>

---

# Staying current without drowning

- Ignore the daily model news. It changes nothing about how you work
- Re-test one task you gave up on every couple of months. Some of them quietly became possible
- Follow the release notes of the one tool you actually use
- Talk to colleagues about what worked, not about what was announced

Thirty minutes a month is enough. The habit matters more than the volume.

---
layout: what-if
---

# What if part of your job description changes?

---
layout: task
---

# Your next 30 days

---

# What to take away

- Attention let a model weigh every word at once, which made training parallel and therefore enormous
- Each generation added context, reliability, senses and patience. The last two are what you feel day to day
- The direction is from answering questions to doing work. Agents are useful today, but supervised
- Goals, judgement and responsibility stay human, and every improvement made them more valuable
- Thirty minutes a month keeps you current, mostly by re-testing what you once gave up on

---
layout: ask-me-anything
---
