SeverTub | Company Website (single file)
==============================================

Files
-----
  index.html               Self-contained landing page, LIGHT premium theme
                           (CSS, JS and all images inlined)
  index-dark-backup.html   Previous dark-theme version (also self-contained)
  README.txt    This file
  assets/       Source images (kept for editing; index.html does not need them)
  screenshots/  Render checks (light-*.png/jpg = current light theme;
                final-*.png/jpg = previous dark theme)

How to open
-----------
  1. Double-click index.html, or
  2. From a terminal:
       open index.html          (macOS)
       start index.html         (Windows)
       xdg-open index.html      (Linux)
  3. Or drag the file into any modern browser (Chrome, Safari, Firefox, Edge).

No server or internet connection is required. There are no external fonts,
images, or CDN dependencies: every photo is embedded as a data URI, so
index.html works on its own even if copied without the assets/ folder.
The contact form is front-end only and shows a local “thank you”
confirmation; it does not send email.

Brand
-----
  SeverTub: Moscow industrial pipe / pipeline engineering (EPC-style support).
  Founder & Co-CEO: Chris E Dunn
  Co-CEO:           Dimitri Kevin Abdulov
  Primary language: English, with short Russian accents (Москва, Трубопроводы).

Sections
--------
  Hero · What we do · Leadership (Founder & Co-CEOs) · Services · Industries ·
  Specs strip · Projects (6) · Why us · Contact / quote form · Footer

Assets (source files; all embedded in index.html)
------
  assets/chris-e-dunn.jpg             Founder & Co-CEO photo (original)
  assets/chris-e-dunn-headshot.jpg    400×400 headshot crop used on the page
  assets/dimitri-kevin-abdulov.png    Co-CEO headshot (JPEG data despite .png name)
  assets/pipe-water-treatment.jpg     Insulated pipe headers in a tunnel
                                      (used: Hero background, About banner,
                                      Boiler house steam project)
  assets/pipe-steam-headers.jpg       Water treatment plant room (used: Water treatment project)
  assets/pipe-pump-station.jpg        Buried mains + valves in a trench (used: District heating project)
  assets/pipe-stainless-process.jpg   Stainless valve manifold (used: Process stainless project)
  assets/pipe-extra.jpg               Engineer with large pump rotor (used: Pump station project)
  assets/t1.jpg                       Control panel wiring (used: Cold-climate retrofit / heat tracing)
  assets/pipe-district-heating.jpg    NOT USED: actually a wood-staining photo, not pipes
  assets/pipe-steam-backup.jpg        NOT USED: byte-identical duplicate of pipe-pump-station.jpg
  Note: the steam-headers / water-treatment filenames are swapped versus their
  content; the page uses each photo where its content fits.

Changelog: Nov 2, 2026 (cleanup)
---------------------------------
  - Removed the footer "Concept site" line entirely (no replacement).
  - Copy cleanup: replaced every em dash in page text, title, meta tags,
    quote attributions and code comments with ordinary punctuation.
  - Removed the short decorative rule drawn before each section label.
  - Embedded images checked: no EXIF, XMP or C2PA metadata in any of them.
  - Verified in headless Chrome at 1440px and 390px.

Changelog: Nov 2, 2026 (retouched headshots, publish)
------------------------------------------------------
  - Replaced the illustrated portraits with subtler, mostly photographic
    retouched headshots (gentle polish only), same clean warm off-white to
    pale steel-blue backdrop for both leaders:
      assets/chris-e-dunn-headshot-retouched.jpg (600x600)
      assets/dimitri-kevin-abdulov-headshot-retouched.jpg (600x600)
    Alt text back to "<Name>, <Role> of SeverTub".
  - Footer: small low-key line "Concept site. Not an operating company."
  - Contact form note now accurate: "This form shows a confirmation on the
    page; for inquiries, email us directly."
  - Published to GitHub Pages: https://axebuild.github.io/severtub/

