# Review the complete website before launch

## Open the interactive preview on a laptop or desktop

1. Open `Deepa-Steel-Preview.html` in this GitHub folder.
2. Click **Download raw file** (the download-arrow icon). If GitHub shows code, that is expected: download the HTML file rather than trying to run it inside GitHub.
3. Open the saved `Deepa-Steel-Preview.html` with Chrome or Edge. On Windows, right-click the file, choose **Open with**, and choose your browser. On macOS, use **Open With** from Finder.
4. The complete website opens from your computer. You do not need Node.js, a server, an account, or an internet connection after downloading.
5. Share this same HTML file with your dad through your usual file-sharing method. A ZIP version is also provided if your mail application does not accept HTML attachments. Extract it before opening.

For the simplest review, use a laptop or desktop. Phone file-preview applications may not run JavaScript; a hosted preview is better for phone-only review.

## What to try with your dad

- Browse the homepage, all five product categories, About, How to Order and Contact.
- Choose **Request a quote**.
- Add mild steel plates: thickness 10 mm, width 1500 mm, length 6000 mm, quantity 5 tonnes.
- Add rectangular pipes: outer width 100 mm, outer height 50 mm, wall thickness 4 mm, length 6000 mm, quantity 5000 kg.
- Continue with fictional customer details and a delivery city/state. Review the complete 10-tonne enquiry.
- Edit or remove products, change the dispatch option, and try the specification-help option.
- The preview deliberately blocks WhatsApp, email and telephone handoffs. Clicking WhatsApp displays a review confirmation instead of opening a real conversation. Copy/download still provide the full enquiry message.

The form values are temporary and are lost when the page is refreshed. Product specifications above are test inputs, not stock claims. The banner clearly identifies this as a review copy.

## After your dad approves: publish the production website for ₹0

The separate `Deepa-Steel-Website.zip` contains the production site with normal WhatsApp handoff enabled. **Do not deploy the preview HTML or preview ZIP as your business website.**

1. Create or sign into the business's Cloudflare account. Choose the free Pages plan and its included `pages.dev` address; a purchased domain is optional and outside this ₹0 plan.
2. In Workers & Pages, create a Pages project using **Direct Upload**. Use the current official steps at https://developers.cloudflare.com/pages/get-started/direct-upload/ if the menu labels differ.
3. Download `Deepa-Steel-Website.zip` and upload that ZIP. Its root contains `index.html`, `_headers`, `src/` and `public/`. If the interface asks for a folder, extract the ZIP and upload the extracted contents.
4. Choose an available project name. Cloudflare provides the resulting HTTPS website address. We cannot know that address until the project is created.
5. Open the published site on a real phone and computer. With the owner's permission, send one labelled test enquiry and manually attach a file in WhatsApp; confirm receipt with the owner before sharing the address with customers.

No publication has been performed. Hosting account registration, the exact available project name, public deployment and real WhatsApp receipt remain pending. Check the provider's current free-plan limits; no paid add-ons are needed for this static website.

## If you need a clickable online preview before approval

A live browser link requires hosting the preview somewhere. You can upload the single preview HTML as `index.html` in a separate free Pages project, with a clearly identified review name. That creates an online review copy, not an official business launch, but the address is accessible to people who have it unless you configure access controls. After approval, create a separate production project using `Deepa-Steel-Website.zip`.

The downloaded-file option above lets you review first without putting a preview website online.

## Validation notes

The standalone sample passed nine Chromium checks for catalogue rendering, multiple products, validation, review, keyboard focus, mobile navigation and disabled outgoing handoff. It was loaded from a local HTTP server and tested with browser networking disabled afterward. This managed test browser blocks file URLs, so direct file opening could not be independently tested here. The sample contains its own styles, scripts and artwork and needs no external assets. Production testing previously passed 16 business-rule tests and 15 browser checks.

## Business calling numbers

The contact section shows **9322758844** and **9322658844** as equal business calling numbers, one below the other, without a separate heading above the second number. Both are click-to-call links in the production website. WhatsApp enquiries go to **9322758844**. Review-copy contact links remain disabled.

## Quotation update

Transport charges are included in quotations. This is stated on the homepage, in ordering guidance and in the enquiry review/message. Delivery timing, payment terms and material availability are confirmed by an owner. Tax and unloading treatment have not been confirmed.

Web product photography is pending: this environment could not access Wikimedia Commons, Pexels or Unsplash to download and verify reusable photographs. The existing local illustrations remain. No GST number, new grades/sizes or document-availability claims have been added.
