# Kodak Build-It

**Build-It** was Kodak's official software for premastering **Photo CD** disc images (PMF) prior to writing them to physical media.
This project restores, patches, and updates the original Build-It tools so they can run reliably on **modern versions of Windows**.

[https://github.com/andkrau/kodak_build-it](https://github.com/andkrau/kodak_build-it)

---

## What’s Been Fixed / Changed

### Compatibility Fixes
- Fixed crash when opening file dialogs
- Fixed crash just after PMF creation
- Bypassed code that crashes on older and newer versions of Windows
- Removed lockups caused by missing/failed file associations

### Feature Removals / Simplifications
- Removed non–Photo CD options
- Disabled "preferred writer" dropdown (obsolete hardware)
- Disabled ability to output directly to disc — modern systems lack compatible writers

---

## Building

This project uses two main tools:

- **Hexagon** for applying binary patches
  https://github.com/Coolcord/Hexagon
- **Resource Hacker** for updating and rebuilding Win32 resources
  https://www.angusj.com/resourcehacker

---

## Running

The applications run on:

- Windows 11
- Windows 10
- Likely compatible with Windows 7/8

**Direct disc writing is intentionally disabled.**
Use [PMF2BIN](https://github.com/andkrau/pmf2bin) to convert PMF files to BIN/CUE.

---

## Included Tools

| Tool | Purpose |
|------|---------|
| **Build-It** | Main Photo CD premastering tool (creates PMF files) |
| **ScriptMaker** | Generates and edits project scripts used by Build-It |

---

## Notes on Photo CD Preservation

While a market failure, Kodak's Photo CD format is a historically significant image format.
By restoring Build-It, this project aims to keep Photo CD creation functional without legacy hardware.

---

## Contributing

Pull requests are welcome!
Patches that increase compatibility or stability are encouraged.
