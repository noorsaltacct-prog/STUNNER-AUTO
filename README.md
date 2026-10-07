# Stunner Autoworks website preview

This is a static website. No build tools are needed.

## Publish it
1. Unzip the download. Open the unzipped folder so you can see `index.html` and the other files.
2. On GitHub, create a new repository. Choose **Add file > Upload files** and drag **all contents** of the unzipped folder into the upload area, keeping the folders intact. Commit the files.
3. On Vercel, choose **Add New Project**, import the GitHub repository, select Framework Preset **Other**, and choose **Deploy**.
4. To add your real work photos, open the `gallery` folder in GitHub, choose **Add file > Upload files**, and upload images named `photo-1.jpg` through `photo-8.jpg`. Commit. They will replace the placeholder tiles. To use fewer photos or change descriptions, edit the `GALLERY_IMAGES` array near the top of `assets/js/main.js`.
5. Before sharing the site, open `assets/js/main.js` in GitHub and edit `BUSINESS_PHONE`, `BUSINESS_EMAIL`, and `FORM_ENDPOINT` at the top. The phone must include its country code, for example `+1...`. A Formspree-compatible form URL can go in `FORM_ENDPOINT`; otherwise, setting the email enables the email-app fallback. Without either, the form shows a clear configuration warning and does not pretend to submit. Update the `[PHONE]`, `[EMAIL]` and hours placeholders in `index.html` as well. Update JSON-LD telephone/email in `index.html`.
6. To add a custom domain, open the Vercel project's **Domains** settings and follow the on-screen instructions. Then replace `[YOUR-DOMAIN]` in the canonical URL, Open Graph URL/image, JSON-LD URLs, `robots.txt`, and `sitemap.xml` with the real domain. The site can deploy before a domain is connected.

## Important launch checklist
- Business information provided: Stunner Autoworks; San Antonio and surrounding areas; mobile mechanic; diagnostics, repairs, tire services, oil changes; tagline 'No job is too big' and 'Fast • Reliable • Affordable'. Other services on the site are typical requests, not independently confirmed offerings; confirm before launch.
- Phone, email, hours, owner, license and street address were not provided. Do not publish placeholders as if they are actual contact information.
- The six testimonial cards are **sample layout content only**, not real reviews. Replace with real, authorized customer reviews or remove the section before publishing.
- No stock photos are used. This avoids guessing incorrect Unsplash IDs. The hero uses a fast branded CSS background. If you later add stock photography, use licensed Unsplash images that depict a mechanic working on an engine. Suggested searches: `mechanic repairing car engine`, `mechanic changing brake pads`, `car battery jumper cables`, `OBD diagnostic scanner`, `mechanic oil change`.
- The included `assets/logo.png` is the supplied logo artwork. `assets/favicon.svg` is a simplified branded favicon.
- Static HTML and CSS are lightweight, but Lighthouse scores depend on network, hosting and added images and cannot be guaranteed without a deployed test.
