# BX Products company hub

Static single-page site for [bx-products.com](https://bx-products.com): the Australian company hub for BX Products brands.

- **Stack:** one `index.html` plus `logo-bx-badge.jpg` at the repo root. No build step.
- **Deploy target:** [Render Static Site](https://render.com/docs/static-sites). Publish root is this repository; the public file is `index.html`.
- **Context:** Australia (AUD). Legal footer names BX Products Pty Ltd ATF BX Products Trust, ABN 26 486 245 507.
- **Go-live:** connecting the Render service and pointing the domain are manual. This repo does not deploy or change DNS on its own.

## Contact form

The form posts to [FormSubmit](https://formsubmit.co/birger@bx-products.com) and emails submissions to birger@bx-products.com. Name, email, and message are unchanged. There is no backend in this repo.

After a successful send, FormSubmit redirects back to this page (`?sent=1#thanks`), which shows a thank-you message.

FormSubmit’s one-time activation for birger@bx-products.com is done. No access key is required. reCAPTCHA is turned off so a visitor returns straight to the thank-you message; a hidden honeypot field is included.
