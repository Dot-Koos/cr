# Hilze Strauss · Conscious Relationships

Website for Imago Couples Intensives in Namibia and online.

## Pages

| File | Page |
|---|---|
| `index.html` | Home page: the intensive, world map, approach, pricing, online intensive, FAQ, enquiry form |
| `space.html` | The in-person space: photo gallery and details |
| `sessions.html` | Sessions and fees: the intensive, observed session and private session, with hourly rates |

Each page is self-contained: its styles and scripts are inside the HTML file.

## Images (`images/` folder)

| File | Used for |
|---|---|
| `logo-full.png` | Footer logo |
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

- **Enquiry email:** in `index.html`, find `const ENQUIRY_EMAIL = "";` and put the email address between the quotes to switch on the "Open in email" button.
- **Map pins:** in `index.html`, each pin has `--x` and `--y` percentages. Nudge these to move a pin.
- **Prices:** search the HTML files for the amount (for example `R16,999`) and change every occurrence.
