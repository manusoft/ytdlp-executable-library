![Static Badge](https://img.shields.io/badge/Ytdlp.FFprobe.Build-red) ![NuGet Version](https://img.shields.io/nuget/v/Ytdlp.FFprobe.Build)  ![NuGet Downloads](https://img.shields.io/nuget/dt/Ytdlp.FFprobe.Build)

# Ytdlp.FFprobe.Build

**Ytdlp.FFprobe.Build** provides the **FFprobe executable** required by **yt-dlp** and **FFmpeg** for media metadata inspection.

**FFprobe** is often used internally by **yt-dlp** to analyze audio/video streams during post-processing.

This package is designed to complement the **YTDLP-Wrapper** library and **Ytdlp.NET** library or developers who want zero-setup media processing when using **yt-dlp** in .NET applications. The **FFprobe** binary is included in the NuGet package and placed in the tools directory for easy access at build or runtime.

## ✨ Features  
- Precompiled **FFprobe executable** 
- Optimized for **yt-dlp post-processing**  
- No system-wide FFprobe installation required
- Works seamlessly with Ytdlp.Stable.Build
- Ideal for CI/CD, desktop apps, and self-contained deployments

## 📦 Package Contents

```bash
Tools/
 └─ ffprobe.exe
```

## 🚀 Usage

```bash
--ffmpeg-location <path-to-tools-folder>
```

In .NET projects, you can reference the ```tools``` directory at runtime or copy the executable to your output folder as part of your build process.

## 🔗 Related Packages
- **Ytdlp.Stable.Build** – Latest yt-dlp executable
- **Ytdlp.FFmpeg.Build** – Patched FFmpeg for post-processing

## ⚠ Disclaimer
This package does not modify **FFprobe** in any way.
**FFprobe** is distributed as a **third-party binary** under its own license.

