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
| `potentia-protect-email.txt` | Plain-text version (Mailchimp "Plain-Text" tab). |
| `assets/potentia-logo.png` | Potentia logo, header top-right. |
| `assets/video-thumbnail.png` | Still for the video block. |
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
3. Six questions: orange heading, plain body copy beneath, thin rules between.
4. Proof strip: one line of copy plus the white panel of credential logos.
5. Video block: thumbnail and play button linking to the three minute film.
6. CTA panel: purple gradient, Suzy's photo, reply-to-this-email as the action.
7. Footer: copyright, address, unsubscribe and update-preferences merge tags.

Roughly 500 words of copy, about a third of the previous version.

## Design notes
- **Visual weight** sits on the video block and the CTA panel. The question set
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
