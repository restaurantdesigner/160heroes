CANADA 160 HEROES — static site bundle
======================================

Everything in this folder is the site. There is no build step, no server code
and no database. index.html plus the assets folder is the whole thing.

WHAT IS INSIDE
  index.html          the entire page: markup, styles and scripts
  assets/             images, the map geometry (canada.js) and three.min.js

The only external request the page makes is to Google Fonts. Everything else,
including the 3D library, is served from this folder.

FASTEST WAY TO PUT IT ONLINE (about two minutes, free)
  1. Go to app.netlify.com/drop
  2. Drag this folder onto the page
  3. You get a live https URL immediately, e.g. canada160.netlify.app
  4. Site settings > Domain management to point your own domain at it

OTHER HOSTS, ALL FINE
  Vercel        vercel.com/new  -> import or drag the folder
  Cloudflare    pages.cloudflare.com -> Direct Upload
  GitHub Pages  push the folder to a repo, Settings > Pages > deploy from branch
  Any web host  upload the folder by FTP into the public directory

CUSTOM DOMAIN
  Point a CNAME record at the host's address, then add the domain in the host's
  dashboard. HTTPS is issued automatically on all four hosts above.

BEFORE IT GOES PUBLIC
  - Portraits and films are AI reconstructions. Every one needs CIHE sign-off.
  - Viola Desmond's portrait has been withdrawn; the page shows a placeholder.
  - Gertrude Elion is listed as unplaced, her Canadian connection unconfirmed.
  - The film player, the conversation and the donation flow are front-end only.
    They need real endpoints before launch.
  - Set a real domain in the footer and add analytics if you want them.

UPDATING
  Edit index.html and re-upload the folder. Netlify, Vercel and Cloudflare all
  accept a fresh drag-and-drop over the same site.
