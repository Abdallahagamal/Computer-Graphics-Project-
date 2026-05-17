<div align="center">

```
██████╗ ██████╗  █████╗ ██████╗ ██╗  ██╗██╗ ██████╗███████╗
██╔════╝ ██╔══██╗██╔══██╗██╔══██╗██║  ██║██║██╔════╝██╔════╝
██║  ███╗██████╔╝███████║██████╔╝███████║██║██║     ███████╗
██║   ██║██╔══██╗██╔══██║██╔═══╝ ██╔══██║██║██║     ╚════██║
╚██████╔╝██║  ██║██║  ██║██║     ██║  ██║██║╚██████╗███████║
 ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝     ╚═╝  ╚═╝╚═╝ ╚═════╝╚══════╝
```

#  Computer Graphics Suite

**A full-featured 2D graphics engine built from scratch — no shortcuts, no shortcuts, no shortcuts.**  
*Every pixel placed by hand. Every algorithm written by algorithm.*

![Platform](https://img.shields.io/badge/Platform-Windows-0078D4?style=for-the-badge&logo=windows)
![Language](https://img.shields.io/badge/Language-C%23-239120?style=for-the-badge&logo=csharp)
![Framework](https://img.shields.io/badge/.NET-10.0-512BD4?style=for-the-badge&logo=dotnet)
![UI](https://img.shields.io/badge/UI-WinForms-68217A?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)

*Designed by **Abdallah Gamal***

</div>

---

## ✨ What Is This?

This is a **computer graphics playground** — a WinForms application implementing the core algorithms taught in computer graphics courses, all rendered from scratch using low-level pixel manipulation. No `Graphics.DrawLine()` shortcuts. No `DrawEllipse()` cheats. Just raw math, pixels, and passion.

Draw lines, circles, ellipses, Bézier curves, and more. Apply clipping algorithms. Fill shapes. Watch the algorithms come to life on a dark grid canvas.

---

##  Screenshots

<div align="center">

### The IDE — Where It All Comes Together
> Visual Studio 2022 · WinForms Designer · Dark Theme

![IDE View]([screenshots/ide-view.png](https://github.com/user-attachments/assets/9434a3b9-a4d0-49e3-83f8-27ac232e4333))

---

### The App in Action — 52 Shapes and Counting
> Circle Bresenham active · Multi-color rendering · Mouse coords live

![App Running]([screenshots/app-running.png](https://github.com/user-attachments/assets/bffe219a-f128-41ff-9056-7f173e0358f0))

</div>

---

##  Algorithms Implemented

###  Lines
| Algorithm | Description |
|-----------|-------------|
| **DDA** | Digital Differential Analyzer — the classic |
| **Bresenham's Line** | Integer-only, pixel-perfect line drawing |
| **Midpoint Line** | Decision parameter approach |

###  Circles
| Algorithm | Description |
|-----------|-------------|
| **Bresenham's Circle** | 8-way symmetry, integer arithmetic |
| **Midpoint Circle** | Decision variable circle rasterization |

###  Ellipses
| Algorithm | Description |
|-----------|-------------|
| **Midpoint Ellipse** | Two-region ellipse drawing algorithm |

###  Curves
| Algorithm | Description |
|-----------|-------------|
| **Bézier Curves** | Smooth parametric curves via control points |
| **Hermite Curves** | Tangent-controlled curve interpolation |
| **B-Spline** | Basis spline for smooth multi-segment curves |
| **Cardinal Spline** | Tension-controlled interpolating splines |

###  Filling
| Algorithm | Description |
|-----------|-------------|
| **Flood Fill** | Recursive region filling from seed point |
| **Scan Line Fill** | Edge-sorted horizontal scan filling |

###  Clipping
| Algorithm | Description |
|-----------|-------------|
| **Cohen-Sutherland** | Region-code line clipping |
| **Liang-Barsky** | Parametric line clipping |
| **Sutherland-Hodgman** | Polygon clipping against a convex region |

### 🌀 Bonus Features
| Feature | Description |
|---------|-------------|
| **Polar Ellipse** | Ellipse drawn in polar coordinates |
| **Cardinal Spline (advanced)** | Extended with tension parameter control |

---

##  Features

-  **Dark grid canvas** — every drawing stands out
-  **10-color palette** — Purple, Green, Orange, Pink, Blue, Yellow, Red, White, Gray, Black
-  **Live mouse coordinates** — X/Y displayed in real time
-  **Shape counter** — tracks every shape drawn this session
-  **Tool sidebar** — freehand, line, curve, circle, ellipse, fill, eraser
-  **Menu bar** — organized by algorithm category
-  **Clear canvas** — start fresh anytime
-  **Save/Load** — preserve your artwork

---

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) *(required)*
- [Visual Studio 2022](https://visualstudio.microsoft.com/) with **Windows Desktop Development** workload
  - Make sure `.NET desktop development` is checked during install
- Windows 10 or later

###  Font Setup

This project uses the **Kenon** font for the UI.

1. Download **Kenon** font (`.ttf` or `.otf`)
2. Right-click the font file → **Install for all users**
3. Restart Visual Studio if it was open

> ⚠️ If the font isn't installed, the UI labels will fall back to a default system font.

---

### 📦 Installation & Running

#### Option 1 — Visual Studio (Recommended)

```bash
# 1. Clone the repository
git clone https://github.com/Abdallahagamal/Computer-Graphics-Project-.git

# 2. Open the solution
# Double-click: WinFormsApp1.sln
```

Then in Visual Studio:
1. Open `WinFormsApp1.sln`
2. Set build configuration to **Debug** or **Release**
3. Target: **Any CPU**
4. Press **F5** or click ▶ **Run**

#### Option 2 — .NET CLI

```bash
# Clone
git clone https://github.com/Abdallahagamal/Computer-Graphics-Project-.git
cd Computer-Graphics-Project-

# Build
dotnet build

# Run
dotnet run --project WinFormsApp1
```

---

## 🕹️ How to Use

| Action | How |
|--------|-----|
| **Select algorithm** | Use the top menu bar (Lines → Bresenham, Circles → Midpoint, etc.) |
| **Pick a color** | Click any color swatch in the right panel |
| **Draw a shape** | Click and drag on the dark canvas |
| **See current algorithm** | Check "ACTIVE ALGORITHM" in the top-right panel |
| **Track coordinates** | Watch X/Y update live as you move your mouse |
| **Count shapes** | "SHAPES DRAWN" counter increments automatically |
| **Clear canvas** | File → Clear (or use the eraser tool) |
| **Apply clipping** | Select a clipping algorithm, then define clip region |
| **Fill a shape** | Select Flood Fill or Scan Line, click inside a closed shape |

---

## 🗂️ Project Structure

```
Computer-Graphics-Project-/
├── Form1.cs                  # Main form — UI + event wiring
├── Form1.Designer.cs         # WinForms auto-generated layout
├── ClippingAlgorithms.cs     # Cohen-Sutherland, Liang-Barsky, Sutherland-Hodgman
├── PolarEllipse.cs           # Polar coordinate ellipse drawing
├── WinFormsApp1.csproj       # Project config (.NET 10, WinForms)
├── Program.cs                # Entry point
└── README.md                 # You are here
```

---

##  Built With

| Technology | Purpose |
|------------|---------|
| **C# 13** | Core language |
| **.NET 10** | Runtime & SDK |
| **WinForms** | UI framework |
| **GDI+** | Low-level pixel drawing |
| **Visual Studio 2022** | IDE |
| **Kenon Font** | Typography |

---

##  Academic Context

This project implements the fundamental algorithms from **Computer Graphics** coursework:

- Rasterization (scan conversion) of geometric primitives
- Parametric and interpolating curve generation  
- Region-based clipping algorithms
- Area-filling techniques

All algorithms implemented **from scratch** — no GDI+ shape functions used for the core drawing logic.

---

## 👥 Team

<div align="center">

*Five minds. One canvas. Infinite pixels.*

| 👤 Name | 🔗 LinkedIn |
|---------|------------|
| **Abdallah Gamal** | [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/abdallah-gamal-731096162/) |
| **Esraa Ahmed** | [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/esraa-ahmed-01418b362/) |
| **Esraa Mohamed** | [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/esraa-mohamed-a4a7b7282/) |
| **Eyad Nader** | [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/eyad-nader-674022309/) |
| **Judy Assem** | [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/judy-assem-5772b4294/) |

---

*"Every pixel is a decision. Make them all count."*

</div>
