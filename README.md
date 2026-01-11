SPDX-License-Identifier: CC-BY-4.0

# Adventure Builder Adventures

This repo contains kid-friendly Adventure Builder adventures and notes for extracting example adventures from the cached rulebook PDF. It’s meant to help Guides quickly spin up new, non-violent adventures for ages 6–12.

## What’s Here
- `cache/Adventure_Builder_A_Family_Roleplaying_Game.pdf`: source PDF with four example adventures (copyrighted, not stored in git).
- `adventures/`: new adventures written in the same structure.
- `AGENTS.md`: repeatable instructions for extraction and creation.

## Getting the Game
- Boxed set (physical): https://www.widerpathgames.com/collections/adventure-builder
- PDF/print-and-play: https://www.drivethrurpg.com/en/product/359850/adventure-builder-a-family-roleplaying-game
- Publisher store: https://www.widerpathgames.com/collections/adventure-builder

## Adventure Structure
Each adventure follows the same format:
- Adventure Hook
- Story Card 1
- Story Card 2
- Story Card 3
- Conclusion

Each section includes a clear goal to guide the story forward.

## Extracting the Example Adventures
Place a legally obtained PDF at `cache/Adventure_Builder_A_Family_Roleplaying_Game.pdf`. The `cache/` folder is gitignored because the PDF is copyrighted.

The cached PDF contains four sample adventures in Chapter 4:
- The King is Missing
- The Dragon and the Talking Pig
- Captain No‑Beard’s Fishy Treasure Map
- Wayzle’s Puzzle Door

To extract text:

```
mutool draw -F text "cache/Adventure_Builder_A_Family_Roleplaying_Game.pdf"
```

Locate the Adventure Hook, Story Cards 1–3, and Conclusion for each adventure. Watch for placeholders like `(candy name)`.

## Creating New Adventures
- Keep language playful, simple, and flexible for a Guide to improvise.
- Emphasize non‑violent, creative solutions.
- Favor fantastical or animal-friendly themes when requested.
- Include a short “Guide Notes” section with trait ideas.

## Using Adventures
Choose any adventure in `adventures/`, read the hook aloud, then reveal the story cards as players find story cards in their deck. Use creature/encounter cards to fill in the action between story beats.

## Generating Adventures with OpenCode
OpenCode is the terminal-based coding agent used to extract the examples and draft new adventures. Clone the repo locally before you start.

1. Install OpenCode: https://opencode.ai
2. Clone this repo and open a terminal in the repo root.
3. Start an OpenCode session in this repo.
4. Ask it to extract the Chapter 4 samples from the cached PDF.
5. Ask it to draft a new adventure using the same structure and save it under `adventures/`.

Example prompts:
- "Extract the four example adventures from the cached PDF in `cache/`."
- "Write a new adventure for ages 6–9 with fantastical animals, then save it as a Markdown file in `adventures/`."

## Licensing
Adventure text in this repo is licensed under Creative Commons Attribution 4.0 (`LICENSE-CC-BY-4.0.md`). Any code or tooling is licensed under the MIT License (`LICENSE-MIT`).

## Contributing
Adventure PRs are welcome. By submitting a contribution, you agree that your adventure text is licensed under CC BY 4.0 and that you have the right to license it under those terms.

Add new adventures as Markdown files in `adventures/`, using the standard structure above.
