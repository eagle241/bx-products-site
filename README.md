# BX Products company hub

Static single-page site for [bx-products.com](https://bx-products.com): the Australian company hub for BX Products brands.

- **Stack:** one `index.html` plus `logo-bx-badge.jpg` at the repo root. No build step.
- **Deploy target:** [Render Static Site](https://render.com/docs/static-sites). Publish root is this repository; the public file is `index.html`.
- **Context:** Australia (AUD). Legal footer names BX Products Pty Ltd ATF BX Products Trust, ABN 26 486 245 507.
- **Go-live:** connecting the Render service and pointing the domain are manual. This repo does not deploy or change DNS on its own.

## Contact form

The form posts to [FormSubmit](https://formsubmit.co/birger@bx-products.com) and emails submissions to birger@bx-products.com. Name, email, and message are unchanged. There is no backend in this repo.

After a successful send, FormSubmit redirects back to this page (`?sent=1#thanks`), which shows a thank-you message.

**One-time activation (required before mail is delivered):** the first submission emails birger@bx-products.com an “Activate Form” link from FormSubmit. Open that email and click the link once. Until then, FormSubmit does not forward messages, and the sender sees FormSubmit’s activation page instead of the thank-you. No access key is required. ReCAPTCHA stays on (FormSubmit’s default) so the inbox is less likely to be rate-limited; a hidden honeypot field is also included.
