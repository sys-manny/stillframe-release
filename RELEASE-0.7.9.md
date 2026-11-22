# Stillframe 0.7.9 Falcon

**Windows x64 · Portable ZIP · Free for personal, noncommercial use**

This release adds manual photo/video tags with reusable name suggestions, keeps the Column scrollbar visible with Details open, and improves thumbnail generation during video playback and People stack stability.

- Add and remove tags in Details for one photo/video or a selection. Combine tag filtering with filename search, media type and sorting in folders and All Libraries. Tags persist through restart and supported in-app rename/move operations without changing original media.
- Global tag names work across libraries, including names with no remaining assignments. After three matching characters, Add tags and Filter tags offer up to eight case-insensitive prefix matches. Use the mouse, arrow keys, Enter or Tab to complete text. Applying tags remains explicit.
- Column view keeps its vertical scrollbar at the visible file-list edge while Details is open. Horizontal scrolling preserves header alignment and row selection.
- Video playback uses verified file-specific reservations so unrelated photo thumbnail work can continue, while retaining same-file/alias protection and conservative handling of unknown identities.
- Naming faces/stacks preserves manual expansion choices. An explicit reveal of a photo in People can still open its containing stack.
- Keep the whole portable profile when upgrading. Saved 1280px thumbnails, manual video frames, the 64 MiB density cache, source checks, full cache-hit validation, per-file locks and durable writes are retained.

Extract the full ZIP and open `Stillframe.exe`. Preserve the complete `app/Stillframe` profile when upgrading. [Getting started](INSTALL-0.7.9.md)

## Verification

Finalized from r2. All five r2 live checks passed: retained settings/saved data, Column scrolling, global tag completion, combined tag filtering and restart persistence. The final production change is the version footer. The normal final build passes; 124 offscreen UI and 199 affected browser tests, plus disposable tag migration and restart checks, carry forward with source identity verified. Additional video reservation, processing and People regressions were checked during development. The full legacy common suite still requires unavailable fixtures/setups; no full-suite pass is claimed. Package files and ZIP entries are verified by SHA-256. Personal profiles and original media are excluded.

## Known limits

- Tags apply to photos/videos, not folders. Tags are stored in the portable profile rather than embedded in original media.
- Full library listing still takes time; verified early cards remain usable while it continues. Grid and Column retain the 128 MiB metadata budget; changing, unavailable or unusually large folders can produce partial results.
- Browsing/importing does not automatically generate thumbnails.
- AVIF remains unsupported, including AVIF with a .jpg extension. Animated, lossless and alpha WebP remain outside current photo-viewer support.
- Suggested People stacks need review. Visual duplicate signatures propose candidates and can miss matches; recycling requires Windows Recycle Bin support on the source drive.
- Catalog migration, folder tags and cloud-managed library work remain deferred.
- This build is unsigned. Portable profiles require a writable local NTFS or exFAT volume reported as fixed by Windows.

## Third-party runtime source

Playback DLLs are unchanged from the 0.7.2 public release. Their [corresponding source and build configuration](https://github.com/sys-manny/stillframe-release/releases/download/v0.7.2/Stillframe-0.7.2-playback-runtime-source.zip) remain available there. Third-party notices are included in the ZIP. `SHA256SUMS.txt` records the application and corresponding-source archive checksums.
