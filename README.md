<p align="center"><img src="assets/stillframe-frost.png" width="88" alt="Stillframe aperture logo"></p>
<h1 align="center">Stillframe 0.7.9</h1>
<p align="center">Browse, organize, and review photos and videos in their existing folders.</p>
<p align="center">
  <a href="https://github.com/sys-manny/stillframe-release/releases/download/v0.7.9/Stillframe-0.7.9-win-x64.zip"><strong>Download for Windows x64</strong></a>
  &nbsp; · &nbsp; <a href="INSTALL-0.7.9.md">Getting started</a>
  &nbsp; · &nbsp; <a href="https://github.com/sys-manny/stillframe-release/issues">Report a problem</a>
</p>
<p align="center"><a href="https://slint.dev/"><img src="assets/made-with-slint.png" width="118" alt="Made with Slint"></a></p>

## Light and dark modes

| Light | Dark |
| --- | --- |
| [![Stillframe Grid in light mode with the Orchid accent](assets/stillframe-076-grid-light.png)](assets/stillframe-076-grid-light.png) | [![Stillframe Grid in dark mode with the Orchid accent](assets/stillframe-076-grid.png)](assets/stillframe-076-grid.png) |

In **Preferences → Theme**, choose **Light**, **Dark**, or **System** to follow Windows. Both views show the same photos from the disposable demo library.

### Accent colors

Under **Preferences → Accent**, choose **Sage**, **Arctic**, **Rose**, or **Orchid**. Each accent works in both themes.

<img src="assets/stillframe-076-accents.png" width="392" alt="Stillframe Accent menu showing Sage green, Arctic blue, Rose pink, and Orchid purple">

## Latest 0.7.9 update

- **Tag photos and videos.** Add or remove tags in Details for one file or a selection. Filter tags together with filename search, media type and sorting, in a folder or across libraries.
- **Reuse tag names.** Names are shared across libraries and remembered after restart. Type three matching characters, such as `bru` for `brunette`, then click a suggestion or choose it with the keyboard. Suggestions appear in both Add tags and Filter tags.
- **Keep Column scrolling in reach.** The vertical scrollbar stays at the visible edge with Details open; headers remain aligned as you scroll horizontally.
- **Generate while watching.** Video playback reserves its own verified file rather than blocking unrelated thumbnail work. Same-file protection and source checks remain.
- **Keep People stacks where you left them.** Naming a face or stack preserves the stacks you opened or closed.
- **Preserve your portable profile.** Keep the complete `app/Stillframe` folder when upgrading to retain settings, libraries, tags, People data, saved thumbnails and manual video frames.

## What's new since 0.7.2

- **People.** Stillframe uses YuNet to detect faces and OpenFace with SFace to suggest groups. Click a stack's count badge to open or close it in place. Compare suggested matches using source photos with face outlines, and ignore unwanted detections such as reflections.
- **Thumbnails.** One **Generate thumbnails** button fills in missing thumbnails for the selected files, folder, or library. Generation runs in the background, and you can still choose a frame for a video thumbnail.
- **Browsing.** Staggered Grid uses saved dimensions to size cards early. It keeps recently viewed thumbnails in memory and preloads the next screen.
- **Portable startup.** Open `Stillframe.exe` directly. The splash shows startup progress while the app opens.
- **Format support.** The viewer and thumbnail generator handle more JPEG, PNG, and WebP files, including the reported JPEGs with extra data after the first complete image.

## Photo viewer

Use the filmstrip to move through a folder. Fit, zoom, pan, and rotate photos in the viewer.

<img src="assets/stillframe-076-viewer.png" alt="Stillframe photo viewer with a car at sunset, zoom controls, and the folder filmstrip" width="1200">

*Photo viewer rendered with the same demo library.*

## Run the portable app

1. [Download the ZIP](https://github.com/sys-manny/stillframe-release/releases/download/v0.7.9/Stillframe-0.7.9-win-x64.zip) and extract the entire archive to a writable folder.
2. Open `Stillframe.exe`.
3. Choose **Import** to add a media folder.

To upgrade from a recent portable release, close Stillframe and preserve the complete `app/Stillframe` profile when moving to the new release. It contains settings, registered libraries, tags, People data, saved thumbnails, and manual video thumbnail choices. Keep the same paths for the original media.

[Getting started](INSTALL-0.7.9.md) · [Release notes and known limits](RELEASE-0.7.9.md) · [SHA-256 checksums](https://github.com/sys-manny/stillframe-release/releases/download/v0.7.9/SHA256SUMS.txt)

The portable app supports writable local NTFS and exFAT drives that Windows reports as fixed. To carry your settings and thumbnails to another drive or PC, close Stillframe and copy the entire extracted application folder.

## Previous releases

Earlier downloads and their documentation are available on the [Releases page](https://github.com/sys-manny/stillframe-release/releases).

## License and runtime source

Stillframe is free for personal, noncommercial use under the [Stillframe Personal Use License](LICENSE). Media and face processing run locally.

0.7.9 ships with the same playback DLLs as the 0.7.2 public release. [Corresponding playback runtime source](https://github.com/sys-manny/stillframe-release/releases/download/v0.7.2/Stillframe-0.7.2-playback-runtime-source.zip)
