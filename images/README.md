# /images

Files referenced by the site:

- `about-christmas-2015.jpg` — About page figure: David and the boys, Christmas 2015 — ✓ in repo
- `rollie-searching.png` — 404 page: Rollie searching with a magnifying glass — ✓ in repo
- `film-poster.jpg` — Poster frame for the film on the index page — ✓ in repo. **886×1920, and NOT the same picture as `panels-v5.zip/02-film-poster-start-mock.png`, despite both being called the film poster.** That panel is the **start-scan** screen (9:41) and carries no scan figures at all; this file is a **completed-scan** Home screen (9:42) showing *"Scan complete — 204 photos checked, 10 flagged for your review"*, split 4/2/3/1 — **locked set v3, superseded by set v4 on 2026-09-10.** The distinction is recorded because the two were confused on 2026-09-11 and the wrong one nearly got re-rendered.
- `about-on-the-water.jpg` — About page farm figure: David on his boat at the lease — ✓ in repo (replaced the interim leases-only `about-oyster-leases.jpg`, removed 2026-09-01 — one farm photo on the page; same image as `/press-kit/founder-photo.jpg`)

David adds images via GitHub web (Add file → Upload files) or by copying them in locally; filenames must match exactly, case-sensitive — lowercase extensions (`.jpg`, not `.JPG`; GitHub Pages is case-sensitive even though Windows isn't).

Photos are committed EXIF-stripped: GPS, device, and capture metadata removed losslessly before publish (image bytes untouched). `about-on-the-water.jpg` arrived 2026-09-01 with GPS embedded and was stripped in-repo.

Three kinds of image live in this repo. Campaign artwork, including the Rollie mascot, is AI-generated and carries embedded C2PA (Content Credentials) provenance. Product screenshots carry a C2PA tool-handling marker, which is not a generation claim. Photographs carry neither, and are EXIF-stripped before publish.
