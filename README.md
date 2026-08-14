# Waterfaller

A single-file schedule viewer for the ZIS 2026/27 **Days 1–8** waterfall rotation. Name
your eight blocks and it lays out every teaching day of the year with the right courses
in the right periods.

## Running it

Open `index.html` in a browser. No build step, no dependencies, no server. It works
offline, and everything you enter stays in your own browser.

## Setting it up

**Your blocks.** Type a course name beside each block number. Blocks you leave empty
stay off the calendar. They're grouped odd and even because a day only ever draws from
one group, starting at the block its number names.

**ET** adds a separate Extended Time slot before the day's first lesson. It can only
fall on days that open with that block, and never on a Wednesday.

**Period times** are editable, with a second set for the Wednesday late start. Lunch is
worked out from the gap between periods 2 and 3.

**Standing commitments** — Faculty Time, Flexible Time and the two Advisory slots — are
checkboxes. The *only on days I teach* switch hides them on any day where none of the
blocks are yours.

## The views

- **Calendar** — every month, Monday to Friday, each school day showing its rotation
  number and your lessons in period order. Breaks and days marked 0 are labelled in
  place. Click a day to see its times.
- **8-day cycle** — the rotation as a grid, showing each course sliding one period
  earlier each time it comes round, with a lesson count for the year.
- **Print** — one month per page, with the controls stripped out.

## Exporting to your calendar

**Export** lets you pick which courses and commitments to include, and whether to get
one combined file or one file per item.

An `.ics` file always imports into exactly one calendar, so to switch subjects on and
off independently in Google Calendar you need one file each:

1. Tick the items you want and choose **One file per item**.
2. In Google Calendar, create a calendar per subject under *Other calendars → Create
   new calendar*.
3. Import each file under *Settings → Import & export*, choosing the matching calendar
   as the destination each time.

Your browser will ask permission to download several files at once.
