# /press-kit

Files linked from /press.html:

- `icon-1024.png` — App icon, 1024px — ✓ in repo
- `wordmark.png` — Wordmark — ✓ in repo
- `panels-v5.zip` — App Store screenshot set: 7 panels (1284×2778) plus the App Preview poster frame (886×1920) — ✓ in repo. **The poster frame inside this zip (`02-film-poster-start-mock.png`) is the START-SCAN screen and carries no scan figures — it is a DIFFERENT picture from `/images/film-poster.jpg`, which fronts the film on the index page and does show figures.** Same nickname, two assets. Supersedes `panels-v4.zip`, which was retired and deleted 2026-09-10 because its closer panel still read "iOS 17+".
- `screenshots-v5.zip` — Raw app screenshots, 7 device captures — ✓ in repo. Supersedes `screenshots-v3.zip`, which was retired and deleted 2026-09-10 because its results screen still showed the superseded demo figures (4,298 / 48) and the pre-fix category order.
- `rollguard-preview-scored.mp4` — App preview film, **scored** — ✓ in repo. **This is the WEB cut**: it plays on the index page and is offered to press as the linkable version. Delivered 2026-09-11 as `RG Film Music.mp4` and renamed on arrival; **stripped of a trailing `uuid`/XMP box before its first commit — see the metadata note below.** Same 28.4 s cut as the silent film, 886×1920.
- `rollguard-preview.mp4` — App preview film, silent — ✓ in repo. **This is the ASC App Preview cut**: silent, accepted by App Review, and never re-opened. Renamed from `rollguard-preview-29s.mp4` in 2c27b28 when duration came off the label; the row was not updated at the time and said the old name until 2026-09-11.
- `rollie.png` — Rollie the RollGuard mascot — ✓ in repo
- `rgm005.png` — Campaign creative sample 1 — ✓ in repo
- `rgm006.png` — Campaign creative sample 2 — ✓ in repo
- `rgm007.png` — Campaign creative sample 3 — ✓ in repo
- `founder-photo.jpg` — Founder photo, David on the oyster lease — ✓ in repo

David adds files via GitHub web (Add file → Upload files) or by copying them in locally; filenames must match exactly, case-sensitive — lowercase extensions.

Photos are committed EXIF-stripped: GPS, device, and capture metadata removed losslessly before publish (image bytes untouched). The founder photo arrived 2026-09-01 with GPS embedded and was stripped in-repo.

**Video is swept the same way, and the rule is not image-only — it reaches any container box that carries identity, capture or third-party metadata.** `rollguard-preview-scored.mp4` arrived from Canva carrying a trailing `uuid` box of XMP with **Facebook ad-attribution fields** (`Attrib:FbId`, `Attrib:ExtId`, `Attrib:TouchType`) and a **TikTok Partner block** (`PartnerAPPID`, `PartnerAssetID`, `PartnerBusinessCenterID`, `Program TTPP`), plus `xmp:CreatorTool`. **Removed before the first commit**, so none of it ever entered git history — a blob committed once stays reachable at its SHA. The strip was lossless: only the trailing box was dropped, with `mdat` and `moov` asserted byte-identical. **An encoder tag (`©too`) is left alone** — an encoder version is not GPS, device or capture metadata, per the 2026-09-10 ruling on `film-poster.jpg`.

Three kinds of image live in this repo. Campaign artwork, including the Rollie mascot, is AI-generated and carries embedded C2PA (Content Credentials) provenance. Product screenshots carry a C2PA tool-handling marker, which is not a generation claim. Photographs carry neither, and are EXIF-stripped before publish.
