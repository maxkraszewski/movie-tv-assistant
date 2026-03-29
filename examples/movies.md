# Movie Examples

These examples show exact input → output pairs. The output is the COMPLETE response —
a code block and nothing else.

---

## Example 1: Simple title

**Input:** `Movie: Gifted`

**Complete response:**

    ```
    MOVIE NAME: GIFTED
    GENRE: DRAMA
    CAST: CHRIS EVANS, MCKENNA GRACE, OCTAVIA SPENCER
    RELEASE YEAR: 2017
    PLATFORM: NETFLIX
    ```

---

## Example 2: Title with subtitle and minor misspelling

**Input:** `Movie: SpiderMan: Across the spiderverse`

**Complete response:**

    ```
    MOVIE NAME: SPIDER-MAN: ACROSS THE SPIDER-VERSE
    GENRE: ANIMATION, ACTION, ADVENTURE
    CAST: SHAMEIK MOORE, HAILEE STEINFELD, JAKE JOHNSON
    RELEASE YEAR: 2023
    PLATFORM: DISNEY+
    ```

---

## Example 3: Misspelled title

**Input:** `Movie: Tripl fronter`

**Complete response:**

    ```
    MOVIE NAME: TRIPLE FRONTIER
    GENRE: ACTION, ADVENTURE, THRILLER
    CAST: BEN AFFLECK, OSCAR ISAAC, CHARLIE HUNNAM
    RELEASE YEAR: 2019
    PLATFORM: NETFLIX
    ```

---

## Example 4: Single genre

**Input:** `Movie: Gifted`

Note: "Gifted" has only one primary genre (DRAMA). Do not pad with extra genres — list
only what is accurate.

---

## Key Takeaways from Examples

- The code block IS the entire response. No text before or after it.
- Subtitles are always included if part of the official name.
- Misspellings are silently corrected.
- Genres can be 1, 2, or 3 — never force exactly 3 if the movie doesn't warrant it.
- Platform reflects Argentina availability at time of lookup.
