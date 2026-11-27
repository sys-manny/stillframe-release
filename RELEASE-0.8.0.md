# Stillframe 0.8.0

**Windows x64 · Portable ZIP · Free for personal, noncommercial use**

This release adds a borderless photo/video pop-out, profile backup/import, refreshed controls and branding, and fixes playback and cache-cleanup issues. It includes the accepted exFAT import-recovery repair.

- **Photo and video pop-out.** Keep a movable, resizable, always-on-top player open while browsing. Preserve aspect ratio, navigate through the folder, open new photos/videos into the floating player, and return to the main viewer. Playback position, volume and audio ownership follow the player.
- **Shared player controls.** Material Symbols and full-width translucent hover controls keep navigation consistent. Volume for videos and zoom for photos share the right-aligned area. Click the video viewport to play or pause.
- **Compact Backup & import.** Choose Settings, Thumbnails, Tags and People data independently; all four means a complete profile. Save ZIP-format `.library` archives with `yyyymmdd_hhmm.library` names. Import replaces selected categories, preserves categories left off, and retains the previous profile. Original photos and videos are excluded.
- **exFAT recovery repair.** Account for native directory identity changes after an owned rename. Interrupted imports use guarded recovery; checksums, per-file validation, unknown-data refusal and retained previous profiles remain in place.
- **Playback and cleanup.** Improve video opening and concurrent thumbnail generation, repair the reported M4V playback errors, and speed up Empty thumbnail cache preparation with a reusable index and checked/total progress.
- **Refreshed interface.** Source Sans 3, Hidden S branding, Slim inset scrollbars, plain slider dots and a bounded, scrollable Preferences panel.

## Upgrade and saved data

Extract the complete ZIP and open `Stillframe.exe`. Use **Preferences → Backup & import** in the previous copy, select the categories to save, and create a new `.library` archive. Import it in the new copy and restart. Closed-profile copying remains supported; preserve the entire `app/Stillframe` folder. [Getting started](INSTALL-0.8.0.md)

Saved thumbnail bytes remain unchanged at 1280 px, with a 64 MiB display cache. Existing manual video frames, tags, People data and source/cache checks remain. No Windows file association, Explorer archive icon or double-click import integration is installed.

## Verification

The owner accepted the r10 player checks and the corrected import's restore, saved-data and restart checks. Fresh repair validation passed 136 UI tests (2 existing ignored) and 28 transfer tests. A separately run real-exFAT test covered all 15 category combinations,30 preference reopenings, interrupted/committed recovery and refusal of altered data. Normal optimized build and all package/ZIP hashes passed. This is targeted coverage, not a full legacy-suite or universal-device claim. Included verification/checklist documents record their build-time state; subsequent live acceptance is recorded here.

## Known limits

- AVIF remains unsupported, including AVIF with a JPEG extension. Animated, lossless and alpha WebP remain outside current photo-viewer support.
- Tags apply to photos/videos, not folders. Suggested People stacks and visual duplicate candidates need review. Visual duplicate review compares photos; differently encoded video matching is not included. Recycling requires Windows Recycle Bin support on the source drive.
- Grid/Column retain their 128 MiB metadata envelope; changing, unavailable or unusually large folders can return partial results. Browsing/importing does not automatically generate thumbnails.
- Profile transfer requires ordinary writable local NTFS/exFAT storage. Reparse/cloud/recall content, hard links, extra streams and unsupported control-file states are refused. Limits remain 64 MiB manifest, 200,000 entries and 16 GiB per member. Incomplete/changed staging may be retained rather than deleted.
- This build is unsigned. Cloud-managed libraries, export/conversion and duplicate acceleration remain deferred.

## Third-party runtime source

Playback DLLs are unchanged from 0.7.2. Their [corresponding source and build configuration](https://github.com/sys-manny/stillframe-release/releases/download/v0.7.2/Stillframe-0.7.2-playback-runtime-source.zip) remain available there. Runtime/font/model notices are included in the ZIP. `SHA256SUMS.txt` records the application and corresponding-source archive checksums.
