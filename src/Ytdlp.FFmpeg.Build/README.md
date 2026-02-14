![Static Badge](https://img.shields.io/badge/Ytdlp.FFmpeg.Build-red) ![NuGet Version](https://img.shields.io/nuget/v/Ytdlp.FFmpeg.Build)  ![NuGet Downloads](https://img.shields.io/nuget/dt/Ytdlp.FFmpeg.Build)

# Ytdlp.FFmpeg.Build

**Ytdlp.FFmpeg.Build** provides a **prebuilt FFmpeg executable** bundled specifically for use with **yt-dlp**.

This package is designed to complement the **YTDLP-Wrapper** library and **Ytdlp.NET** library or developers who want zero-setup media processing when using **yt-dlp** in .NET applications. The **FFmpeg** binary is included in the NuGet package and placed in the tools directory for easy access at build or runtime.

## ✨ Features  
- Precompiled **FFmpeg executable** 
- Optimized for **yt-dlp post-processing**  
- No system-wide FFmpeg installation required
- Works seamlessly with Ytdlp.Stable.Build
- Ideal for CI/CD, desktop apps, and self-contained deployments

## 📦 Package Contents

```bash
Tools/
 └─ ffmpeg.exe
```

## 🚀 Usage

```bash
--ffmpeg-location <path-to-tools-folder>
```

In .NET projects, you can reference the ```tools``` directory at runtime or copy the executable to your output folder as part of your build process.

## 🔗 Related Packages
- **Ytdlp.Stable.Build** – Latest yt-dlp executable
- **Ytdlp.FFprobe.Build** – Patched FFprobe for media inspection

## ⚠ Disclaimer
This package does not modify **FFmpeg** in any way.
**FFmpeg** is distributed as a **third-party binary** under its own license.

