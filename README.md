# JAW AI — landing page

The built site. Source lives in a private repository; this one holds only what is served.

- `index.html` — the page, with the stylesheet inlined
- `js/` — `main.js` plus a `brain-*.js` chunk fetched after load, so three.js is not in the
  initial request graph
- `brain/` — the specimen: crest nodes and edge indices sampled from the FreeSurfer fsaverage
  pial surface, plus the poster used when WebGL is unavailable
- `plates/` — three renders of the specimen, one per practice, with that hub lit
- `standalone.html` — the whole thing in one file, no requests

Everything degrades in four rungs: text with JavaScript off, the poster without WebGL, no motion
under `prefers-reduced-motion`, and the full object otherwise.

Contact on the page is `hello@jaw.sg`. That domain is not registered yet.
