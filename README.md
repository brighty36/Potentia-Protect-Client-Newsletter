# Potentia Protect — Client Newsletter (HTML email)

A responsive, Mailchimp-ready HTML email recreating the **Potentia Protect –
Overview** PDF (dark theme, gradient "Key Pillars" cards, Top 3 takeaways,
contact panel).

## Files
| File | Purpose |
|------|---------|
| `potentia-protect-email.html` | The email. Paste the whole file into Mailchimp. |
| `assets/video-thumbnail.png` | Still for the "Watch our short video" block. |
| `assets/suzy-hassan.png` | MD photo for the "To learn more" panel. |
| `assets/potentia-logo.png` | Optional Potentia+ wordmark (header uses text by default). |

## How to use in Mailchimp
1. Create a campaign → **Code your own → Paste in code**, and paste the entire
   contents of `potentia-protect-email.html`.
2. Upload the two images in `assets/` to Mailchimp (Content Studio / the
   campaign image manager) and copy their hosted URLs.
3. In the pasted HTML, replace these placeholders:
   - `{{VIDEO_THUMB_URL}}` → hosted URL of `video-thumbnail.png`
   - `{{SUZY_PHOTO_URL}}` → hosted URL of `suzy-hassan.png`
   - `{{VIDEO_URL}}` (appears twice) → the link to your video
   - `{{POTENTIA_LOGO_URL}}` → *optional*; only if you uncomment the logo `<img>` in the header
4. Send yourself a test to check on desktop, mobile and (if you use it) Outlook.

## Design notes
- **Responsive:** two-column card grid on desktop collapses to a single column
  on phones; the Top 3 circles and contact panel also stack.
- **Everything except the two photos is pure HTML/CSS** — the dark background,
  gradient cards, chips, circles and contact panel need no image hosting.
- **Outlook:** CSS gradients aren't supported by Outlook's Word engine, so cards
  fall back to a solid brand colour (orange / purple / blue). Rounded corners
  also square off in Outlook. This is expected and still on-brand.
- The header padlock uses an emoji (🔒). To match the exact logo, replace the
  `Pr&#128274;tect` text block with a hosted image of the Protect wordmark.
