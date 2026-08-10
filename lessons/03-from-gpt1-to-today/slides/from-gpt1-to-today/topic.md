---
layout: cover
---

# From GPT-1 to Today

Why everything changed in 2017, and why you only noticed in 2022

---
layout: section
---

# How We Got Here

---
layout: why
---

# Language models existed for decades. Why did everyone notice in November 2022?

---
layout: little-what
---

# One architectural idea from 2017 made it possible to train on internet-scale text — and scale turned out to be the deciding factor.

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

# Why that unlocked the scale

- Looking at all words at once removes the memory bottleneck
- It also removes the ordering bottleneck, so training runs in parallel
- Parallel training means more text, more hardware, bigger models

<Callout type="info">
The surprise of the following years was not a new idea. It was that making the same idea much bigger kept producing new abilities.
</Callout>

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

# What actually improved

- **Context** — from a few paragraphs to entire document collections in one conversation
- **Reliability** — the same question yields a wrong answer far less often
- **Senses** — images, audio and screens instead of text alone
- **Patience** — the model can work on one task for minutes instead of milliseconds

The jump you feel day to day is mostly the last two.

---

# The shift you are living through

For years the answer to every weakness was a bigger model.

Now a second lever matters just as much: letting the model think longer before it answers.

That is why today's interface asks you how much reasoning you want, rather than which brain you would like to use.

<Callout type="info">
Practical consequence: quality has become something you can buy with time and money per question, not just with a better subscription.
</Callout>

---
layout: what-if
---

# What if the next jump does not come from size at all?

---

# Two minutes: what did you give up on?

- Which of the four improvements matters most for your own work?
- When did you last try a tool like this and abandon it as useless?
- Which improvement was missing back then, and does it exist now?

<!--
A short discussion, not a written exercise. Around five minutes, one sentence per person, then move on.

Two things to watch for. The room can tip into venting about bad chatbot experiences — redirect with the diagnostic question about which capability was actually missing. And someone may claim nothing has really changed; take the example seriously, note it down, and use it as a live test in Lesson 7. Being proven right in front of the group is worth more than any slide.

People routinely confuse a missing product feature with a weaker model. "It could not read my PDF" was usually a missing feature, not a dumber model. Good moment to preview the model-versus-product distinction that Lesson 5 makes concrete.

Someone almost always asks why it still invents things if it got so much better. That is the perfect handover into Lesson 4. If nobody asks, ask it yourself.
-->

---
layout: ask-me-anything
---
