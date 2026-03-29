# Changelog

## 2026-03-29

### Changed
- Output is now wrapped in a fenced code block (triple backticks) — the entire response is just the code block, nothing else.
- Added prominent "Output Rule" section at the top of SKILL.md to prevent Claude from adding preamble, narration, or sign-off text around the card.
- Strengthened "Core Rules" and "What NOT to Do" sections with explicit examples of unwanted commentary (e.g., "Here's the info…", "Pulling information…").
- Rewrote `references/formats.md` templates using indented code blocks to avoid confusing nested backtick parsing.
- Updated all examples in `examples/movies.md` and `examples/tvshows.md` to label outputs as "Complete response" — reinforcing that the code block is the entire response.

## 2026-03-22

### Initial release
- Movie and TV show structured information cards.
- Uppercase-styled formatting for titles, actors, and genres.
- Streaming platform lookup for Argentina.
- Title normalization (misspellings, non-English titles, subtitles).
- Disambiguation flow for ambiguous titles.
- Reference-based architecture with formats, streaming, disambiguation, and examples.
