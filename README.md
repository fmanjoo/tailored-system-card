# System cards for broader audiences

A working prototype exploring how AI **system cards** could be made legible to the people a model actually affects — and auditable by the people who hold the lab to account. Built on one real section of a real card: the cybersecurity capability material from OpenAI's [GPT-5.6 Preview System Card](https://deploymentsafety.openai.com/gpt-5-6-preview) (June 26, 2026).

**Live page:** https://fmanjoo.github.io/tailored-system-card/

## The problem

The 2018 paper that proposed model cards imagined "one to two page" documents that would help readers "quickly grasp" a model's capabilities and dangers. In the years since, the models — and all the ways they can be used and misused — have been supersized, and the cards have grown with them, into dense documents that almost no one reads end to end. The usual fix, an executive summary, only moves the problem: a summary you can't check asks for trust instead of delivering transparency.

## Two ideas

The prototype is written in the card's own first-person voice, as a demonstration of what a lab could publish. It offers two things:

1. **A tabbed explainer for specific use cases.** The same material, retold for a local official, a small-business owner, and a school-district IT lead — each naming the risks the model poses to *that* reader and, crucially, what they can do about them. Every underlined claim opens the verbatim source passage it came from, so the compression is auditable, not just trusted.
2. **An invitation to challenge the card with rival models.** A panel where a frontier model the lab didn't build flags the card's own blind spots, and a box that hands the card (or your own question) to a different company's AI for adversarial review — because you shouldn't have to take the lab's word, or its own model's, for any of it.

## What's real and what isn't

- The verbatim source passages behind every receipt are quoted from OpenAI's published card (© OpenAI, reproduced for commentary and demonstration).
- The three explainer layers are original prose written as examples; each claim maps to the source paragraphs that license it, checked by an AI fidelity pass that flags any sentence it cannot ground.
- The "what we might have missed" list is an illustrative pass by a frontier model, shown to demonstrate the feature.
- The interrogation tools build a prompt and hand it to the reader's own AI — the page runs no model and stores no key, so it can't certify answers, only ground and cite them.
- This is a **personal prototype accompanying a job application. It is not affiliated with, or endorsed by, OpenAI.** The first-person voice is a demonstration of what the lab could publish, not a statement by OpenAI.

## Implementation

One self-contained HTML file. No build step, no dependencies, no external requests, no analytics. System font stacks only. Light and dark themes, keyboard-navigable, degrades to stacked plain text without JavaScript.
