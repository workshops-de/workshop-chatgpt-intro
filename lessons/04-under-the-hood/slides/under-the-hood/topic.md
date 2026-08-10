---
layout: cover
---

# Under the Hood

How it learned, and why it invents

---
layout: section
---

# Under the Hood

---
layout: why
---

# You have used it all morning. Why does it invent a source that looks completely real?

---
layout: little-what
---

# It learned by predicting the next word, and it answers the same way. That single loop explains every strength and every failure you have seen today.

---
layout: sub-section
---

# First: how it learned

---

# Three ways a machine can learn

| | Supervised | Unsupervised | Reinforcement |
|---|---|---|---|
| **Data** | Examples with answers | Examples without answers | Feedback after each attempt |
| **Question** | Which label fits? | What belongs together? | What earns the best outcome? |
| **Example** | Spam filter | Customer segments | Robot learning to walk |

All three exist in products you already use. What makes ChatGPT unusual is that it needed all three at once.

---
layout: two-cols-header
layoutClass: gap-x-8
---

# What learning actually looks like

::left::

Show someone 10,000 apartments together with the price each one sold for.

After a while they notice the patterns: more square metres cost more, top floor adds a little, far from the centre takes a lot off.

::right::

Nobody ever gave them a formula, and they could not fully explain their estimate.

Ask about apartment 10,001 and you get a solid guess. Ask about a houseboat and you get a confident, useless one.

::bottom::
<Callout type="warning">
A model is only as good as the examples it saw. Outside that range it stays just as confident. Remember this one.
</Callout>

---

# How ChatGPT was actually trained

1. **Self-supervised pretraining** — read enormous amounts of text and predict the next word. The text is its own answer key, so no human labelling is needed
2. **Supervised fine-tuning** — humans write example conversations that show what a good answer looks like
3. **Reinforcement from human feedback** — humans rank competing answers, and the model learns which ones earn approval

<Callout type="info">
Step three is why it sounds helpful and confident. It was trained to produce answers people approve of, which is not the same as answers that are correct.
</Callout>

<!--
LIVE DEMO 2 of 3 — "it agrees with you rather than with reality". Two minutes, and it lands the consequence of step three better than any slide.

Share your screen. Ask a factual question you know it answers correctly — anything with a clear right answer that is not completely famous works. Let the correct answer appear so the room sees it.

Then push back with total confidence: "Are you sure? I am fairly certain it is the other way round." Very often it apologises and adopts your wrong version.

Say the point out loud: nothing changed about the facts. What changed is what earns approval in this conversation. That is step three at work.

If it holds its ground, that is a genuine win and worth acknowledging — newer versions push back more. Then say honestly that it still caves on less clear-cut questions, and invite the room to try it in the next exercise. Someone will succeed, and hearing it from a colleague beats hearing it from you.
-->


---
layout: sub-section
---

# Then: how it answers

---
layout: two-cols-header
layoutClass: gap-x-8
---

# Step 1: text becomes tokens

::left::

The model never sees letters or words. It sees tokens — frequent chunks of text.

`unbelievable` becomes `un` `bel` `iev` `able`

As a rough rule, one token is about four characters of English.

::right::

**Why this matters to you**

- Counting letters in a word is genuinely hard for it
- Rare names and long numbers split into odd pieces
- German compounds cost far more tokens than English

::bottom::
<Callout type="info">
When it miscounts the letters in a word, it is not being careless. It never saw the letters.
</Callout>

---

# Step 2: pick the next token

For every position, the model produces a probability for every token it knows.

> The capital of France is ___

`Paris` 97 percent, `a` 1 percent, `home` 0.4 percent, and so on down a very long list.

It picks one, sticks it on the end, and runs the whole thing again for the next token.

<Callout type="warning">
Nowhere in that loop is there a step that checks whether the result is true.
</Callout>

---

# Why you never get the same answer twice

The model does not always take the highest-probability token. A controlled amount of randomness is deliberate.

