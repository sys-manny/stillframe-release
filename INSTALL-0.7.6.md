# Getting started with Stillframe 0.7.6

1. [Download the Windows x64 ZIP](https://github.com/sys-manny/stillframe-release/releases/download/v0.7.6/Stillframe-0.7.6-win-x64.zip).
2. Extract the entire archive to a writable folder and open `Stillframe.exe`.
3. Choose **Import** and pick one of your existing media folders.

Use a writable local NTFS or exFAT drive that Windows reports as fixed. For an existing 0.7.6 installation, close Stillframe and replace the root `Stillframe.exe` with the one from the updated ZIP. Your portable profile stays in `app/Stillframe`.

To reuse settings and thumbnails from 0.7.5, close both copies of Stillframe. Copy the complete `app/Stillframe` folder from 0.7.5 into the new release's `app` folder before launch. Keep the previous copy until your libraries and thumbnails appear as expected. If you move to another PC, keep the app folder together and reconnect any media paths that differ. Original media stays in its registered folders.

If you're upgrading from 0.6.4, import your folders into the new release. Migration of old catalogs and tags is deferred.

This build is unsigned. Windows may show a SmartScreen reputation warning. Use the [published checksums](https://github.com/sys-manny/stillframe-release/releases/download/v0.7.6/SHA256SUMS.txt) to verify the ZIP.
