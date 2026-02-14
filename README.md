![Static Badge](https://img.shields.io/badge/Ytdlp.Stable.Build-red)
![NuGet Version](https://img.shields.io/nuget/v/Ytdlp.Stable.Build)
![NuGet Downloads](https://img.shields.io/nuget/dt/Ytdlp.Stable.Build)

![Static Badge](https://img.shields.io/badge/Ytdlp.FFmpeg.Build-blue)
![NuGet Version](https://img.shields.io/nuget/v/Ytdlp.FFmpeg.Build)
![NuGet Downloads](https://img.shields.io/nuget/dt/Ytdlp.FFmpeg.Build)

![Static Badge](https://img.shields.io/badge/Ytdlp.FFprobe.Build-green)
![NuGet Version](https://img.shields.io/nuget/v/Ytdlp.FFprobe.Build)
![NuGet Downloads](https://img.shields.io/nuget/dt/Ytdlp.FFprobe.Build)

![Static Badge](https://img.shields.io/badge/Ytdlp.Deno.Runtime-orange)
![NuGet Version](https://img.shields.io/nuget/v/Ytdlp.Deno.Runtime)
![NuGet Downloads](https://img.shields.io/nuget/dt/Ytdlp.Deno.Runtime)

![Static Badge](https://img.shields.io/badge/Ytdlp.Excecutable-black)
![NuGet Version](https://img.shields.io/nuget/v/ytdlp-executable)
![NuGet Downloads](https://img.shields.io/nuget/dt/ytdlp-executable)

---

# Ytdlp.Builds

**Ytdlp.Builds** is a collection of NuGet packages that provide **prebuilt executables required by yt-dlp**, packaged for easy use in **.NET applications**.

This repository exists to eliminate the need for manual downloads, PATH configuration, or external installers when working with **yt-dlp**, FFmpeg, and FFprobe, and the required JavaScript runtime (Deno).

All binaries are redistributed **unmodified** and placed in the `Tools` directory for predictable access.

---

## 📦 Available Packages

### 🔴 Ytdlp.Stable.Build

Provides the **latest stable `yt-dlp.exe`** as a NuGet package.

* Ships with the latest official yt-dlp release
* Designed to complement **Ytdlp.NET**, **YTDLP-Wrapper**, or any custom integration
* Ideal for desktop apps, automation, and CI/CD pipelines

**Executable path:**

```
Tools\yt-dlp.exe
```

---

### 🔵 Ytdlp.FFmpeg.Build

Provides the **FFmpeg executable** required by yt-dlp for media post-processing.

* Enables audio/video merging and conversion, and format handling
* No system-wide FFmpeg installation required
* Optimized for use with yt-dlp

**Executable path:**

```
Tools\ffmpeg.exe
```

---

### 🟢 Ytdlp.FFprobe.Build

Provides the **FFprobe executable** used for media inspection and metadata analysis.

* Used internally by yt-dlp and FFmpeg
* Required for certain post-processing workflows

**Executable path:**

```
Tools\ffprobe.exe
```

---


### 🟠 Ytdlp.Deno.Runtime
Provides the official **deno.exe** (Windows x64) — the recommended JavaScript runtime for yt-dlp.

- Required since yt-dlp 2025.11.12+ for YouTube signature extraction & JS challenges
- Official stable binary from denoland/deno (unmodified)
- Deno is yt-dlp's **default and highest-priority** external runtime
- No global Deno installation needed

**Executable path:**

```
Tools\deno.exe
```

---


### ⚫ Ytdlp.Executable
(Alternative / legacy package name – provides `yt-dlp.exe` in a different layout)

**Executable path:**
```
Tools\yt-dlp.exe
```


## ✨ Features

* Latest stable binaries for yt-dlp, FFmpeg, FFprobe, and Deno
* Standalone NuGet packages — install only what you need
* Clean, predictable `Tools` directory layout
* No installers, no PATH configuration
* Works with any .NET application or wrapper library
* Self-contained setup for full yt-dlp functionality (including YouTube)

---

## 🔗 Supported Sites

yt-dlp supports **thousands of websites**:

👉 [https://github.com/yt-dlp/yt-dlp/blob/master/supportedsites.md](https://github.com/yt-dlp/yt-dlp/blob/master/supportedsites.md)

---

## 📜 License & Attribution

### This repository

The NuGet packaging logic and metadata are licensed under the **MIT License**.

### Third-party software

This repository redistributes **unmodified third-party binaries**:

* **yt-dlp**
  Licensed under the **Unlicense**
  [https://github.com/yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp)

* **FFmpeg / FFprobe**
  Licensed under **LGPL or GPL**, depending on build configuration
  [https://ffmpeg.org](https://ffmpeg.org)

* **Deno**  
  Licensed under the **MIT License**  
  [https://deno.com](https://deno.com) • [https://github.com/denoland/deno](https://github.com/denoland/deno)

This project is **not affiliated with or endorsed by** the yt-dlp, FFmpeg, or Deno projects.

---

## 🧠 Versioning

Each NuGet package is **versioned independently** and follows (or closely tracks) the version of the tool it ships.

Packaging-only changes may use an additional revision number when required.

---

## ⭐ Why Ytdlp.Builds?

Because using yt-dlp in .NET should be as simple as:

```bash
dotnet add package Ytdlp.Stable.Build
dotnet add package Ytdlp.FFmpeg.Build
dotnet add package Ytdlp.FFprobe.Build
dotnet add package Ytdlp.Deno.Runtime
```

No extra downloads. No environment setup. Just works.


### Notes on this version

- Added **Ytdlp.Deno.Runtime** with orange badge (common color for JS-related tools, contrasts nicely)
- Included a short explanation why Deno is needed (YouTube JS challenges)
- Kept the color coding consistent with your earlier badges
- Mentioned that all binaries are unmodified
- Included the legacy `Ytdlp.Executable` package (assuming it's still published)
- Added Deno license attribution
