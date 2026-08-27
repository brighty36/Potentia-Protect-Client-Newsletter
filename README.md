# Potentia Protect: Client Newsletter (HTML email)

A responsive, Mailchimp-ready HTML email for the **September 2026** send to
existing Potentia Insight clients.

The email answers the data quality questions clients are being asked by their
own stakeholders, so it can be forwarded internally. It is a reference document,
not a brochure: six questions in the client's voice, each with a short, specific
answer naming the tools and standards involved.

**Subject line (primary):** How do we know this data is real?
Alternates: "The data quality questions your stakeholders are asking" /
"Six questions to ask any research supplier".
**Preheader:** Before you scope your Q4 studies, the answers worth having to hand.

## Files
| File | Purpose |
|------|---------|
| `potentia-protect-email.html` | The email. Paste the whole file into Mailchimp. |
| `potentia-protect-email-light.html` | Plain build: same copy typed as an ordinary email, white background, logo is the only image. |
| `potentia-protect-email.txt` | Plain-text version (Mailchimp "Plain-Text" tab). |
| `assets/potentia-logo.png` | Potentia logo, header top-right. |
| `assets/video-thumbnail.png` | Unused. Was the still for the video block, now replaced by a PDF link. |
| `assets/cred-mrs.png` | MRS Company Partner logo (proof strip). |
| `assets/cred-gdq.png` | Global Data Quality (GDQ) logo (proof strip). |
| `assets/cred-pjr.png` | PJR / ISO 27001 (UKAS) logo (proof strip). |
| `assets/suzy-hassan.png` | MD photo for the CTA panel. |
| `assets/award-winner.png`, `assets/award-commended.png` | MRS Operations Awards 2025 badges. Not used in this version. |
| `archive/` | The previous PDF-transcription version of the email, kept for reference. |

## How to use in Mailchimp
1. Create a campaign, choose **Code your own → Paste in code**, and paste the
   entire contents of `potentia-protect-email.html`.
2. No image hosting is needed. All `<img>` and background URLs already point at
   the Mailchimp-hosted assets used by the previous send.
3. Paste `potentia-protect-email.txt` into the campaign's Plain-Text tab.
4. Send yourself a test to check on desktop, mobile and (if you use it) Outlook.

## Structure
1. Header: Potentia lockup, logo, "Pr🔒tect" wordmark, standfirst.
2. Opening: two short paragraphs framing the questions.
3. Six questions: orange heading, plain body copy beneath, vertical spacing between.
4. Proof strip: one line of copy plus the white panel of credential logos.
5. PDF block: icon and button linking to the PDF overview.
6. CTA panel: purple gradient, Suzy's photo, reply-to-this-email as the action.
7. Footer: copyright, address, unsubscribe and update-preferences merge tags.

Roughly 500 words of copy, about a third of the previous version.

## Which build to send

Both files carry identical copy, structure and brand styling. Pick one:

- **`potentia-protect-email.html`** is the full build: hosted PDF-link block,
  credential logo images, Suzy's photo.
- **`potentia-protect-email-light.html`** is the plain build. It carries the
  same copy but is presented as an ordinary typed email: white background,
  dark text, full-width reading column, no dark theme and no panels. The
  Potentia logo and the accreditation strip are the only images. The PDF
  overview is a text link, and it ends with a typed signature from Suzy.

The plain build reads as a personal message rather than a campaign, which is
the point: this email is meant to be forwarded internally, and a forwarded
message travels better than a forwarded brochure. It also renders completely
with images blocked (the default in Outlook and much corporate mail), is small
enough that Gmail will not clip it, and cannot break if a hosted image URL moves.

Two copy differences in the plain build, both consequences of it being a typed
message rather than a designed one:

- The "Pr🔒tect" wordmark and the "How we're tackling your biggest data
  quality concerns" standfirst are dropped. A typed email does not open with
  a masthead. It opens with "Hi *|FNAME|*," instead.
- The close is in the first person ("get in touch with me directly") and signs
  off "Suzy", rather than referring to her in the third person. The "Want to
  talk this through in person?" heading is dropped for the same reason.

Note that the plain build is still an HTML email, not the plain-text
alternative. Mailchimp's "Plain-Text" tab only accepts plain text, so
`potentia-protect-email.txt` is still what goes there.

## Design notes
- **Visual weight** sits on the PDF block and the CTA panel. The question set
  is deliberately light: headings and body copy on the dark background, no cards,
  so the answers read as reference material rather than brochure furniture.
- **Responsive:** 600px container, single column below 600px. The proof strip
  logos and the CTA panel stack on phones.
- **Copy rules:** no em dashes, no exclamation marks, named tools and named
  standards throughout.
- **Accuracy:** ISO 27001 is *certified through PJR*, not merely aligned to the
  principles. Supplier vetting is against *ISO 20252 and the ESOMAR 37*, not
  "recognised industry benchmarks". Do not revert to the PDF wording.
- **Outlook:** CSS gradients are not supported by Outlook's Word engine, so the
  background and CTA panel fall back to a solid brand colour. Rounded corners
  also square off. This is expected and still on-brand.
- The header padlock uses an emoji (🔒). To match the exact logo, replace the
  `Pr&#128274;tect` text block with a hosted image of the Protect wordmark.

## Dropped from the previous version
- The twelve gradient pillar cards.
- The TOP 3 TAKEAWAYS circles.
- The two MRS Operations Awards 2025 badges in the contact panel.
- The website link as a CTA. There is now one action, which is to reply.
