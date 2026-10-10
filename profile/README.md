<div align="center">

  <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/logo.svg" alt="OpenFishTools" width="120" height="120" />

  # OpenFishTools

  **Open-source motion graphics and video editing tools.**

  <a href="https://github.com/openfishtools/Studio"><img src="https://img.shields.io/badge/Studio-In_Progress-9DFF00?style=for-the-badge&labelColor=121212" alt="Studio" /></a>
  <a href="https://github.com/openfishtools/web"><img src="https://img.shields.io/badge/Web-In_Progress-9DFF00?style=for-the-badge&labelColor=121212" alt="Web" /></a>
  <a href="https://github.com/openfishtools/CEP"><img src="https://img.shields.io/badge/CEP-Stable-229200?style=for-the-badge&labelColor=121212" alt="CEP" /></a>
  <a href="https://github.com/openfishtools/web-tools"><img src="https://img.shields.io/badge/Web_Tools-Active-229200?style=for-the-badge&labelColor=121212" alt="Web Tools" /></a>

</div>

---

## Projects

<div align="center">
<table>
  <tr>
    <td align="center" width="25%">
      <a href="https://github.com/openfishtools/CEP"><img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/projects/cep.svg" width="96" height="96" alt="CEP" /></a>
      <br /><sub><b>CEP</b></sub>
    </td>
    <td align="center" width="25%">
      <a href="https://github.com/openfishtools/Studio"><img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/projects/studio.svg" width="96" height="96" alt="Studio" /></a>
      <br /><sub><b>Studio</b></sub>
    </td>
    <td align="center" width="25%">
      <a href="https://github.com/openfishtools/web"><img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/projects/web.svg" width="96" height="96" alt="web" /></a>
      <br /><sub><b>web</b></sub>
    </td>
    <td align="center" width="25%">
      <a href="https://github.com/openfishtools/web-tools"><img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/projects/web-tools.svg" width="96" height="96" alt="web-tools" /></a>
      <br /><sub><b>web-tools</b></sub>
    </td>
  </tr>
</table>
</div>

- **Studio**: the standalone version of CEP. It has its own timeline, keyframes and effects, so After Effects is not required.
- **Web Tools**: small utilities for video, audio, image and Alight Motion files.
- **CEP**: an After Effects panel for easing, auto save and conversion to Alight Motion. Requires After Effects.

---

## Showcase

### Studio

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

### Web Tools

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

Each tool is a standalone script. It can be loaded from the CDN without cloning the repository:

```html
<script src="https://cdn.jsdelivr.net/gh/openfishtools/web-tools/video/audio-extractor-tool.js"></script>
```

See the [web-tools README](https://github.com/openfishtools/web-tools#readme) for the full integration guide.

---

### CEP

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


---

## Contributing

1. Fork the repository you want to improve.
2. Create a branch and keep changes focused.
3. Open a pull request describing what changed and why.

## Licenses

Each repository has its own license. Check the `LICENSE` file before reusing code.

| Repository | License |
| :--- | :--- |
| Studio | MIT |
| CEP | MIT |
| web | CC BY-NC-ND 4.0 |
| web-tools | CC BY-NC 4.0 |

<div align="center">
  <sub>OpenFishTools</sub>
</div>
