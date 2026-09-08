# TROOPERS — F&B Staffing page

Static HTML. No build step, no dependencies.

## Files

```
index.html        the whole page (inline styles + a <style> block for @keyframes and :hover)
assets/           photos and client logos referenced by index.html
```

## Open it

Open `index.html` in a browser, or in VS Code use the **Live Server** extension → *Go Live*.

## Editing notes

- Layout and colours are inline `style` attributes on each element. Brand colours: navy `#131249`, orange `#F47F20`.
- The `<style>` block in `<head>` holds only what cannot be inline: `@keyframes` for the three marquees (`roll`, `band`, `logos`) and the `.h1`–`.h19` hover rules.
- Fonts load from Google Fonts (Poppins). Remove the `<link>` tags and self-host if the site must work offline.
- Three marquees: the orange role ticker (`roll`), the photo band (`band`), the client logos (`logos`). Speed is the duration in `animation: <name> 34s linear infinite`. Each has two identical tracks — if you add or remove an item, add or remove it in **both** tracks or the loop will jump.
- Logos on the dark ground: `logo-chagee-dark.png` and `logo-tealive-dark.png` are recoloured copies (neutral dark ink turned white, brand colours kept). `logo-baskbear.jpg` has an opaque orange background; a transparent PNG would sit better.
- Every call to action links to `https://troopersapp.com/employer-signup`.

## Still to confirm before publishing

- `role-*.png` and `case-*.png` photos are AI-generated placeholders, not real shoots.
- The Kitchen helper row in the call sheet has a "PHOTO NEEDED" placeholder tile.
- Pricing copy (RM 25 per completed shift, 8% SST, RM 5,000 minimum order, 50% charge for cancellations under 48 hours) follows troopers.com.my/partner/pricing-plans as of the export date. Re-check before going live.
