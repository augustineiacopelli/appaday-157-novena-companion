# Novena Companion

**AppADay Day 157** | Category S, Spirituality | Claude API: No

Live: https://augustineiacopelli.github.io/appaday-157-novena-companion/
Portfolio: https://augustineiacopelli.github.io/appaday/

Novena Companion walks you through a nine day Catholic novena. Pick a devotion, name your intention, and come back each day for that day's meditation, the traditional prayers, and a closing prayer. A nine dot progress row shows which days you have prayed, which you missed, and which are still ahead, alongside your current day, days remaining, and streak.

## The novenas

Seven built in novenas are included: the Holy Spirit (the seven gifts), Divine Mercy (a different group of souls each day), St. Jude, St. Joseph, Our Mother of Perpetual Help, the Miraculous Medal, and the Immaculate Conception. Each has nine themed days and its own closing prayer, worded to be prayed on any day; on Day 9 it gains a concluding line that gives thanks for the nine days and entrusts the intention to God.

A Custom Novena follows a nine day arc of Trust, Surrender, Patience, Humility, Perseverance, Hope, Charity, Peace, and Gratitude, with your intention woven into each day's meditation. An intention is required for the custom novena and optional for the others, and is limited to 140 characters.

The Custom Novena can also carry your own prayers, such as the text of a prayer card or a parish novena booklet. When you choose Custom Novena, the start box has a field right under your intention to type or paste the prayer you will pray each day. Add more prayers, or a prayer for one day only, from the gear menu or from the Your prayers card on any custom novena day. Each prayer has an optional title, up to 2,000 characters of text with line breaks kept, and a schedule of every day or a single day from 1 to 9. Prayers appear open beneath that day's meditation, can be edited or deleted at any time (deleting asks first), and stay saved for future custom novenas. Up to 12 prayers can be kept.

## How it works

The novena starts on the day you begin it. Day numbers are computed from local calendar dates, so they stay correct across daylight saving time changes. Tap any past dot to read that day again and mark it prayed after the fact; future days stay locked. The streak counts consecutive prayed days ending today, or ending yesterday if today is not yet marked. Marking the last of the nine days opens the completion screen and adds one to your lifetime count of completed novenas. If nine days pass without finishing, the app moves to a summary showing how many days were prayed.

Ending a novena early or erasing all data asks for confirmation in an in-app dialog.

## Traditional dates

Each built in novena shows when it is traditionally prayed and the next upcoming window, or flags it as in season now. The picker lists the novenas in order of their next traditional start, recalculated each time the app opens. Custom Novena leads the list, except while a traditional window is in season, when that novena moves to the top and Custom drops to the end. The Holy Spirit novena runs from the Friday after Ascension Thursday to the eve of Pentecost and Divine Mercy from Good Friday to the eve of Divine Mercy Sunday, both computed from the date of Easter each year. The rest end on the eve of a fixed feast: St. Joseph (March 10 to 18), Perpetual Help (June 18 to 26), St. Jude (October 19 to 27), Miraculous Medal (November 18 to 26), and the Immaculate Conception (November 29 to December 7).

## Calendar reminders

The gear in the header opens Settings, which holds Calendar reminders and Custom novena prayers. Pick a daily time (no earlier than 6:30 AM) and either download an .ics file or add a repeating event to Google Calendar.

The .ics file holds one private, 15 minute event with an on time alert for each remaining day of the novena. It opens directly in Outlook and Apple Calendar and imports into Google Calendar. Each event links to its own day in the app, for example `#novena=st-jude&day=4`, so tapping the link opens that day's meditation ready to pray. Times are written in your device's time zone. For America/Chicago the file carries a full VTIMEZONE with both the CDT and CST rules, so reminders stay at the same wall clock time across the daylight saving change; other US zones get the same rules with their own offsets, zones without daylight saving get a fixed offset, and anything else falls back to floating local times.

Google's quick add link creates a single daily repeating event for the remaining days that links to the novena and opens whatever day is current.

A deep link for a novena that is not active on the current device preselects that novena on the picker.

## Content

The Our Father, Hail Mary, and Glory Be are the traditional public domain texts. Every meditation and closing prayer was written originally for this app; no published novena booklet or Divine Mercy diary text is reproduced.

## Data

Everything is stored in your browser under the single localStorage key `appaday157_novena`, holding the active novena (devotion, intention, start date, nine prayed flags), the completed count, your reminder time, and your custom prayers. Nothing leaves your device. Use Reset all data in the footer to clear it.

## Build

A single self-contained `index.html` with inline CSS and JavaScript and no external dependencies. Saved to a phone home screen, it launches full screen with its own icon.
