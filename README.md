# The Awards Watch

A cinematic, static awards-season dashboard hosted on GitHub Pages, with publicly shared viewing reactions and a subscribable Canadian release calendar.

## Content standards

- Film awards tiers are **provisional editorial tracking labels**, not verified award nominations or probability forecasts.
- The current roster is a curated starting set, not a claim of 15 Oscar and 24 Emmy contenders.
- Dates are omitted until checked against Canadian distributors, exhibitors, or streaming platforms.
- Poster and promotional images are now linked from public studio, distributor, and entertainment-media sources; source names and URLs are recorded in `data.json` and listed on `credits.html`. Abstract typographic artwork remains as a loading/error fallback. The hero uses an externally hosted cinema photograph.
- Artwork can break if its origin stops serving the image. This first implementation does not use the TMDB API; **no API key is included in this repository or website**. TMDB image-path integration is a possible future improvement using a private GitHub Actions secret.
- The owner's reactions are intentionally public; each visitor's watchlist checkboxes are local browser storage only.

## Deployment

GitHub Pages: main branch, repository root. No Netlify, build tools, database, API keys, tracking scripts, or paid dependencies.

## Release feed

The initial releases.ics is empty but valid. Update it and data.json together when confirmed Canadian dates become available. Use stable UID values and all-day DTSTART;VALUE=DATE and exclusive DTEND;VALUE=DATE. Google Calendar controls feed refresh frequency.

The scheduled ChatGPT monthly Awards Watch report does not automatically commit website changes.
