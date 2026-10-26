# PinLog

A private dose log for TRT. Tick off each dose in one tap, see what's due, rotate injection sites, track your supply, and follow your weight and bloodwork.

Everything is saved in the browser of the device you use. There is no server, no account, and nothing is uploaded. Each person who opens the link gets their own separate log on their own phone or computer, and it is still there when they come back.

## What's in this folder

| File | What it does |
|---|---|
| `index.html` | The whole app |
| `manifest.webmanifest` | Lets it install as an app on phones and computers |
| `sw.js` | Lets it open without internet after the first visit |
| `icon.svg`, `icon-192.png`, `icon-512.png` | App icons |

## Put it online with GitHub Pages (free, about 5 minutes)

1. Sign in at [github.com](https://github.com) (create a free account if you need one).
2. Click **+** at the top right, then **New repository**.
   - Name it something like `pinlog`.
   - Set it to **Public** (free GitHub Pages needs a public repository; only the app's code is in it, never anyone's log).
   - Click **Create repository**.
3. On the new repository page, click **uploading an existing file**.
   Drag in all the files from this folder (not the folder itself) and click **Commit changes**.
4. Go to **Settings**, then **Pages** in the left menu.
   Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose branch **main** and folder **/ (root)**, and click **Save**.
5. Wait a minute or two and refresh the page. GitHub shows your link, which looks like:

   `https://YOUR-USERNAME.github.io/pinlog/`

That link is what you open yourself and what you send to your friend.

## Sharing it

Send the link. When your friend opens it:

- He gets an empty log of his own. He can't see yours and you can't see his.
- Whatever he logs is saved on his phone or computer and is still there next week.
- The data belongs to that one browser on that one device. If he opens the link on a different phone, that's a separate, empty log.

Tell him to do two things once:

1. **Install it.** On iPhone, open the link in Safari, tap **Share**, then **Add to Home Screen**. On Android or in Chrome/Edge on a computer, use the install icon in the address bar (or **More → Install as an app** inside PinLog). On iPhone this matters: Safari can clear data for websites that haven't been opened in 7 days, but apps added to the Home Screen are kept.
2. **Download a backup now and then** (More → Back up). It's a small file that restores everything if the browser is ever cleared or he changes phones (More → Restore from a backup).

## Updating the app later

Upload the new files to the same repository (Add file → Upload files, then commit), replacing the old ones. Everyone's logs stay as they are and are upgraded automatically; they get the new version the next time they open it with internet.

## Using it

Five places, each answering one question.

**Today: what do I take now?**
- The ring at the top shows how much of today is done.
- **Next up** shows the next dose large: how much, how much to draw, which site. Tap **Log it**, or **Skip**.
- Everything else due today is a checklist. Tap the circle when you take it. Tap the name to change the dose, site, time or notes.
- **This week** shows planned doses as dots. Tap a day to open it in the calendar.
- **At a glance**: four tiles, one number each: weight, doses of supply left, % on schedule, days since bloodwork.

**Calendar: what happened when?** Month view with dots, or a list of every entry. Tap any entry to edit or delete it.

**Compounds: what am I on?**
- **Add**: four short steps. What is it (search the list or type any name to create your own), how you take it, how much, how often. Strength and supply are optional prompts at the end.
- Tap a compound to see its schedule, supply ("35 doses left"), recent doses and details, with an Edit button on each.
- Schedules support extra daily times, start and end dates, pausing and dose steps (titration). These sit under **More options** so they stay out of the way.

**Progress: how am I doing?** One scroll of cards: % of planned doses taken, latest bloodwork, a weight chart with an optional goal, and estimated levels. **All measurements** opens body fat, lean mass, waist, resting heart rate and blood pressure.

**More**: injection sites (turn off ones you don't use, add your own by tapping the body), a calculator (how much to draw, mixing vials, nmol/L ↔ ng/dL), backup and restore, calendar reminders, spreadsheet export and preferences.

## Privacy

There is no tracking, analytics or server. The only outside request is for the IBM Plex fonts from Google Fonts; if it's blocked, the app uses your device's normal font.

PinLog is a personal record, not medical advice. Doses and schedules come from you and your doctor. Half-life values are approximate published figures you can edit, and level curves are rough estimates.
