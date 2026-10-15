# Innologic website

Two designs of the same site. Each is **one file**, with no build step and no external scripts or fonts, so it loads fast and works anywhere.

| File | Look |
|---|---|
| `index.html` (option A) | Dark blue and teal, modern and technical. Feature cards, a one-sale flow card, FAQ. |
| `option-b.html` (option B) | Warm cream and green with orange, serif headlines, friendlier. A picture of the app with sample numbers, a day-in-your-business timeline, tabs for features, an honest comparison table, FAQ. |

Pick one. To publish it, save your choice under the name `index.html` (so option B becomes `index.html` and A is set aside). Both follow the visitor's light or dark mode. Edit the contact settings in whichever you keep.

**Option B now needs the `images` folder next to it** (12 screenshots of the app, about 1.3 MB in total). When you upload the site, upload the whole folder, not just the HTML file. Keep `images/` and `option-b.html` together (rename the HTML to `index.html`, leave the images folder as it is).

### About the screenshots

- They were taken from a throwaway copy of the app with a demo company called "Demo Trading Co", sample customers and vendors, made-up login names, and masked bank account numbers. The corner logo was changed to "Innologic" in the pictures only.
- Click a picture on the page to see it large. On a phone it opens big and you swipe sideways to look around.
- If the app changes and you want fresh pictures, ask Claude to retake them: it uses a demo copy of the database, never your real data.
- Before you publish, look through all 12 images once yourself (they are in `images/`) to be sure you are happy with what they show.
- `option-b.before-screens.html` is a backup of option B from before the pictures were added. You can delete it.

## Before you publish: edit 3 things

Open `index.html`, search for `var CONTACT` near the bottom:

```js
var CONTACT = { whatsapp: '62XXXXXXXXXX', email: 'hello@example.com', formUrl: '' };
```

- `whatsapp`: your number with country code, **no + and no spaces** (example: `6281234567890`).
- `email`: where enquiries should go.
- `formUrl`: optional. Paste the address from a form service (Formspree, Getform, Web3Forms) and the contact form sends messages there. If you leave it empty, the form opens the visitor's email program with the message filled in, which also works.

Also check the text for anything you do not want to promise, and replace the year or wording as you like. Search the page for words such as "Coretax" and "SAP Business One" if you want to change what you claim.

## Publish for free

Any of these accept a folder with `index.html` (drag and drop):

1. **Cloudflare Pages**: pages.cloudflare.com, "Upload assets".
2. **Netlify**: app.netlify.com/drop, drag the folder in.
3. **GitHub Pages**: put the file in a repository and turn on Pages.

You get an address like `innologic.pages.dev` straight away.

## Your own address (domain)

Buy something like `innologic.id` or `innologic.com` from a registrar (an `.id` domain needs an Indonesian ID or company papers), then add it as a custom domain in the host above. They give you the exact DNS records to enter.

## So people can find you

- Create a free **Google Business Profile** with the same name and your WhatsApp number.
- Put the website address in your WhatsApp Business profile, LinkedIn and anywhere you advertise.
- After publishing, add the site to **Google Search Console** and submit its address.
- When you have a real customer who agrees, add a short quote or logo to the page. Do not add invented ones.
