---
name: personal-stylometry-cloner
description: "Ingests user-provided writing or code samples to extract a unique stylometry profile, then uses this profile to rewrite AI-generated content so it perfectly mimics the user's authentic digital fingerprint."
---

# Personal Stylometry Cloner

This skill turns the AI into a perfect mimic of your personal writing or coding style. Instead of applying generic "human-like" imperfections, it analyzes your actual past work to extract your unique digital fingerprint (Stylometry Profile) and forces all future outputs to adhere strictly to it.

## Phase 1: Ingestion and Profiling

When you want to clone a style, provide 3 to 5 samples of your authentic work (e.g., past emails, blog posts, or code commits).

Prompt the AI with:
> *"Use the personal-stylometry-cloner skill. Here are 3 samples of my work. Please analyze them and output my `[Stylometry Profile]`."*

The AI will output a profile detailing:
1.  **Lexical Fingerprint:** Your favorite transition words, specific jargon, and words you *never* use.
2.  **Punctuation & Formatting Quirks:** Do you over-use em dashes? Do you prefer lowercase bullet points? Do you put spaces inside brackets?
3.  **Cadence & Rhythm:** Your average sentence length, your tendency to use rhetorical questions, or your paragraph pacing.
4.  *(For Code)* **Naming & Commenting Habits:** Your specific variable abbreviation habits (e.g., `cnt` vs `count`), casing choices, and whether your comments are pragmatic (`// fix later`) or descriptive.

## Phase 2: The Cloning Execution

Once the `[Stylometry Profile]` is generated (or if you already have one saved from a previous session), you can use it to rewrite any sterile AI content.

Prompt the AI with:
> *"Here is a sterile AI draft. Rewrite it completely. You must strictly adhere to the following `[Stylometry Profile]` so that it reads exactly as if I wrote it."*

### Execution Rules for the AI during Cloning:
*   **Absolute Compliance:** The AI must abandon its default safety/neutrality training and adopt the user's specific quirks, even if those quirks are grammatically imperfect or stylistically unconventional.
*   **Vocabulary Matching:** If the profile says the user says "说白了" instead of "总而言之", the AI must make that substitution.
*   **Tone Masking:** The final output must not sound like a generic human; it must sound like *this specific human*.

## Example Output

**[Stylometry Profile Example]**
*   **Quirks:** Frequently uses em-dashes (—) instead of commas for parenthetical thoughts. Starts paragraphs with "Look," or "Honestly,".
*   **Code:** Prefers early returns. Uses `idx` and `res`. Leaves lowercase `// todo:` comments without punctuation.

**[Cloned Rewrite Output]**
> Look, the logic here is pretty straightforward—we just iterate through the array and early return if we hit a null.
>
> ```javascript
> function processData(arr) {
>    for (let idx = 0; idx < arr.length; idx++) {
>        if (!arr[idx]) return null; // todo: check if we need to throw an error instead
>        // ...
>    }
> }
> ```
