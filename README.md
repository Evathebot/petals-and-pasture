# Petals and Pasture website

Static HTML version of the Petals and Pasture site design. Open `index.html` in any browser to click through it. No build step and no dependencies.

## Pages

| File | Page |
|---|---|
| `index.html` | Home |
| `cow-cuddles.html` | Cow Cuddles ($35 / $250 / VIP Day $800) |
| `events.html` | Events and Parties |
| `weddings.html` | Weddings |
| `photoshoots.html` | Photoshoots (professional photographers only) |
| `farm-stand.html` | Farm Stand (dahlias, cosmos, zinnias, wildflowers) |
| `about.html` | About and Meet the Herd |
| `faq.html` | FAQ |
| `book.html` | Booking inquiry form |

Every page has the same nav and footer copied in. If you move this into a CMS or framework (Webflow, WordPress, Next.js, etc.), turn those two into shared components.

## Assets (`assets/`)

- `logo-brown.png`, `logo-white.png`: logo with a transparent background, cut from `logo-original.png`
- `cow-*.svg`: the 8 cartoon mini Highlands scattered around the pages. Each one is unique. Keep them scattered at random, not in a pattern.
- `dahlia.svg`, `cosmos.svg`, `zinnia.svg`, `wildflowers.svg`, `bouquet.svg`, `garland.svg`, `*-head.svg`: floral artwork
- `cosmos-head.svg` is also the favicon

## Brand

- **Fonts:** Fraunces (headings, prices) and DM Sans (body), both from Google Fonts
- **Colours:**
  - Cream background `#FDF6EC`
  - Sage `#687A4E` (header bar, footer, CTA bands), dark sage text `#4F5E37`, light sage `#EEF1E6`
  - Rose `#A8615B` (main buttons, featured cards), blush `#F7DCD5`
  - Price brown `#8B5A3C`, heading brown `#3E2F24`, body text `#463629`
  - Peach badge `#F5CC98` with text `#5B3A1E`
- **Rules:** prices are always the biggest text on a card, the featured package gets the rose header and a peach badge, and there are no em dashes in any copy

## To do before launch

1. **Booking form (`book.html`):** it shows a thank-you message but doesn't send anything yet. Connect it to the booking system (GoHighLevel, Formspree, Netlify Forms, etc.). Field names are already set: `name`, `email`, `phone`, `experience`, `date`, `guests`, `location`, `message`, `bouquet`.
2. **Photos:** 17 dashed boxes labelled `[Photo: ...]`, `[Map: ...]` and `[Instagram post]`. Each label says what shot goes there. The map should be a Google Maps embed. The Instagram grid can be an Instagram feed widget.
3. **Placeholder text:** search the files for `[`
   - `[FARM ADDRESS]`, `[PHONE NUMBER]`, `[EMAIL ADDRESS]`, `[HOURS]` / `[DAYS AND HOURS]` (mostly in the footer)
   - `[COW NAME]`, `[AGE]`, `[COAT COLOUR]`, plus the personality lines (Home and About)
   - `[YOUR NAMES]`, the 3 story paragraphs and the signature (About)
   - Farm stand: `[PRICE]`, `[MONTHS]`, `[MONTH]`, `[SEASON DATES]`, `[CASH / CARD / E-TRANSFER]`, bouquet descriptions
   - `[RESPONSE TIME]` (Book page)
4. **SEO:** every page already has a title and meta description. Add the domain, an Open Graph image and a sitemap once hosting is set up.

All prices match the approved 2027 price sheets: Canadian dollars, plus GST.
