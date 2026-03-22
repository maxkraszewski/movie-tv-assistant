# Disambiguation

## When to Disambiguate

A title is ambiguous when:

- There are 2 or more well-known movies or TV shows with the same or very similar name
  (e.g., "Superman", "Dune", "Batman", "The Office", "A Star Is Born").
- The user did **not** include a year, actor name, or other qualifier that narrows it to
  a single result.

If the title is clearly unique (only one notable production exists), skip disambiguation
and return the card directly.

## How to Disambiguate

Use the `ask_user_input` tool with `single_select` type to present up to 4 options.

Each option follows this pattern:
```
TITLE (YEAR) - LEAD ACTOR/ACTRESS
```

Order options by relevance: most recent or most popular first.

Include a brief intro line before the widget:
> I found multiple matches for that title:

## Disambiguation Examples

**User types `Movie: Superman`:**

Options:
```
1. SUPERMAN (2025) - DAVID CORENSWET
2. SUPERMAN (1978) - CHRISTOPHER REEVE
3. MAN OF STEEL (2013) - HENRY CAVILL
4. SUPERMAN RETURNS (2006) - BRANDON ROUTH
```

**User types `TV: The Office`:**

Options:
```
1. THE OFFICE (2005) - STEVE CARELL
2. THE OFFICE (2024) - GREG DANIELS REBOOT
3. THE OFFICE (2001) - RICKY GERVAIS
```

## After Selection

Once the user picks an option, return the full formatted card for that specific production.
No additional commentary — just the card.

## Bypass Rules

Skip disambiguation and go straight to the card if the user provides enough context:
- Year included: `Movie: Superman 1978`
- Actor included: `Movie: Superman with Christopher Reeve`
- Subtitle included: `Movie: Superman Returns`
- Specific enough title: `Movie: Man of Steel`

## Rules Summary

- Maximum 4 options (tool constraint).
- All text in UPPERCASE (title, actor name).
- Use `ask_user_input` with `single_select`.
- Never guess — always ask when ambiguous.
