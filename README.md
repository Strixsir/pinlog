# PinLog

A private diary for TRT. Tick off each dose in one tap, see what's due and what you've taken each day, rotate injection sites, track your supply, keep notes, and follow your weight and bloodwork.

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

The layout follows the pattern food diaries such as Cronometer made familiar: a dark menu on the left, the day in the middle, and a calendar and quick facts on the right. On a phone the menu moves to the bottom bar and the side cards follow the day.

**Diary: what did I take, and what's left?**
- The arrows at the top (or the calendar on the right) move between days. Every day uses the same layout, so going back to yesterday to add something you forgot works exactly like today.
- Four buttons add to the day you're looking at: **Dose**, **Body** (weight and other measurements), **Bloodwork** and **Note**. On a past day they use that date.
- When something is due, a strip at the top shows how much to draw and which site to use, with **Log it** and **Skip**.
- Entries are grouped into Morning, Afternoon, Evening and Other. Each band header totals what you took in it, for example "500 mg Test C • 1 to go". Every row shows the time, the amount and unit, and the volume.
- Tap a circle to log a dose. On a past day, a dashed circle marks a dose that wasn't logged; tap it to log it at its scheduled time. Tap a name to change the dose, site, time or notes.
- **Dose summary** shows three rings: doses taken, planned and remaining. **Amounts** sets each compound against your plan, for the day or the whole week, for example "500 / 250 mg, 250 mg over plan".
- **On-schedule scores** shows the share of planned doses you logged in the last 30 days, for all compounds together and for each one.
- **Plot my levels** draws estimated levels for the injected esters in your plan, right on the page. **Adjust in plotter** opens the full plotter.
- **This week** is a grid of amounts per day. Tap a day to open it.
- On the right: a month calendar (days with entries are tinted), your next injection site, supply left, and your latest weight and bloodwork.

**Notes.** Write how you feel, side effects or questions for your doctor. Quick-add phrases ("Pin pain", "Poor sleep", "Acne") make it one tap. Notes show in the diary at the time you wrote them and are included in backups.

**Levels plotter** (Tools). Pick an ester (testosterone cypionate, enanthate, propionate or undecanoate, nandrolone decanoate, one of your own compounds, or any half-life you enter), a dose and how often, then tap **Plot**. It shows when levels settle, the highest and lowest point between doses, and how big the ups and downs are. Add lines to compare. Short-acting things like oral tablets and GH are left out of the plan plot because they clear within hours. It's a model from approximate half-lives, not a blood test and not dosing advice.

**Calendar: what happened when?** Month view with dots, or a list of every entry. Each day shows totals per compound ("Testosterone Cypionate: 500 mg in 2 doses").

**My compounds: what am I on?**
- **Add**: four short steps. What is it (search the list or type any name to create your own), how you take it, how much, how often. Strength and supply are optional prompts at the end.
- Tap a compound to see its schedule, supply ("35 doses left"), recent doses and details, with an Edit button on each.
- Schedules support extra daily times, start and end dates, pausing and dose steps (titration), under **More options**.

**Progress: how am I doing?** % of planned doses taken, latest bloodwork, a weight chart with an optional goal, and estimated levels from what you actually logged. **All measurements** opens body fat, lean mass, waist, resting heart rate and blood pressure.

**Tools and More**: levels plotter, injection sites (turn off ones you don't use, add your own by tapping the body), a calculator (how much to draw, mixing vials, nmol/L ↔ ng/dL), backup and restore, calendar reminders, spreadsheet export and preferences.

## Privacy

There is no tracking, analytics or server. The only outside request is for the Rubik font from Google Fonts; if it's blocked, the app uses your device's normal font.

PinLog is a personal record, not medical advice. Doses and schedules come from you and your doctor. Half-life values are approximate published figures you can edit, and level curves and the plotter are rough estimates.
