# YearGlance

A single-file event calendar that shows your entire year at a glance. No installation, no server, no dependencies — just open the HTML file in a browser.

![YearGlance Calendar](screenshot.png)

## Features

- **Full year view** — all 12 months visible at once in a compact grid
- **Month expand** — click any month header for a full weekly grid view
- **Event management** — add, edit, and delete events via a clean modal
- **Recurring events** — weekly, monthly, or yearly repeat; delete future occurrences without affecting past ones
- **Event colours** — 11 flat colours (Google Calendar palette)
- **Categories** — Meeting, Food, Call, Travel, Birthday, Reminder, Payment
- **National holidays** — select your country to overlay public holidays (powered by [Nager.Date](https://date.nager.at))
- **Upcoming events strip** — next 7 days shown below the toolbar with day counters
- **ICS export / import** — compatible with Google Calendar, Apple Calendar, Outlook
- **Dark mode** — charcoal theme, toggle in the toolbar
- **Colour / grayscale toggle** — switch between coloured and monochrome event display
- **Drag to reschedule** — drag a day to move its events to another date
- **Year navigation** — browse any year; events are stored per date so years are naturally separate
- **Past day shading** — past days are visually dimmed and read-only
- **Today highlight** — current day outlined in accent colour
- **Fully offline** — events saved to browser `localStorage`; no account or server needed

## Usage

Download `calendar.html` and open it in any modern browser. That's it.

```bash
git clone https://github.com/ib-ra/yearglance.git
cd yearglance
open calendar.html
```

All events are saved automatically in your browser's local storage. Use **Export .ics** to back up your data or move it to another device.

## Import from another calendar

Any `.ics` file exported from Google Calendar, Apple Calendar, or Outlook can be imported directly. Click **Import .ics** and select the file.

## Tech

- Vanilla HTML, CSS, and JavaScript — no frameworks, no build step
- `localStorage` for persistence
- [Nager.Date API](https://date.nager.at) for public holidays (fetched once per country/year, cached locally)
- iCalendar (RFC 5545) for export and import

## Browser support

Works in all modern browsers: Chrome, Firefox, Safari, Edge.

## License

MIT — see [LICENSE](LICENSE)
