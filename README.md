<div align="center">

  <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/logo.svg" alt="OpenFishTools" width="120" height="120" />

  # OpenFishTools

  **Open-source motion graphics and video editing tools. Built for editors, runs in your browser.**

  <a href="https://github.com/openfishtools/Studio"><img src="https://img.shields.io/badge/Studio-In_Progress-9DFF00?style=for-the-badge&labelColor=121212" alt="Studio" /></a>
  <a href="https://github.com/openfishtools/web"><img src="https://img.shields.io/badge/Web-In_Progress-9DFF00?style=for-the-badge&labelColor=121212" alt="Web" /></a>
  <a href="https://github.com/openfishtools/CEP"><img src="https://img.shields.io/badge/CEP-Stable-229200?style=for-the-badge&labelColor=121212" alt="CEP" /></a>
  <a href="https://github.com/openfishtools/web-tools"><img src="https://img.shields.io/badge/Web_Tools-Active-229200?style=for-the-badge&labelColor=121212" alt="Web Tools" /></a>

</div>

---

> [!IMPORTANT]
> **Private by design.** Studio and Web Tools process media locally in your browser (WebCodecs, WebAssembly, WebGPU). Your files are never uploaded to a server.

## What we build

- **A real editor in a browser tab.** Multi-track timeline, keyframes, blend modes and an effect plugin registry, with no install.
- **Small tools that do one job well.** Compress, extract, convert, upscale, remove a background. Open, drop a file, done.
- **Native workflow helpers.** An After Effects panel for easing, auto save and conversion to Alight Motion.

---

## Showcase

### Studio: browser-based motion graphics editor

<div align="center">
  <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/screenshots/studio-desktop.png" alt="Studio desktop editor" width="100%" />
</div>

<br />

<table>
  <tr>
    <td width="30%" align="center">
      <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/screenshots/studio-mobile.png" alt="Studio mobile editor" width="100%" />
      <br /><sub><b>Mobile editor</b><br />Touch timeline and gesture controls</sub>
    </td>
    <td width="70%" valign="top">
      <h4>Highlights</h4>
      <ul>
        <li><b>Desktop suite</b> with docked inspector, track headers, playhead scrubbing and a curve graph editor.</li>
        <li><b>Mobile editor</b> with a viewport-adaptive canvas and gesture-driven timeline.</li>
        <li><b>Modular effects.</b> Each effect is one file registering to <code>FishEffectsRegistry</code>, with automatic parameter-to-timeline binding.</li>
        <li><b>Local export</b> through WebCodecs and MP4 muxing, with no cloud rendering.</li>
        <li><b>Zero-dependency dev server</b> with live reload and an optional tunnel.</li>
      </ul>
      <a href="https://github.com/openfishtools/Studio">Open the Studio repository</a>
    </td>
  </tr>
</table>

**Effect library preview**

<div align="center">
  <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/effects/glow-aura.png" width="15%" alt="Glow Aura" />
  <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/effects/deep-glow.png" width="15%" alt="Deep Glow" />
  <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/effects/chromatic-aberration.png" width="15%" alt="Chromatic Aberration" />
  <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/effects/anamorphic-flare.png" width="15%" alt="Anamorphic Flare" />
  <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/effects/rgb-split.png" width="15%" alt="RGB Split" />
  <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/effects/shatter.png" width="15%" alt="Shatter" />
</div>

---

### Web Tools: creative utilities that run client-side

<div align="center">
  <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/screenshots/web-tools-grid.png" alt="Creative Tools grid" width="100%" />
</div>

| Tool | Category | What it does |
| :--- | :--- | :--- |
| **Remove Background** | AI | Video and image matting with MediaPipe, RVM and MODNet |
| **Media Upscaler** | AI | GPU-assisted upscale with selectable enhancement presets |
| **Video Compressor** | Video | Re-encode to a target size with FFmpeg WebAssembly |
| **Audio Extractor** | Video | Pull a clean MP3 out of any video |
| **Image Sequence to Video** | Video | Turn a ZIP of frames into a video, with optional audio |
| **Video Interpolation** | Video | Raise frame rate 2x, 4x or 8x |
| **AE to AM** | Converters | After Effects beat markers to Alight Motion XML |
| **5MB XML Generator** | Converters | Slim down Alight Motion projects safely |
| **Quality method** | TikTok | Patch and compress video for higher quality uploads |
| **TikTok Downloader / Statistics** | TikTok | Download without watermark, inspect metadata |

Every tool is a self-describing module. Load it from the CDN and run it in your own page, no clone needed:

```html
<script src="https://cdn.jsdelivr.net/gh/openfishtools/web-tools/video/audio-extractor-tool.js"></script>
```

See the [web-tools README](https://github.com/openfishtools/web-tools#readme) for the full integration guide.

---

### CEP: After Effects extension panel

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>Graph Editor and Easing</h4>
      Interactive bezier handles, easing presets and an auto-apply toggle.
      <h4>AE to AM Converter</h4>
      Compositions to Alight Motion XML, with pre-comp embedding and optional expression baking.
    </td>
    <td width="50%" valign="top">
      <h4>Auto Save</h4>
      Background project backups with timestamped names.
      <h4>Layer and Transform Utilities</h4>
      Anchor grid, smart auto-crop, comp ratio and FPS changers, text animator presets.
    </td>
  </tr>
</table>

Installers for macOS (`.pkg`) and Windows (`.exe`) are on the [CEP releases page](https://github.com/openfishtools/CEP/releases).

---

## Ecosystem

| Repository | Stack | Status | Focus |
| :--- | :--- | :---: | :--- |
| [**Studio**](https://github.com/openfishtools/Studio) | JavaScript, Canvas, WebCodecs | `In Progress` | Text engine development |
| [**web**](https://github.com/openfishtools/web) | HTML, CSS, JavaScript | `In Progress` | Migrating tools to web-tools |
| [**web-tools**](https://github.com/openfishtools/web-tools) | JavaScript, FFmpeg.wasm, WebGPU | `Active` | Headless tool modules and CDN delivery |
| [**CEP**](https://github.com/openfishtools/CEP) | ExtendScript, CEP | `Stable` | Up to date, no active tasks |

```mermaid
flowchart LR
    AE["After Effects"] -->|"CEP panel"| AM["Alight Motion XML"]
    AE -->|"projects and assets"| STU["Studio"]
    STU -->|"WebCodecs export"| OUT["MP4 output"]
    WT["web-tools modules"] -->|"CDN"| WEB["web"]
    WT -->|"CDN"| YOU["Your own site"]
    WEB --> OUT
```

---

## Contributing

1. Fork the repository you want to improve.
2. Create a branch and keep changes focused.
3. Open a pull request describing what changed and why.

All projects are released under the MIT License.

<div align="center">
  <sub>OpenFishTools</sub>
</div>
