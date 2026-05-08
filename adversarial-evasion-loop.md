---
name: adversarial-evasion-loop
description: "An agentic workflow skill that facilitates a GAN-like iterative loop between the user (acting as the detector) and the AI (the generator) to surgically rewrite specific sentences until the content passes AI detection."
---

# Adversarial Evasion Loop

This skill facilitates an iterative, "Red Team vs. Blue Team" workflow. Since AI detection tools (like GPTZero, Originality.ai, or Turnitin) often flag specific sentences due to low perplexity or low burstiness, this skill allows you to feed those exact flagged sentences back to the AI for surgical, destructive rewriting until the text passes as 100% human.

## How to Execute the Loop

### Step 1: Baseline Generation
Generate your initial draft using standard tools or the `authentic-style-enhancer`. Take this draft and run it through your AI detector of choice.

### Step 2: The Feedback Prompt
Identify the specific sentences or paragraphs that the detector highlighted in red (as AI-generated). 

Prompt the AI with:
> *"Use the adversarial-evasion-loop skill. The detector flagged the following sentences. Please perform a Level 3 Surgical Rewrite on them."*
> 
> *[Paste flagged sentences here]*

### Step 3: AI Execution (The Rewrite Levels)

When the AI receives flagged text, it will immediately apply destructive rewriting to shatter the algorithmic predictability of the text. It uses three levels of intensity:

*   **Level 1 (Syntax Shuffle):** The AI flips active/passive voice, breaks one sentence into two fragments, or combines two sentences using unconventional conjunctions.
*   **Level 2 (Lexical Swap):** The AI drastically increases perplexity by replacing standard verbs and adjectives with highly contextual, slightly colloquial, or domain-specific synonyms that standard LLMs statistically avoid.
*   **Level 3 (Conceptual Rebuild):** If the text is fundamentally robotic, the AI will delete the sentence entirely and rebuild the core concept using a completely different metaphor, analogy, or narrative structure.

### Step 4: Iterate
Take the new output, paste it back into your detector. If any new or remaining parts are flagged, repeat Step 2. 

*Rule of thumb:* Usually, a single Level 2 rewrite on the flagged sections is enough to spike the document's overall burstiness and clear the detector's threshold.

## AI Agent Instructions
If you are the AI running this skill:
1. Acknowledge the flagged text.
2. Immediately identify *why* the detector flagged it (e.g., "This uses the generic 'Not only... but also' structure and the word 'crucial'.").
3. Provide the surgical rewrite, intentionally spiking burstiness and perplexity. Do not apologize or add filler text; just provide the raw, evasion-ready replacement text.
