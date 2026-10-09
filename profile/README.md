<div align="center">

  <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/brand-banner.svg" alt="OpenFishTools Logo" width="180" height="180" style="border-radius: 40px; box-shadow: 0 12px 32px rgba(34, 146, 0, 0.25);" />

  # OpenFishTools

  ### *The Open-Source Creative Ecosystem for Motion Designers & Visual Artists*

  <p align="center">
    <strong>Bridging desktop power with modern, zero-latency client-side browser editing.</strong>
  </p>

  <p align="center">
    <a href="https://github.com/openfishtools"><img src="https://img.shields.io/badge/GitHub-openfishtools-121212?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Org" /></a>
    <a href="#-ecosystem"><img src="https://img.shields.io/badge/Ecosystem-4_Projects-229200?style=for-the-badge&logoColor=white" alt="Ecosystem" /></a>
    <a href="#license"><img src="https://img.shields.io/badge/License-MIT-9DFF00?style=for-the-badge&labelColor=1a2e00&color=9DFF00" alt="License: MIT" /></a>
    <a href="https://github.com/cutefishaep"><img src="https://img.shields.io/badge/Crafted_by-cutefishaep-6BAE00?style=for-the-badge" alt="Author" /></a>
  </p>

  <p align="center">
    <a href="#-about-openfishtools">About</a> •
    <a href="#-key-pillars">Key Pillars</a> •
    <a href="#-ecosystem">Ecosystem</a> •
    <a href="#-architecture--workflow">Workflow</a> •
    <a href="#-getting-started">Get Started</a> •
    <a href="#-community--support">Community</a>
  </p>

</div>

---

## 🌊 About OpenFishTools

Traditional motion graphics and video editing workflows are frequently locked inside heavy proprietary software or throttled by expensive cloud rendering pipelines. 

**OpenFishTools** is built to rethink creative tooling:
- **Desktop Workflow Optimization**: Native extensions for Adobe After Effects that remove repetitive bottlenecks.
- **Pure Client-Side Video Creation**: High-performance browser-based non-linear editing using WebCodecs and GPU-accelerated canvas compositing.
- **Cross-Platform Portability**: Seamless conversion of desktop compositions to mobile animation environments (AE ➔ Alight Motion).

---

## ✨ Key Pillars

<table width="100%">
  <tr>
    <td width="50%" valign="top">
      <h3>⚡ 100% Client-Side & Private</h3>
      <p>Zero cloud render queues. Video encoding, frame compositing, and shader processing happen entirely on the user's hardware via WebCodecs and MP4-muxer. Your media never leaves your machine.</p>
    </td>
    <td width="50%" valign="top">
      <h3>🎛️ Precision Curve & Motion Control</h3>
      <p>Professional Bezier easing graphs, real-time curve manipulators, and automated preset injections designed for animators who obsess over motion cadence and fluid timing.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🔄 Universal Composition Bridges</h3>
      <p>Direct translation pipeline from complex After Effects project hierarchies into lightweight mobile-compatible animation project files with recursive pre-composition nesting.</p>
    </td>
    <td width="50%" valign="top">
      <h3>🧩 Modular Visual Effects Registry</h3>
      <p>A pluggable registry architecture featuring 50+ built-in optical, chromatic, distortion, and 3D transform modules with instant timeline parameter binding.</p>
    </td>
  </tr>
</table>

---

## 📦 Ecosystem

OpenFishTools consists of specialized repositories designed to work seamlessly both standalone and together:

| Project | Role | Highlights | Repository |
| :--- | :--- | :--- | :---: |
| <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/logo.svg" width="28" height="28" /> **Studio** | **Web NLE & Motion Engine** | • Desktop AE-style layout & mobile touch canvas<br>• Hardware-accelerated WebCodecs 4K/60fps export<br>• Multi-track keyframe interpolation & curve editor<br>• 50+ modular GPU shaders & visual effects | [**Open Studio**](https://github.com/openfishtools/Studio) |
| <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/logo.svg" width="28" height="28" /> **CEP** | **After Effects Panel Extension** | • Interactive Bezier curve easing graph with auto-apply<br>• AE to Alight Motion (AM) composition XML converter<br>• Smart non-disruptive auto-save backup system<br>• Layer alignment, auto-crop, and utility tools | [**Open CEP**](https://github.com/openfishtools/CEP) |
| <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/logo.svg" width="28" height="28" /> **Web** | **Portal & Services Platform** | • Unified web platform, preset index, and documentation<br>• Edge-deployed on Cloudflare Workers & Pages<br>• Community templates, scripts, and asset library | [**Open Web**](https://github.com/openfishtools/web) |
| <img src="https://raw.githubusercontent.com/openfishtools/.github/main/profile/assets/logo.svg" width="28" height="28" /> **Web Tools** | **Lightweight Utilities** | • Rapid keyframe data converters & preset builders<br>• Online animation calculators and asset formatters<br>• Zero-install standalone browser helpers | [**Open Tools**](https://github.com/openfishtools/web-tools) |

---

## 🔁 Architecture & Workflow

```mermaid
flowchart LR
    subgraph Desktop["🖥️ Desktop Suite"]
        AE["Adobe After Effects"] --> CEP["OpenFishTools CEP"]
        CEP --> Easing["Interactive Graph Editor"]
        CEP --> AutoSave["Smart Background Backup"]
        CEP --> Converter["AE ➔ Alight Motion XML"]
    end

    subgraph Browser["🌐 Web Creative Suite"]
        Studio["OpenFishTools Studio (NLE)"] --> Timeline["Multi-Track Timeline"]
        Timeline --> FX["Modular FX Registry (50+ Shaders)"]
        FX --> Canvas["Compositor Engine"]
        Canvas --> WebCodecs["WebCodecs Hardware Export"]
    end

    subgraph Hub["☁️ Hub & Web Services"]
        WebPortal["Web Portal & Docs"] --> Assets["Presets & Asset Hub"]
        WebTools["Web Tools"] --> Helpers["Keyframe & Format Utilities"]
    end

    Converter -.-> Mobile["📱 Alight Motion & Mobile"]
    WebCodecs --> MP4["🎬 Rendered Video (MP4)"]
    Desktop <===> Browser
```

---

## 🚀 Getting Started

Select the tool tailored to your workflow:

- **Using After Effects?**
  Head over to [**openfishtools/CEP**](https://github.com/openfishtools/CEP) and grab the one-click installer (`.pkg` for macOS or `.exe` for Windows).
- **Want to edit in the browser?**
  Check out [**openfishtools/Studio**](https://github.com/openfishtools/Studio) to run the zero-dependency local dev server and start editing immediately with client-side GPU export.
- **Looking for online tools and presets?**
  Visit [**openfishtools/web**](https://github.com/openfishtools/web) and [**openfishtools/web-tools**](https://github.com/openfishtools/web-tools).

---

## 🤝 Community & Contributing

We welcome contributions from motion designers, shader programmers, web developers, and creative minds!

- 🐛 **Found a bug?** Open an issue in the respective repository.
- 💡 **Have a feature idea?** Start a discussion or suggest a new modular effect.
- 🛠️ **Want to submit code?** Pull requests are warmly welcomed across all sub-projects.

---

<div align="center">

  <sub>Crafted with passion for creators by <a href="https://github.com/cutefishaep"><strong>cutefishaep</strong></a> & the OpenFishTools community.</sub>

  <br />

  [![MIT License](https://img.shields.io/badge/License-MIT-9DFF00.svg?style=flat-square)](LICENSE)

</div>
