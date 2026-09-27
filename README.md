# ◈ FRAMER — Smart Frame Extractor

> Extract frames from any drone or camera video — with or without GPS — for photogrammetry, 3D reconstruction, and any frame-based workflow.


<img width="1913" height="1128" alt="Screenshot 2026-09-27 210452" src="https://github.com/user-attachments/assets/25e28c1b-205a-4861-a357-b56199ad288e" />


---

## What it does

FRAMER takes a video file and outputs JPEG frames ready for WebODM, ODM, Metashape, RealityCapture, DroneDeploy, or any software that works with images.

Works with **360° equirectangular** footage (DJI Avata, Osmo 360, etc.) and **regular flat** footage (DJI Mini, Air, Mavic, phone, action cam, any camera).

GPS is **optional** — FRAMER works with or without an SRT telemetry file.

---

## Features

- **GPS-distance sampling** — extract frames based on drone movement so overlap stays consistent regardless of speed *(requires SRT)*
- **Time Interval mode** — extract frames every N seconds, no GPS needed
- **18 virtual camera directions** — nadir, zenith, oblique 45°, horizontal 0° (cardinal + diagonal) — *360° mode only*
- **Equirectangular → perspective reprojection** — each direction becomes a proper rectilinear image — *360° mode only*
- **GPS EXIF + DJI XMP** — coordinates and gimbal orientation embedded in every JPEG *(when SRT is available)*
- **Sharpness filter** — automatically skip blurry frames (Gentle / Strict)
- **Time range** — extract only a specific segment of the video
- **Virtual Tour** — build a standalone 360° HTML tour with minimap from any 360° footage

---

## Installation

Download `FRAMER_setup_v1.0.0.exe` from [Releases](../../releases) and run the installer.
No Python required — fully self-contained.

**Requirements:** Windows 10 / 11 (x64)

---

## Usage

1. Load your video (MP4 / MOV)
2. Choose **360°** or **Regular** capture type
3. Choose **GPS sampling** (with SRT) or **Time Interval** (no GPS needed)
4. Set overlap %, directions, and optional time range
5. Click **Extract Frames**
6. Import the output folder into your software of choice

---

## Virtual Tour

Switch to the **Virtual Tour** tab to build a self-contained `.html` panoramic tour from any 360° footage. No server needed — open in any browser.

---

## Support

If FRAMER saves you time, consider buying me a coffee ☕

[![Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/opsabove)

---

## License

MIT
