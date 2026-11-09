# Chapter 3: Reasoning Models

- **Concept I shared on LinkedIn:** Modifying Proposal Distribution
- **LinkedIn post:** _link to add_
- **Excalidraw notes:** https://lnkd.in/e_tMrUd7 (put the `.excalidraw` file or an exported image in this folder too)

## Key takeaways

- Some problems need the model to break the question into smaller steps before answering, not just produce an answer from learned patterns.
- Reasoning models generate intermediate reasoning steps (Chain of Thought) before the final answer.
- A simplified view of an LLM: a tokenizer turns text into tokens, a stack of Transformers builds representations, and an LM head gives the probability of each possible next token. The model picks a token and repeats autoregressively.
- **Modifying Proposal Distribution:** change the probability distribution the next token is drawn from, so the model is more likely to start with tokens that begin reasoning (for example "Let's" or "First") instead of jumping to the final answer (for example "408" for `17 × 24`).
- This is not done by manually forcing token choices. It can be done with:
  - **SFT (Supervised Fine-Tuning):** train on examples that include reasoning steps before the final answer.
  - **RL (Reinforcement Learning):** use reward signals so the model learns to prefer generation patterns that lead to better results.
- The chapter covers more approaches to building reasoning models than this one concept.

## Extra resources

_to add_
