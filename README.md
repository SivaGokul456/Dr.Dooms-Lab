# Si-gul website

Static site. No build step, no framework, no server.

## Files

- `index.html`  the homepage
- `partner.html`  the enquiry page, served at `/partner`
- `scrollcraft.css`, `scrollcraft.js`  the scroll engine and design tokens
- `assets/`  the two photographs (WebP)
- `vercel.json`  clean URLs and cache headers

## Deploy to Vercel

Option A, no terminal: go to vercel.com, New Project, drag this folder onto
the upload area. Framework preset: Other. Leave build command and output
directory empty. Deploy.

Option B, terminal:

    npm i -g vercel
    vercel

Accept the defaults (Other, no build command, output directory `.`). Then
`vercel --prod` to publish.

## After the first deploy

1. Open `/partner`, send one real enquiry. FormSubmit emails a one-time
   activation link to the Si-gul inbox. Click it. Until then nothing is
   delivered.
2. FormSubmit then shows a random alias endpoint. In `partner.html`, replace
   `formsubmit.co/sivagokul456@gmail.com` with `formsubmit.co/<alias>` in the
   form's `action` so the address is not in the page source. Redeploy.
3. Attach sources to the four statistics on the homepage before launch.
