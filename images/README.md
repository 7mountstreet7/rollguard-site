# /images

Files referenced by the site:

- `about-christmas-2015.jpg` — About page figure: David and the boys, Christmas 2015 — ✓ in repo
- `rollie-searching.png` — 404 page: Rollie searching with a magnifying glass — ✓ in repo
- `about-on-the-water.jpg` — About page farm figure: David on his boat at the lease — ✓ in repo (replaced the interim leases-only `about-oyster-leases.jpg`, removed 2026-09-01 — one farm photo on the page; same image as `/press-kit/founder-photo.jpg`)

The index-page film carries **no poster image**: `poster=` was removed from the `<video>` on 2026-09-11 and `film-poster.jpg` deleted with it. The film's own first frame stands in — which needs `preload="metadata"` on the element, because `preload="none"` fetches nothing and paints a black box. **A removed asset cannot go stale, which is the point: the deleted poster carried locked set v3 (204/10) and would have needed re-cutting at every set change.** **[Updated 2026-09-21: that cross-reference is retired with its asset.** `panels-v5.zip` was superseded by `panels-v6.zip` and deleted, and `02-film-poster-start-mock.png` ships nowhere — **it was the App Preview’s poster frame, and the App Preview was removed from the listing entirely to resolve Guideline 2.3.4.** So there is now no "film poster" anywhere in either repo, and nothing left to confuse this with.]**

David adds images via GitHub web (Add file → Upload files) or by copying them in locally; filenames must match exactly, case-sensitive — lowercase extensions (`.jpg`, not `.JPG`; GitHub Pages is case-sensitive even though Windows isn't).

Photos are committed EXIF-stripped: GPS, device, and capture metadata removed losslessly before publish (image bytes untouched). `about-on-the-water.jpg` arrived 2026-09-01 with GPS embedded and was stripped in-repo.

Three kinds of image live in this repo. Campaign artwork, including the Rollie mascot, is AI-generated and carries embedded C2PA (Content Credentials) provenance. Product screenshots carry a C2PA tool-handling marker, which is not a generation claim. Photographs carry neither, and are EXIF-stripped before publish.
