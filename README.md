# Innologic website

The public website for **Innologic**: ERP software, setup, training and support for trading, retail and distribution companies.

- `index.html` is the whole site (no build step, no external scripts or fonts).
- `images/` holds the screenshots. They come from a demo company with sample data.

## Before you go live

Open `index.html`, find the line starting `var CONTACT` near the bottom and replace the WhatsApp number and email with real ones.

## Languages

The site has two languages. **English is the default**; visitors switch to Bahasa Indonesia with the ID / EN buttons in the top bar (the choice is remembered in their browser, and ?lang=en opens the English version).

- English text: content.json. Indonesian text: content.id.json. Both are edited at /admin (two entries: English and Bahasa Indonesia) and must keep the same structure and the same number of items.
- Words that are not in the editor (the drawings of the restaurant POS, form labels, screenshot descriptions) are translated by a list inside index.html (I18N_ID).
- Upload all of: index.html, content.json, content.id.json, dmin/config.yml.
