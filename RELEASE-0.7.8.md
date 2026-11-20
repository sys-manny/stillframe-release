# Stillframe 0.7.8 Falcon

**Windows x64 · Portable ZIP · Free for personal, noncommercial use**

This release improves Library thumbnail generation, startup navigation and All Libraries loading, and makes People scanning an explicit sidebar action.

- Verified All Libraries cards appear before the full listing finishes. Select and open an early photo during loading; selection remains through completion.
- The sidebar becomes usable early, restores the last folder or All Libraries, and reveals the restored folder row.
- All Libraries shows checked counts, loading progress and Cancel in the bottom bar. Completed listings leave scan and thumbnail controls available.
- Include subfolders is remembered between sessions.
- Thumbnail generation reuses the job's cache-name index to reduce repeated cache-directory opens, preserving source checks and complete validation of cache hits. Generation stays responsive and supports normal cancellation.
- People scans use the shared Selected / This folder / Library sidebar controls. Opening the controls does not automatically scan the library; explicitly press Scan People to run the chosen scope.
- Saved thumbnails remain 1280px; the density-sized memory cache stays at 64 MiB. Source validation, per-file locks, manual video thumbnail choices and durable writes remain.

Extract the full ZIP and open `Stillframe.exe`. Preserve the complete `app/Stillframe` profile when upgrading. [Getting started](INSTALL-0.7.8.md)

## Verification

Finalized from the accepted r8 candidate. All four live checklist checks passed. The final production build and 120 UI tests passed; the final source changes only the release footer from r8. A native early-photo interaction and full-list merge check carries forward with functional source identity verified. All executable and runtime bytes match the verified local final release. Public package files and ZIP entries are checked by SHA-256. Personal profiles and original media are excluded.

## Known limits

- Full library listing still takes time; verified early cards remain usable while it continues. Grid and Column retain the 128 MiB metadata budget, and changing, unavailable or unusually large folders can produce partial results.
- Browsing/importing does not automatically generate thumbnails.
- AVIF remains unsupported, including AVIF with a .jpg extension. Animated, lossless and alpha WebP remain outside current photo-viewer support.
- Suggested People stacks need review. Visual duplicate signatures propose candidates and can miss matches; duplicate recycling needs Windows Recycle Bin support on the source drive.
- Tags, catalog migration and cloud-managed libraries remain deferred.
- This build is unsigned. Portable profiles require a writable local NTFS or exFAT volume reported as fixed by Windows.

## Third-party runtime source

Playback DLLs are unchanged from the 0.7.2 public release. Their [corresponding source and build configuration](https://github.com/sys-manny/stillframe-release/releases/download/v0.7.2/Stillframe-0.7.2-playback-runtime-source.zip) remain available there. Third-party notices are included in the application ZIP. `SHA256SUMS.txt` records the application and corresponding-source archive checksums.
