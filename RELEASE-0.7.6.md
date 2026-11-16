# Stillframe 0.7.6 Falcon

**Windows x64 · Portable ZIP · Free for personal, noncommercial use**

This update adds selected-photo People scans, resizable Details, and cross-library duplicate review. It retains direct startup on supported exFAT SSDs. To update an existing 0.7.6 installation, close Stillframe and replace the root `Stillframe.exe`.

- Carry a selected photo between People and All Libraries, and open its source folder from a face card.
- Run **Scan people** on one or more selected photos from the Grid or Column right-click menu.
- Drag the Details divider to resize the panel in Grid, Column, and People.
- Review Exact and Visual duplicates across libraries and save Keep choices. Within one library, process discards from both tabs in one confirmation.
- Reopen saved folder pages and use available photo dimensions to size Staggered Grid cards before display.

- Review suggested People stacks inline and open or close them from the same badge. Compare source photos with face outlines before assigning names. **Ignore** covers both false detections and unwanted duplicates such as reflections.
- YuNet detects faces. OpenFace and SFace score matches for suggested stacks. Previously scanned records stay readable.
- Generate missing thumbnails from the sidebar while you browse. Manual video frame selection remains available.
- Staggered Grid uses saved dimensions and reads missing photo dimensions in the background. Nearby thumbnails preload during scrolling.
- The viewer and thumbnail generator handle the reported JPEGs with an extra entropy sequence after the first complete image, along with expanded PNG and WebP support.

Extract the full ZIP and open `Stillframe.exe`. [Getting started](https://github.com/sys-manny/stillframe-release/blob/main/INSTALL-0.7.6.md)

## Known limits

- Tags, catalog migration, and cloud-managed libraries remain deferred.
- Animated, lossless, and alpha WebP are outside the current photo viewer's WebP support. Very large or changing folders can return partial results when files are unavailable or when the metadata budget is reached.
- Suggested face stacks need review. The report of thumbnails reverting to placeholders during a People scan is deferred unless it recurs.
- This build is unsigned. Windows may show a SmartScreen reputation warning.

## Third-party runtime source

The four playback DLLs match the 0.7.2 public release byte for byte. Their [corresponding source and build configuration](https://github.com/sys-manny/stillframe-release/releases/download/v0.7.2/Stillframe-0.7.2-playback-runtime-source.zip) remain available there. The new ZIP includes third-party notices. `SHA256SUMS.txt` checks both archives.
