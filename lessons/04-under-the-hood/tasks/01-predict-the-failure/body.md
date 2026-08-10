## Overview

You now know the mechanism: text becomes tokens, and the model repeatedly picks a likely next one. That is enough to predict where it will fail — before you ever type the request. This exercise trains exactly that instinct, which is the difference between a confident user and a careless one.

## Prerequisites

- None

## Steps

### 1. Judge these eight requests

For each one, decide: does plain ChatGPT handle this reliably, or not?

1. How many times does the letter "r" appear in "strawberry"?
2. Shorten this attached two-page memo to five bullet points.
3. What did our competitor announce last week?
4. Multiply 48,271 by 9,463.
5. Name three peer-reviewed studies on remote work productivity.
6. Rewrite this rejection letter to sound warmer.
7. What is our internal process for approving travel expenses?
8. Translate this product description into French and keep the tone.

### 2. Name the mechanism, not the verdict

For every request you marked as unreliable, write which part of the mechanism causes it. Use the vocabulary from this lesson:

- It never sees individual letters
- It has no store of facts to look things up in
- It has no access to anything current without a tool
- It was never given the information at all
- Plausible-looking output is exactly what it produces

### 3. Repair three of them

Pick three failing requests and change them so they would work. You are allowed to add material, add a tool, or narrow the question.

### 4. Find the pattern

Look at your four reliable requests. Write one sentence describing what they have in common.

## Success Criteria

- [ ] All eight requests judged
- [ ] Each failure traced to a specific part of the mechanism
- [ ] Three requests rewritten so they would work
- [ ] The common pattern of the reliable ones stated in one sentence

## Troubleshooting

**"Isn't number 4 just arithmetic?"**
That is the interesting one. A language model predicting digits is guessing, but the product can run an actual calculation with a tool. The answer depends on whether a tool is involved, which is precisely the model-versus-product distinction.

**"Number 5 looks completely reasonable."**
It is the most dangerous item on the list. You will get three studies with plausible authors, journals and years. Some may not exist. This is the failure mode that damages reputations.

**"I marked everything as unreliable."**
Read 2, 6 and 8 again. All three bring their own material and ask for shaping rather than sourcing. That is the safe zone.
