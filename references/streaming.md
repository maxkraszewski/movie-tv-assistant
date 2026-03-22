# Streaming Platform Lookup

## Target Region

Always look up streaming availability for **Argentina**. If Argentina-specific data is
not available, omit the PLATFORM field entirely rather than showing another region's data.

## Search Strategy

After building the rest of the card, run a separate search:
```
[title] streaming Argentina [year]
```

Reliable sources for streaming availability:
- JustWatch (justwatch.com/ar)
- Google search knowledge panels
- Platform-specific sites (netflix.com, etc.)

## Platform Name Formatting

Always use these short names in UPPERCASE:

| Platform | Display as |
|----------|-----------|
| Netflix | NETFLIX |
| Disney+ / Disney Plus | DISNEY |
| Amazon Prime Video | AMAZON |
| Apple TV+ | APPLE |
| HBO Max / Max | MAX |
| Paramount+ | PARAMOUNT |
| Star+ | STAR |
| Crunchyroll | CRUNCHYROLL |

## Rules

- List only the **primary** platform where the content is available for streaming
  (subscription-based). Rental-only or purchase-only does not count.
- If available on multiple platforms, pick the most prominent one.
- If no subscription streaming is available in Argentina, omit the PLATFORM line entirely.
- Never write "N/A", "Not available", or similar — just omit the line.
