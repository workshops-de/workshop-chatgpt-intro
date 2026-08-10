---
layout: cover
---

# Prompting

Supplying the context the model cannot guess

---
layout: section
---

# Prompting

---
layout: why
---

# Same model, same question, completely different answers. The variable is you.

---
layout: little-what
---

# A good prompt says who is asking, what for, with which material, and what the result should look like.

---
layout: two-cols-header
layoutClass: gap-x-8
---

# The same request, twice

::left::

**What most people type**

> Write something about our new product launch.

The model has to guess the audience, the channel, the tone, the length and every fact about the product.

It guesses average, because average is the most likely continuation.

::right::

**What actually works**

> You are writing for our existing B2B customers.
>
> Draft a short launch email for the attached product sheet.
>
> Around 150 words, plain German, one clear call to action.
>
> No superlatives.

::bottom::
<Callout type="info">
Nothing here is clever wording. It is just the information the model had no way of knowing.
</Callout>

---

# The five building blocks

- **Role** — who is speaking and to whom
- **Task** — one clear verb: draft, summarise, compare, rewrite
- **Material** — the actual source text, pasted or attached
- **Format** — length, structure, language, tone
- **Constraints** — what to avoid, what to leave out

You rarely need all five. You almost always need material and format.

---

# Bring the material

The single biggest quality jump does not come from better wording. It comes from stopping the guessing.

- Paste the source text instead of describing it
- Attach the document, the spreadsheet, the screenshot
- Add the example your company already published
- Say what you have already tried and why it did not work

Every fact you supply is a fact it cannot invent.

---
layout: two-cols-header
layoutClass: gap-x-8
---

# What about just giving it a link?

::left::

**Pasting and attaching are reliable**

The text sits in the conversation. There is no question about whether it arrived.

::right::

**A link is convenient and conditional**

- It only helps if the page was actually fetched
- Intranet links, logins and paywalls are out of reach
- Pages built entirely in JavaScript often arrive empty

::bottom::
<Callout type="warning">
If it did not fetch the page, it will answer anyway. Ask it to quote the first heading — no quote, no page.
</Callout>

---

# Let it interview you

The most useful sentence for a beginner:

> Ask me questions until you have everything you need to do this well. Then start.

It turns a bad prompt into a good one without you knowing what a good prompt looks like.

Especially useful when you cannot yet name what you want, which is most of the time.

---
layout: two-cols-header
layoutClass: gap-x-8
---

# Iterate, do not restart

::left::

**What people do**

Get a mediocre answer, close the chat, rewrite the whole request from scratch.

::right::

**What works better**

Stay in the conversation and correct:

- "Shorter, and drop the last paragraph."
- "Same content, but for someone who has never heard of us."
- "Give me three versions of the opening line."

::bottom::
<Callout type="info">
The second and third message are usually where the useful output appears.
</Callout>

---

# Checking an answer you cannot verify

- Ask for sources and actually open one
- Ask it to argue the opposite case and see whether that sounds equally convincing
- Ask which parts it is least certain about
- Spot-check one concrete fact. If that one is wrong, assume the rest is too
- For anything numerical, recalculate it yourself

<Callout type="important">
Confidence in the wording tells you nothing about correctness. It is a style, not a signal.
</Callout>

---

# The usual pitfalls

- Asking for five things in one message and getting five mediocre answers
- Treating a fluent answer as a checked answer
- Accepting statistics, citations and quotes without opening them
- Letting a long chat drift instead of starting clean
- Pasting things that should never leave the building

---
layout: what-if
---

# What if you never had to write the same prompt twice?

---
layout: task
---

# Rewrite a bad prompt

---
layout: task
---

# Prompt gym: three rounds, four minutes each

---

# What to take away

- Role, task, material, format, constraints. Material and format do most of the work
- Paste the source instead of describing it. Every fact you supply is one it cannot invent
- When you cannot name what you want, let it interview you before it starts
- Fluent is not checked. Open one source, recalculate one number, then decide
- A prompt worth repeating belongs in your project instructions, not in your memory

---
layout: ask-me-anything
---
