# Where a Word Goes

An interactive 3D notebook that follows one token, " prices", through a large language model, from the tokenizer to preference tuning. Built with Three.js; no build step.

**Open it:** `index.html` (enable GitHub Pages on this repo to use it from any device).

## The ten stops

| # | Stop | What you play with |
|---|------|--------------------|
| 1 | Tokens | read by letters vs word-pieces, add a rare word |
| 2 | Embeddings | look up a word, compare the table before and after training |
| 3 | Attention | choose who is asking, let it peek at the future |
| 4 | Feed-forward | send a token through the detector bank, remove attention's context |
| 5 | Layers | read the guess at any depth, remove residual connections |
| 6 | Predict | change the end of the prompt, see raw scores vs probabilities |
| 7 | Sampling | set the temperature and spin the wheel |
| 8 | Learning | set the learning rate and train on a loss surface |
| 9 | Fine-tuning | change the LoRA rank, train, merge |
| 10 | Preferences | loosen the KL leash, plant a bug in the reward scorer |

Each stop: predict first, run the guided experiment, lift the "Why?" flap, then answer the exam question later from the spaced-repetition recall deck.

Numbers inside the models (token ids, attention scores, layer-by-layer guesses) are illustrative, not taken from a real model. Progress and the recall deck are saved in your browser's local storage, so they stay per device.

## Also here

`lab.html` — the earlier **LLM Mechanics Lab**: six free-play 3D simulations (embeddings, attention, sampling, gradient descent, LoRA, RLHF/DPO) with recall cards.

## Files

- `index.html` — Where a Word Goes (single self-contained page; loads Three.js r128 and Google Fonts from CDNs)
- `lab.html` — LLM Mechanics Lab
