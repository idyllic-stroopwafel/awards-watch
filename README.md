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

`releases.ics` is a populated, public iCalendar subscription feed; `data.json` contains the matching upcoming Canadian release events and their source URLs. Keep both in sync on every weekly update. Use stable UIDs, UTC DTSTAMP, all-day DTSTART;VALUE=DATE, and exclusive next-day DTEND;VALUE=DATE. Do not add unsourced dates or misrepresent North American dates as confirmed Canadian releases.

Subscription URL: `https://idyllic-stroopwafel.github.io/awards-watch/releases.ics`. Apple Calendar can use `webcal://idyllic-stroopwafel.github.io/awards-watch/releases.ics`. Google Calendar supports Other calendars → From URL. A downloaded `.ics` is a one-time import, not a live subscription. Client refresh frequency is controlled by the calendar provider. The weekly Awards Watch & Site Update automation is instructed to maintain both the site and calendar feed.