Changelog: Nov 2, 2026 (stylized leadership portraits)
-------------------------------------------------------
  - Both leader photos replaced with polished semi-stylized illustrated
    portraits (smooth painterly shading, ~50% less photoreal), made from
    the original photos so each person stays recognizable, on a matching
    warm off-white to pale steel-blue background:
      assets/chris-e-dunn-stylized.jpg (600x600)
      assets/dimitri-kevin-abdulov-stylized.jpg (600x600)
    Embedded as data URIs; alt text now reads "Illustrated portrait of ...".
    Originals kept in assets/ untouched.
  - Removed the footer "Demo concept site" line and reworded the contact
    form note so no "demo" wording appears anywhere on the page.
  - Not published: the local file only; the GitHub copy was not updated.
  - Verified in headless Chrome at 1440px and 390px: 0 console errors,
    0 broken images, no horizontal overflow.
    Screenshots: screenshots/stylized-leadership.png, stylized-leadership-mobile.png

Changelog: Nov 2, 2026 (light theme)
-------------------------------------
  - Converted the site to a light, premium EPC-firm look; the dark version
    is kept as index-dark-backup.html.
  - Palette: warm off-white #fafaf8 page, #f2f1ec alternate bands, white
    cards; deep navy text #0e1a2b; deep steel-blue accent #13355a for
    buttons, links, eyebrows and stats; muted gold #8a6410 kept only for
    hairlines, photo rings, leadership roles and bullets.
  - Typography: larger, tighter display headings (hero up to 4.5rem,
    section titles up to 3rem, -0.03 to -0.035em tracking), small
    wide-tracked uppercase eyebrow labels, 1.65 body line-height.
  - Layout: more whitespace (7rem section padding, 1200px max width),
    thin 1px borders, soft layered shadows, 10px card radius, gentle
    hover lift on cards, pill-shaped buttons/chips/spec pills.
  - Hero: same pipe photo under a warm-white gradient (solid behind the
    text, fading to show the pipes on the right); white glass diagram
    card; on mobile a uniform light overlay keeps text legible.
  - Navy logo, white mobile menu with shadow, white form fields with
    navy focus ring, deep navy footer band.
  - Accessibility: text colours checked for WCAG AA contrast (muted grey
    4.9:1+, gold text 4.75:1+, body text 7:1+); focus outlines kept.
  - Verified in headless Chrome at 1440px and 390px: 0 console errors,
    0 broken images/links, no horizontal overflow, mobile menu and form
    confirmation work. Screenshots: screenshots/light-*.

Changelog: Nov 2, 2026 (dark theme pass)
-----------------------------------------
  - Hero (front screen) is now clearly pipe-related: embedded photo of
    insulated industrial pipe headers as the background with a dark
    gradient overlay, new headline “Industrial pipelines, engineered for
    the north”, pipe-specific intro copy, “See pipe projects” button, and a
    more detailed pipe isometric (flanges, valve, supports, DN/PN label).
    Also fixed the hero diagram card collapsing to zero width on desktop.
  - Added Chris E Dunn as Founder & Co-CEO (photo, bio, quote) in Leadership.
  - Dimitri Kevin Abdulov is now Co-CEO (no longer listed as founder) in
    About text, Leadership, Contact, footer, and meta author.
  - All images embedded as data URIs; previously 5 project/banner images
    were relative links that broke when index.html was opened on its own.
  - Replaced mismatched photos (the wood-staining image was used 3 times as
    "district heating"; steam/water-treatment photos were swapped).
  - Fixed the Dimitri headshot data URI MIME type (image/png → image/jpeg).
  - Nav: swapped the out-of-order “Specs” link for “Industries” so the
    menu follows page order (Specs strip is still on the page).
  - Toast: [hidden] now actually hides it (display:flex was overriding it).
  - Small-screen polish (≤480px padding, headshot size, footer link wrap).
  - Verified in headless Chrome at 1440px and 390px: 0 console errors,
    0 broken images, 0 broken in-page links, no horizontal overflow,
    mobile menu and form confirmation work.

© 2026 SeverTub · Moscow
