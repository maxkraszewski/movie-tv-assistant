# TV Show Examples

These examples show exact input → output pairs. Follow the format precisely.

---

## Example 1: Title in another language

**Input:**
```
TV: El hombre infiltrado
```

**Output:**
````
```
TV SHOW NAME: A MAN ON THE INSIDE
GENRE: COMEDY, DRAMA
CAST: TED DANSON, MARY ELIZABETH ELLIS, STEPHANIE BEATRIZ
SEASONS AND EPISODES:
- Season 1: 8 episodes (November 21, 2024)
- Season 2: 8 episodes (Expected in 2025)
PLATFORM: NETFLIX
```
````

Note: Spanish title is translated to the official English title. Season 2 uses "Expected"
since it hasn't aired yet.

---

## Example 2: Multi-season show

**Input:**
```
TV: Slow Horses
```

**Output:**
````
```
TV SHOW NAME: SLOW HORSES
GENRE: ESPIONAGE, DRAMA, BLACK COMEDY
CAST: GARY OLDMAN, JACK LOWDEN, KRISTIN SCOTT THOMAS
SEASONS AND EPISODES:
- Season 1: 6 episodes (April 1, 2022 – April 29, 2022)
- Season 2: 6 episodes (December 2, 2022 – December 30, 2022)
- Season 3: 6 episodes (November 29, 2023 – January 3, 2024)
- Season 4: 6 episodes (September 4, 2024 – October 9, 2024)
PLATFORM: APPLE TV+
```
````

Note: Each season has its own line with episode count and full date range.

---

## Example 3: Show with single premiere date per season

**Input:**
```
TV: Severance
```

**Output:**
````
```
TV SHOW NAME: SEVERANCE
GENRE: DRAMA, SCIENCE FICTION, THRILLER
CAST: ADAM SCOTT, BRITT LOWER, PATRICIA ARQUETTE
SEASONS AND EPISODES:
- Season 1: 9 episodes (February 18, 2022 – April 8, 2022)
- Season 2: 10 episodes (January 17, 2025 – March 21, 2025)
- Season 3: Renewed
PLATFORM: APPLE TV+
```
````

Note: Season 3 is confirmed but has no date — listed as "Renewed" without inventing dates.

---

## Key Takeaways from Examples

- Non-English titles are always converted to the official English title.
- Season dates use the format: `Month Day, Year – Month Day, Year` for ranges.
- Upcoming seasons: use "Expected in [year]" if a year is known, or "Renewed" if only
  renewal is confirmed.
- Every season is listed, no matter how many.
- The dash-space prefix (`- `) is required for every season line.