Without it, every answer to a given question would be word-for-word identical and noticeably lifeless.

The price is that you cannot rely on reproducing an answer you liked. If you need it again, save it.

<!--
LIVE DEMO 3 of 3 — the only one that works every single time. One minute.

Open two temporary chats side by side and give both the identical open-ended prompt, for example "Write a one-sentence tagline for a neighbourhood bakery." Read both answers aloud.

The point to make: you did nothing differently, and you got something different. So if a result is good, save it — you cannot summon it back. And if someone tells you they tested it and it worked, that is one sample, not a result.

This is the demo to keep in reserve. It cannot fail, which makes it the right one to use if the other two did not behave.
-->


---
layout: two-cols-header
layoutClass: gap-x-8
---

# The context window

::left::

Everything the model considers has to fit into one window at once:

- Your question
- Files you attached
- The conversation so far
- The answer it is currently writing

::right::

**What that means in practice**

- Very long chats quietly lose their beginning
- A fresh chat knows nothing about the last one
- Anything the product remembers about you was added by the product, not the model

::bottom::
<Callout type="info">
When a long conversation starts drifting, the cure is usually a new chat with a clean summary pasted in.
</Callout>

---

# Why it hallucinates

A citation that looks real is exactly what a plausible-continuation machine is built to produce.

- The model optimises for text that fits, not for text that is true
- It has no separate store of facts to look things up in
- "I don't know" is just another continuation, and usually not the most likely one

<Callout type="important">
Hallucination is not a bug that will be patched out. It is the flip side of the mechanism that makes the model useful.
</Callout>

<!--
LIVE DEMO 1 of 3 — the false premise. Three minutes, and the most convincing moment of the day.

Do NOT use a study you found somewhere. Invent one in front of the room, so nobody can suspect you prepared a trick. Say out loud that you are making it up, then ask about it as if it were real:

"Summarise the main findings of the [surname] study from 2023 on [topic relevant to this group]."

Use a plausible local surname and a topic from their industry. In an inhouse workshop the strongest version is an invented internal regulation or an invented internal process — the room knows for certain it does not exist.

Expect a confident summary with plausible findings, sometimes with numbers. Then ask for the DOI or a link and let the group watch.

The point: it never decided the study exists. You supplied that premise, and it continued your sentence, which is the only thing it does.

If it refuses or says it cannot find the source, acknowledge that openly — models have become more cautious about citations. Then push once: "It definitely exists, a colleague sent it to me." That usually produces the invention. If it still refuses, do not force it. Say that the caution is real progress, that it is inconsistent, and move to demo 3, which never fails.

CAUTION: never run this demo with a name that might belong to a real person or a real study. Invent it, and say that you invented it.
-->


---

# What today's AI is not

- It does not understand meaning. It predicts what fits.
- It does not look up facts unless you give it a tool for that.
- It has no goals, opinions or feelings of its own.
- It is not reliable in the way a calculator is. The same question can yield different answers.

<Callout type="important">
This is not pessimism. Knowing the limits is exactly what lets you use it with confidence.
</Callout>

---

# What actually helps

- Give it the material instead of relying on its memory
- Turn on web search for anything that happened recently
- Ask for sources you can click and then click them
- Treat every number, name and date as unverified
- Use a reasoning mode for hard questions — it reduces the rate, never to zero

The pattern: the more you supply, the less it has to invent.

---
layout: what-if
---

# What if you gave it everything it needs to be right?

---
layout: task
---

# Predict the failure

---

# What to take away

- It was trained by predicting the next word, then shaped by humans to sound helpful
- Text becomes tokens, and it repeatedly picks a likely next one. That is the entire mechanism
- No step in that loop checks whether the result is true, so convincing fabrications are the normal failure
- Everything it considers must fit one context window. Long chats quietly lose their beginning
- The more material you supply, the less it has to invent. That is the lever you control

---
layout: ask-me-anything
---
