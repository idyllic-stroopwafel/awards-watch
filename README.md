# The Awards Watch

A cinematic, static awards-season dashboard hosted on GitHub Pages, with publicly shared viewing reactions and a subscribable Canadian release calendar.

## Content standards

- Film awards tiers are **provisional editorial tracking labels**, not verified award nominations or probability forecasts.
- The current roster is a curated starting set, not a claim of 15 Oscar and 24 Emmy contenders.
- Dates are omitted until checked against Canadian distributors, exhibitors, or streaming platforms.
- The poster-like gradients are **original abstract typographic artwork**, not official film or TV posters. The hero uses an externally hosted cinema photograph.
- The owner's reactions are intentionally public; each visitor's watchlist checkboxes are local browser storage only.

## Deployment

GitHub Pages: main branch, repository root. No Netlify, build tools, database, API keys, tracking scripts, or paid dependencies.

## Release feed

The initial releases.ics is empty but valid. Update it and data.json together when confirmed Canadian dates become available. Use stable UID values and all-day DTSTART;VALUE=DATE and exclusive DTEND;VALUE=DATE. Google Calendar controls feed refresh frequency.

The scheduled ChatGPT monthly Awards Watch report does not automatically commit website changes.
