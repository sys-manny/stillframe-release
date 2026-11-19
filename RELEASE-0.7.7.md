# Stillframe 0.7.7 Falcon

**Windows x64 · Portable ZIP · Free for personal, noncommercial use**

This release improves duplicate scanning and review, saved-thumbnail reuse after remounts, image compatibility, Grid scrolling, and viewer navigation.

- Separate **Scan exact (fast)** and **Scan visual (slow)** buttons use the shared Selected / This folder / Library scope panel. Refresh remains independent.
- Exact and Visual duplicate scans use temporary SQLite listings across registered libraries. The previous duplicate-listing limit and 512-photo Visual cap are removed; source checks and shared memory budgets remain.
- Preparation respects the selected folder and Include subfolders. Retry, Stop and review, bottom-bar progress, action visibility, and group alignment are repaired.
- Recycling reviewed duplicates updates affected folder counts and removes stale review entries while preserving unrelated library state.
- Saved thumbnails remain reusable after drive remounts, including manually chosen video thumbnails, with per-file source validation retained.
- JPEG primary-image handling, unset EXIF orientation, short padding, large PNG viewing, and blank People crops include the accepted compatibility fixes.
- Grid scroll bounds settle after density changes. Video progress follows playback after seeking and switching files.
- Back, Escape, and native-menu Back restore the normal window when leaving a fullscreen photo or video.

Extract the full ZIP and open `Stillframe.exe`. Keep your complete `app/Stillframe` profile when upgrading. [Getting started](INSTALL-0.7.7.md)

## Verification

The published executable is the owner-accepted r10 executable. All five release-candidate live checks, 113 production UI tests, and the normal production build passed. The image fixes passed checks on 20 affected originals, including thumbnail generation and reuse after restart; 56 photo regressions passed. Package files are verified by SHA-256. Personal profiles and media are excluded from the download.

## Known limits

- Tags, catalog migration, and cloud-managed libraries remain deferred.
- AVIF images remain unsupported, including AVIF data stored with a .jpg filename. Animated, lossless, and alpha WebP are outside current photo-viewer support.
- Grid and Column browsing retain the shared 128 MiB metadata budget; very large, changing, or unavailable folders can yield partial results. The duplicate listing changes do not remove that browsing budget.
- Visual duplicate signatures propose candidate pairs and can miss matches that exhaustive comparison would find.
- Duplicate recycling requires Windows Recycle Bin support on the source drive.
- Suggested People stacks need review. The earlier People-scan thumbnail report stays deferred unless it recurs.
- This build is unsigned. Supported portable volumes must be writable local NTFS or exFAT drives that Windows reports as fixed.

## Third-party runtime source

The playback DLLs are unchanged from the 0.7.2 public release. Their [corresponding source and build configuration](https://github.com/sys-manny/stillframe-release/releases/download/v0.7.2/Stillframe-0.7.2-playback-runtime-source.zip) remain available there. The ZIP includes third-party notices. `SHA256SUMS.txt` records the application and corresponding-source archive checksums.
