Aurora Studio — Final Project (3 pages)
=======================================

Files
-----
index.html      Home    (hero image + about image, stats, services grid)
portfolio.html  Work    (6 project images — this is the "5+ images" page)
contact.html    Contact (4 team photos + contact form)
style.css       One shared stylesheet linked in all three pages
images/         12 placeholder SVG images  <-- REPLACE WITH YOUR OWN PHOTOS

IMPORTANT — use your own images before submitting
--------------------------------------------------
The .svg files are placeholders so the site works right away. To swap one:
  1. Put your photo (e.g. team1.jpg) into the images/ folder.
  2. Change the matching <img src="..."> to point at it.
  3. Rewrite that image's alt="..." to describe YOUR photo.
Keep at least 1 image on every page and at least 5 on portfolio.html.

Where each rubric item lives
----------------------------
1.  Skip to Main Content ......... style.css ".skip-link" (position + :focus); top of every page
2.  Validates clean .............. all 3 pages pass W3C Nu HTML checker; text passes WCAG AA contrast
3.  Position + :focus skip link .. ".skip-link" hidden at left:-9999px, shown at left:0 on :focus
4.  Navigation (>=3 properties) .. ".nav-list" / ".nav-link" use flex, gap, padding, border-radius, color, transition
5.  Box model on EVERY image ..... style.css "img { border + padding + border-radius }"
6.  Grid parent (>=2 columns) .... ".services-grid", ".work-gallery", ".about-grid", ".contact-grid"
7.  Flex parent .................. ".nav-list", ".hero-actions", ".stats-band", ".team-flex", ".footer-inner"
8.  Hover (interesting) .......... ".work-item:hover" lift+zoom+glow; ".service-card:hover"; ".btn:hover"
9.  nth-child ................... ".work-item:nth-child(odd/even) img" — alternating corner radius on images
10. WAVE accessible ............. lang set, one <h1>/page, alt on all images, labelled form fields, visible focus

How to host on GitHub Pages (free)
----------------------------------
1.  Create a github.com account and a new PUBLIC repository.
2.  Upload index.html, portfolio.html, contact.html, style.css and the images/ folder.
3.  Settings -> Pages -> Branch: main, Folder: / (root) -> Save.
4.  Wait ~1 min for the https://USERNAME.github.io/REPO/ link, then submit it.

Validate before submitting
--------------------------
HTML:  https://validator.w3.org/   (Validate by URI with your live link — all 3 pages)
WAVE:  https://wave.webaim.org/     (paste your live link for each page)

Note on the optional W3C CSS validator
---------------------------------------
The separate jigsaw CSS validator is outdated and will warn about valid modern
properties (var(), backdrop-filter, background-clip:text). These are correct CSS
and the assignment only requires the HTML validator + WAVE, so no action needed.
