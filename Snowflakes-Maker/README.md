# ❄️ Snowflakes Maker

**Parametric snowflake generator for Grasshopper**

Create mathematically unique, manufacturing-ready snowflake designs with infinite variations. Perfect for laser cutting, 3D printing, and computational design projects.

[![License](https://img.shields.io/badge/License-All%20Rights%20Reserved-red.svg)](LICENSE)
[![Grasshopper](https://img.shields.io/badge/Grasshopper-Compatible-brightgreen.svg)](https://www.grasshopper3d.com/)
[![Rhino](https://img.shields.io/badge/Rhino-7%2B-blue.svg)](https://www.rhino3d.com/)

---

## 🌟 Features

- **Random Generation Mode** - Generate infinite unique snowflake designs
- **Mathematically Accurate** - Based on real snowflake formation principles
- **N-fold Symmetry** - Perfect radial symmetry patterns
- **Manufacturing Ready** - Outputs optimized for laser cutting and 3D printing
- **Parametric Control** - Fine-tune thickness and randomization
- **One-of-a-Kind Designs** - 1.25 quintillion possible combinations

---

## 📦 What's Included

### Free Version
- Random snowflake generation
- Thickness control (0.5-3.0mm)
- Seed-based randomization
- Manufacturing-ready curves
- Planar surface output
- DNA code generation for reproduction

### Professional Version
- Full parametric control (10+ parameters)
- Batch generation tools
- Database integration
- Branded code system for reordering
- Commercial license
- Priority support

[Contact for PRO version →](https://ambrosinus.altervista.org)

---

## 🚀 Installation

### Requirements
- Rhino 7 or later
- Grasshopper (included with Rhino)

### Installation Steps

1. **Download** the latest release from [Food4Rhino](https://www.food4rhino.com/) or [GitHub Releases](../../releases)

2. **Install** the `.gha` file:
   ```
   Windows: %AppData%\Grasshopper\Libraries\
   Mac: ~/Library/Application Support/McNeel/Rhinoceros/X.0/Plug-ins/Grasshopper/Libraries/
   ```

3. **Restart** Rhino and Grasshopper

4. Find components in **Ambrosinus > 9.Extra** tab

---

## 📚 Usage

### Basic Workflow

```
1. Add "Snowflakes Maker" component to canvas
2. Adjust Thickness parameter (0.5-3.0mm)
3. Change Seed for different variations
4. Press "❄ Frost Magic" button for instant random designs
5. Export curves for manufacturing
```

### Inputs

| Parameter | Type | Range | Description |
|-----------|------|-------|-------------|
| **Code** | Text | Optional | DNA code to regenerate exact snowflake |
| **Thickness** | Number | 0.5-3.0 | Line thickness / offset distance (mm) |
| **Seed** | Integer | Any | Random seed for variation control |

### Outputs

| Output | Type | Description |
|--------|------|-------------|
| **Curves** | Curves | All curves (outline + holes) - ready for manufacturing |
| **Surface** | Brep | Planar surfaces with holes |
| **DNA Code** | Text | Unique code to regenerate this exact snowflake |
| **Info** | Text | Generation information and statistics |

---

## 🎨 Examples

### Example 1: Basic Random Generation
```
Thickness: 1.5mm
Seed: 42
Result: 6-armed snowflake with organic branching
```

### Example 2: Thick Crystal Design
```
Thickness: 2.5mm
Seed: 1337
Result: Bold, geometric snowflake pattern
```

### Example 3: Delicate Lace Pattern
```
Thickness: 0.8mm
Seed: 777
Result: Fine, intricate snowflake design
```

See `/examples` folder for sample Grasshopper definitions.

---

## 🛠️ Manufacturing

### Laser Cutting
- Export curves as DXF/DWG
- All outlines and holes included
- Recommended materials: Acrylic, wood, cardboard
- Typical size: 50-100mm diameter

### 3D Printing
- Use Surface output for extrusion
- Extrude 2-5mm for ornaments
- Recommended: PLA, PETG
- Add mounting hole if needed

### CNC Routing
- Export curves as toolpaths
- Set appropriate depth per material
- Consider adding tabs for fragile areas

---

## 📖 Documentation

- **Getting Started Guide** - [docs/getting-started.md](docs/getting-started.md)
- **API Reference** - [docs/api-reference.md](docs/api-reference.md)
- **FAQ** - [docs/faq.md](docs/faq.md)
- **Troubleshooting** - [docs/troubleshooting.md](docs/troubleshooting.md)

Full documentation available at: [ambrosinus.altervista.org](https://ambrosinus.altervista.org/blog/ambrosinus-toolkit/)

---

## 🎯 Use Cases

- **Jewelry Design** - Unique snowflake pendants and earrings
- **Holiday Decorations** - Laser-cut ornaments and window decals
- **Architectural Models** - Parametric facade patterns
- **Gift Tags** - Personalized holiday gift decorations
- **Educational** - Teaching computational design and geometry
- **Art Installations** - Large-scale parametric artworks

---

## 🔧 Technical Details

### Algorithm
- Based on dendritic crystal growth patterns
- Implements N-fold radial symmetry
- Parametric branch distribution systems
- Clipper2 library for offset operations
- Collision-free geometry generation

### Performance
- Typical generation time: 150-200ms
- Optimized for Paths64 integer operations
- Smart curve sampling and preprocessing
- Handles complex geometries efficiently

### File Formats
- Native: Grasshopper definition (.gh)
- Export: DXF, DWG, STL, 3DM, PDF
- DNA Code: Encrypted text string

---

## 🤝 Contributing

This is a commercial project with a free tier. Contributions are welcome for:
- Bug reports and fixes
- Documentation improvements
- Example definitions
- Use case showcases

Please open an issue first to discuss proposed changes.

---

## 📧 Support

- **Website**: [ambrosinus.altervista.org](https://ambrosinus.altervista.org)
- **Shop**: [etsy.com/shop/TheArchitectLAB](https://www.etsy.com/shop/TheArchitectLAB)
- **Email**: Contact via website
- **Social**: [@AmbrosinusDEV](https://twitter.com/AmbrosinusDEV)

For PRO version inquiries and commercial licensing, please contact through the website.

---

## 📜 License

**© 2024 Luciano Ambrosini - All Rights Reserved**

### Free Version
- ✅ Personal use
- ✅ Educational use
- ✅ Non-commercial projects
- ❌ Commercial use (requires PRO license)
- ❌ Redistribution
- ❌ Modification of source code

### Professional Version
- ✅ All Free features
- ✅ Commercial use
- ✅ Extended support
- ✅ Source code access (upon request)

See [LICENSE](LICENSE) for full terms.

---

## 🏆 Credits

**Created by**: Luciano Ambrosini  
**Website**: [lucianoambrosini.it](https://lucianoambrosini.it)  
**Part of**: [Ambrosinus Toolkit](https://ambrosinus.altervista.org/blog/ambrosinus-toolkit/)

### Built With
- [Rhinoceros 3D](https://www.rhino3d.com/)
- [Grasshopper](https://www.grasshopper3d.com/)
- [Clipper2](https://github.com/AngusJohnson/Clipper2) - Polygon clipping library
- [RhinoCommon SDK](https://developer.rhino3d.com/)

---

## 🎄 Acknowledgments

Special thanks to:
- The Grasshopper community for inspiration
- McNeel & Associates for Rhino/Grasshopper
- All users and supporters of Ambrosinus Toolkit

---

## 📊 Project Status

**Current Version**: 3.0.0 FREE  
**Last Updated**: December 2025  
**Status**: Active Development  

### Roadmap
- [ ] Additional export formats
- [ ] Advanced symmetry patterns
- [ ] Material presets library
- [ ] Cloud rendering service
- [ ] Mobile app companion

---

## ⭐ Star This Repository

If you find this tool useful, please consider starring this repository to show your support!

---

**Made with ❄️ by [Ambrosinus](https://ambrosinus.altervista.org)**
