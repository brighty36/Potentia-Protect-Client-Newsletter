# Potentia Protect — Client Newsletter (HTML email)

A responsive, Mailchimp-ready HTML email recreating the **Potentia Protect –
Overview** PDF (dark theme, gradient "Key Pillars" cards, Top 3 takeaways,
contact panel).

## Files
| File | Purpose |
|------|---------|
| `potentia-protect-email.html` | The email. Paste the whole file into Mailchimp. |
| `potentia-protect-email.txt` | Plain-text version (Mailchimp "Plain-Text" tab). |
| `assets/potentia-logo.png` | Potentia+ logo — header, top-right. |
| `assets/video-thumbnail.png` | Still for the "Watch our short video" block. |
| `assets/cred-mrs.png` | MRS Company Partner logo (credentials row). |
| `assets/cred-gdq.png` | Global Data Quality (GDQ) logo (credentials row). |
| `assets/cred-pjr.png` | PJR / ISO 27001 (UKAS) logo (credentials row). |
| `assets/award-winner.png` | MRS Operations Awards 2025 — Winner badge. |
| `assets/award-commended.png` | MRS Operations Awards 2025 — Highly Commended badge. |
| `assets/suzy-hassan.png` | MD photo for the "To learn more" panel. |

## How to use in Mailchimp
1. Create a campaign → **Code your own → Paste in code**, and paste the entire
   contents of `potentia-protect-email.html`.
2. Upload the images in `assets/` to Mailchimp (Content Studio / the campaign
   image manager) and copy their hosted URLs.
3. In the pasted HTML, replace these placeholders:
   - `{{POTENTIA_LOGO_URL}}` → hosted URL of `potentia-logo.png`
   - `{{VIDEO_THUMB_URL}}` → hosted URL of `video-thumbnail.png`
   - `{{CRED_MRS_URL}}` / `{{CRED_GDQ_URL}}` / `{{CRED_PJR_URL}}` → the three credential logos
   - `{{AWARD_WINNER_URL}}` / `{{AWARD_COMMENDED_URL}}` → the two award badges
   - `{{SUZY_PHOTO_URL}}` → hosted URL of `suzy-hassan.png`
   - `{{VIDEO_URL}}` (appears twice) → the link to your video
4. Send yourself a test to check on desktop, mobile and (if you use it) Outlook.

**Logo note:** the credential and award logos were extracted from the source
PDF, so they are only as sharp as the originals. The MRS Company Partner mark in
particular is low-resolution — if you have cleaner vector/PNG versions of any
logo, drop them into `assets/` (same file names) or just upload them in
Mailchimp and point the matching placeholder at them.

## Design notes
- **Responsive:** two-column card grid on desktop collapses to a single column
  on phones; the Top 3 circles and contact panel also stack.
- **Masonry cards:** the Key Pillars use two independent columns, so cards flow
  and stagger to their own height instead of aligning row-by-row — this removes
  the dark gaps caused by mismatched card lengths. Respondent Verification is a
  card in the left column. The two columns are balanced to end at roughly the
  same point. On mobile the columns stack (left column cards first, then right).
- **Why no click-to-reveal accordion:** interactive "click heading to expand"
  isn't reliable in email — JavaScript is always blocked, and Gmail/Outlook/most
  webmail strip the CSS/`<details>` tricks that fake it. If the toggle is
  stripped, those clients would show headings with no content, so the content is
  always kept visible. (A real accordion is only safe on a hosted web page, e.g.
  a "view in browser" landing page — happy to build that separately if wanted.)
- **Everything except the two photos is pure HTML/CSS** — the dark background,
  gradient cards, chips, circles and contact panel need no image hosting.
- **Outlook:** CSS gradients aren't supported by Outlook's Word engine, so cards
  fall back to a solid brand colour (orange / purple / blue). Rounded corners
  also square off in Outlook. This is expected and still on-brand.
- The header padlock uses an emoji (🔒). To match the exact logo, replace the
  `Pr&#128274;tect` text block with a hosted image of the Protect wordmark.
