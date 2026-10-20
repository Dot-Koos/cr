# Hilze Strauss · Conscious Relationships

Website for Imago Couples Intensives in Namibia and online.

## Pages

| File | Page |
|---|---|
| `index.html` | Home page: the intensive, world map, approach, pricing, online intensive, FAQ, enquiry form |
| `space.html` | The in-person space: photo gallery and details |
| `sessions.html` | Sessions and fees: the intensive, observed session and private session, with hourly rates |
| `book.html` | Enquire: choose online, in-person intensive or single session, then days, dates and send a booking request |

Each page is self-contained: its styles and scripts are inside the HTML file.

## Images (`images/` folder)

| File | Used for |
|---|---|
| `logo-full.png` | Footer logo (birds artwork, no lettering) |
| `hero-art.png` | Large birds artwork at the top of the home page |
| `logo-mark.png` | Header logo (the birds) |
| `favicon.png` | Browser tab icon |
| `world-map.jpg` | "Connection, across continents" map |
| `space-1.jpg` to `space-5.jpg` | Photos on the Space page (add these when ready) |

File names are case-sensitive on GitHub Pages: `space-1.jpg` works, `Space-1.JPG` does not.

## Publishing (GitHub Pages)

1. Create a **Public** repository on github.com.
2. Upload these files, keeping the `images` folder.
3. **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After a minute or two the site is live at `https://<your-username>.github.io/<repository-name>/`.

## Making changes

Edit a file on GitHub (pencil icon) or upload a replacement, then commit. The live site updates within a minute or two.

## Common edits

- **Booking requests:** open `book.html` and find the `CONFIG` settings near the bottom. Fill in ONE of:
  - `formEndpoint`: a free Formspree form URL (create a form at formspree.io with Hilze's email). Requests then arrive in her inbox automatically. **Recommended.**
  - `email`: Hilze's email address. The visitor's email app opens with the request filled in.
  - If both are empty, visitors are shown their request to copy and send themselves.
- **Unavailable dates:** in the same `CONFIG`, add dates to `unavailable` as `"YYYY-MM-DD"`. Any week touching those dates is shown as unavailable.
- **Single-session times:** change `times` (the start times people can tick) and `sessionWindow` in `CONFIG`. Currently 08:00 – 13:00.
- **Booking prices:** the `PRODUCTS` list just below `CONFIG` holds the prices used on the booking page.
- **Reviews:** in `index.html`, find `<!-- REVIEWS -->`. Each review is one `<figure class="review placeholder">` in the sliding row. Replace the text in `<blockquote>` with the real review and remove the word `placeholder` from its class. To add a review, copy a whole `<figure>…</figure>` block; to remove one, delete it. The sliding loop adjusts by itself. Only use reviews you have permission to share.
- **Map pins:** in `index.html`, each pin has `--x` and `--y` percentages. Nudge these to move a pin.
- **Prices:** search the HTML files for the amount (for example `14,999` or `22,999`; all prices are in NAD) and change every occurrence, including the hourly rates next to them (fee ÷ 15 hours).
