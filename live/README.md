# One-file production deployment

This is the live business website, with normal calling, email and WhatsApp handoffs. It is not the preview copy. It preserves the five supplied images, GSTIN, grades, both numbers and transport-inclusive quotation wording.

1. Download Deepa-Steel-One-File.zip.
2. Open it in the Chromebook Files app. Copy index.html out of the ZIP into Downloads. Keep the exact name index.html.
3. In the existing Cloudflare deepasteel project, choose New deployment and upload just this index.html file. The file list must show one file at the root. Do not add the old src/public folders or _headers file.
4. Keep Not Found Handling set to None. Deploy the new version to production; assign 100% traffic if asked.
5. Open Visit and refresh. The live URL still needs verification after deployment.

The self-contained HTML embeds all images, CSS and JavaScript. A hash-based Content Security Policy is embedded in the HTML. The old _headers policy is for the multi-file deployment and must not be uploaded with this version because it blocks inline scripts/styles.

Validation: 16 local Chromium checks passed, including all five images, enquiry validation, MS/GI selection, review, copy/download, WhatsApp handoff handler (navigation cancelled for tests), mobile layouts and offline browser operation after initial load. No real customer messages were sent.

The existing hosted URL returned 404 for its homepage and expected assets. Its public URL is shown as enabled in the user's dashboard. The exact Cloudflare-side cause is not confirmed. This alternative removes nested folders and separate asset requests from the upload; success on Cloudflare is not claimed until the user deploys it and the live URL is checked.

Rebuild from repository root: npm run build, then node scripts/build-single-file.mjs. Verify with node scripts/browser-check.mjs --single-file. Do not edit the generated HTML manually: rebuild it so the embedded CSP hashes stay correct.

## Google Search Console verification

The production index.html includes the owner-provided google-site-verification meta tag in its head. Upload this updated file as the production deployment, then click Verify in Search Console. Retain the tag in future versions. Adding it locally does not establish Google verification or indexing; those are confirmed in Search Console after deployment.
