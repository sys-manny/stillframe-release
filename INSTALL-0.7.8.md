# Getting started with Stillframe 0.7.8

1. [Download the Windows x64 ZIP](https://github.com/sys-manny/stillframe-release/releases/download/v0.7.8/Stillframe-0.7.8-win-x64.zip).
2. Extract the entire archive to a writable folder and open `Stillframe.exe`.
3. Choose **Import** and pick one of your existing media folders.

Use a writable local NTFS or exFAT drive that Windows reports as fixed. Keep `app` and `runtime-notices` beside the root executable. The download contains application files only; a fresh extraction creates its own profile.

## Keep settings and thumbnails when upgrading

Close both copies of Stillframe. Keep a backup of your existing complete `app/Stillframe` folder, then move or copy that folder into the new release's `app` folder before launching it. Preserve the entire profile together: settings, registered libraries, saved thumbnails, and manual video thumbnail choices belong to that profile. Keep the existing media paths available.

To move to another drive or PC, close Stillframe and copy the entire extracted application folder, including `app/Stillframe`. Original media stays in its registered folders; reconnect media paths if they differ on the other PC.

If you're upgrading from 0.6.4, import your folders into the new release. Migration of old catalogs and tags remains deferred.

This build is unsigned. Windows may show a SmartScreen reputation warning. Use the [published checksums](https://github.com/sys-manny/stillframe-release/releases/download/v0.7.8/SHA256SUMS.txt) to verify the ZIP.
