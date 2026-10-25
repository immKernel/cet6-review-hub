# GitHub Copilot Repository Instructions

Follow the canonical instructions in the repository root [AGENTS.md](../AGENTS.md) before editing this CET-6 review website.

- Keep **one** `index.html`-based study site with unified reading, vocabulary, grammar, quiz, and review sections. Never create a separate lesson site by default.
- Append all new words and options (including distractors) to the **single** `wordbank`; deduplicate existing entries, preserve existing numerical word IDs and mastery flags, and keep the default "all words" view across all exam sets.
- Integrate new articles into `articles`, grammar into `grammar`, and all quiz items into the unified `allQuizzes` workflow. Internal quiz IDs must be globally unique across papers.
- Preserve existing browser progress at `cet6_reading_lab_v1`, including import/export compatibility.
- Before committing, test UI flows for old and new study material, word search/cards/mastery, quiz scoring, and progress persistence.

For details and edge cases, read **AGENTS.md** in full.
