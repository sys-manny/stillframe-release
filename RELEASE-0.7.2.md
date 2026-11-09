# Stillframe 0.7.2

**Windows x64 · Portable ZIP · Free for personal, noncommercial use**

<p><a href="https://slint.dev/"><img src="https://raw.githubusercontent.com/slint-ui/slint/v1.18.1/logo/MadeWithSlint-logo-whitebg.png" width="118" alt="Made with Slint"></a></p>

- Browse imported folders together in All Libraries, with continuous Grid and Column scrolling and full-folder search and sort.
- Use People to scan selected folders, review local face matches, and browse named albums.
- Generate thumbnails from the sidebar while you browse. Pin a video frame to use as its thumbnail.
- Stop and resume Exact or Visual duplicate scans within one library.
- Open and generate thumbnails for JPEGs with an unset EXIF orientation.

Extract the full ZIP and open `Launch.cmd`. [Getting started](https://github.com/sys-manny/stillframe-release/blob/main/INSTALL-0.7.2.md)

## Known limits

- Tags, catalog migration, and cloud-managed libraries are outside this release.
- Thumbnails are generated on demand. Unfinished jobs stay stopped after a restart.
- Very large or changing folders can show partial results when files are unavailable or the metadata budget is reached.
- This release is unsigned. Windows may show a SmartScreen reputation warning.

## Third-party source and checksums

The playback runtime’s corresponding source and build configuration are included in the separate source ZIP below. See `runtime-notices` inside the application ZIP for license texts and notices. Verify both ZIPs using `SHA256SUMS.txt`.
