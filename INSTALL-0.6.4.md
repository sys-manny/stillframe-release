# Install Stillframe 0.6.4

For 64-bit Windows. The application includes its .NET Desktop runtime.

## Guided setup

1. Download `Stillframe-0.6.4-Setup.exe` and `Stillframe-0.6.4-win-x64.zip` from the same release into one folder.
2. Run setup and choose where Stillframe should be installed.
3. Choose shortcuts and optional addons. The desktop shortcut is selected by default; uncheck it if unwanted.
4. Review the location and choices, then select Install. Setup verifies the supplied files and shows its current stage/progress.
5. Open Stillframe and add media folders through Manage libraries.

Keep a previous installation as a fallback and use a separate location when trying this beta. Existing application-file replacement needs explicit review. Do not move the setup EXE away from its matching application ZIP before installation.

## Optional addons

The base app works without these downloads:

| Feature | Files to place beside setup |
| --- | --- |
| Local visual tag suggestions (visEngine) | `Stillframe-0.6.4-visEngine-01.sfa` **and** `Stillframe-0.6.4-visEngine-02.sfa` |
| RTX acceleration for supported NVIDIA GPUs | `Stillframe-0.6.4-RTX.sfa` |

Setup verifies the selected addons and joins the visEngine parts. Do not rename or join them manually. Optional engines remain off unless selected.

## Portable use

Extract the complete `Stillframe-0.6.4-win-x64.zip` and run the root `Stillframe.exe`. Keep the runtime, App folder, models, assets and third-party notices together. A portable copy can still share Windows-user settings/caches with another installation; a separate folder alone is not an isolated profile.

## Verify downloads

Compare files with the release's `SHA256SUMS.txt`. In PowerShell, `Get-FileHash -Algorithm SHA256 .\Stillframe-0.6.4-win-x64.zip` prints the ZIP's hash. Setup also checks the matching package and selected addons before installing.

## Upgrading and beta limits

Keep backups of important media. The application and installer are unsigned, so Windows may show a SmartScreen warning. Original media is not part of the application package.

Volume defaults to 100% and supports 0–150%, remembering your choice. **Set it to 100% or lower before returning to 0.6.3**, whose older validator rejects higher saved values.

Read `KNOWN-LIMITATIONS-0.6.4.md` and `RELEASE-0.6.4.md`. This publication uses the already verified, unchanged beta binaries; it does not add fresh-PC, owner-installation or hardware loudness acceptance.
