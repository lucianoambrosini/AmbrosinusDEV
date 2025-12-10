# Getting Started with Snowflakes Maker

Welcome to Snowflakes Maker! This guide will help you create your first parametric snowflake in minutes.

---

## 📋 Prerequisites

Before starting, ensure you have:
- ✅ Rhino 7 or later installed
- ✅ Grasshopper (included with Rhino)
- ✅ Ambrosinus Toolkit installed

---

## 🚀 Quick Start (5 minutes)

### Step 1: Open Grasshopper
```
In Rhino, type: Grasshopper
or press the Grasshopper icon in the toolbar
```

### Step 2: Add Component
```
1. Navigate to: Ambrosinus > 9.Extra tab
2. Drag "Snowflakes Maker" onto canvas
3. Component appears with default parameters
```

### Step 3: Generate Your First Snowflake
```
1. Leave default values (Thickness: 1.5, Seed: 42)
2. Component automatically generates snowflake
3. Right-click component → Preview to see geometry
```

### Step 4: Explore Variations
```
Press the "❄ Frost Magic" button on component
→ Instant new random design!
→ Press again for another variation
```

---

## 🎨 Basic Parameters

### Thickness (0.5 - 3.0 mm)
Controls the width of snowflake arms:
- **0.5-1.0mm**: Delicate, lace-like patterns
- **1.5-2.0mm**: Balanced, classic look
- **2.5-3.0mm**: Bold, geometric designs

### Seed (Any Integer)
Determines the random variation:
- Same seed = same snowflake every time
- Different seed = new design
- Try: 42, 777, 1337 for interesting results

### Code (Optional)
DNA code to regenerate exact snowflake:
- Leave empty for random generation
- Insert saved code to recreate design
- Code starts with "SFC-"

---

## 📤 Outputs Explained

### Curves
All outline and hole curves combined. Use for:
- Laser cutting (DXF/DWG export)
- CNC routing toolpaths
- Vector graphics

### Surface
Planar surface with holes. Use for:
- 3D printing (extrude in Z)
- Rendering and visualization
- Boolean operations

### DNA Code
Encrypted code representing this exact snowflake:
- Copy and save for later
- Share with others to reproduce design
- Paste in "Code" input to regenerate

### Info
Statistics and generation details:
- Curve count
- Surface count
- Seed used
- DNA code preview

---

## 💡 Tips & Tricks

### Generate Multiple Variations
```
1. Add "Series" component → connect to Seed
2. Set Count to 10
3. Bake all results
4. Choose your favorite!
```

### Perfect Symmetry Check
```
Snowflakes always have N-fold symmetry
Rotate by 360°/N to see pattern repeat
Quality control for manufacturing
```

### Export for Manufacturing
```
For Laser Cutting:
- Select Curves output
- Right-click → Bake
- File → Export Selected → DXF

For 3D Printing:
- Select Surface output
- Use ExtrudeCrv (2-5mm height)
- File → Export Selected → STL
```

### Save DNA Code
```
1. Panel component to DNA Code output
2. Right-click panel → Stream Contents
3. Save to text file
4. Load later to regenerate
```

---

## 🎯 Common Workflows

### Workflow 1: Quick Exploration
```
Goal: Generate 50 variations, pick best one

1. Add Snowflakes Maker
2. Press Frost Magic 50 times
3. Bake favorites as you go
4. Compare and choose winner
```

### Workflow 2: Controlled Series
```
Goal: Create themed collection (same thickness)

1. Set Thickness: 1.5mm (constant)
2. Connect Series to Seed: 1-20
3. Bake all
4. Select top 5 for production
```

### Workflow 3: Reorder Production
```
Goal: Recreate exact design from DNA code

1. Add text panel with saved DNA code
2. Connect to Code input
3. Snowflake regenerates perfectly
4. Export for manufacturing
```

---

## 🐛 Troubleshooting

### "No geometry visible"
- Check Preview is enabled (right-click component)
- Verify Rhino units (mm recommended)
- Zoom to fit: type "Zoom" → "All"

### "Curves look wrong"
- Check Thickness value (0.5-3.0 range)
- Verify Seed is integer
- Try pressing Frost Magic for reset

### "DNA Code doesn't work"
- Ensure code starts with "SFC-"
- Check no extra spaces
- Try copying code again from Info panel

### "Component is slow"
- Expected: 150-200ms generation time
- If slower: check Rhino performance
- Close unnecessary applications

---

## 📚 Next Steps

Now that you've created your first snowflake:
- ✅ Explore different Thickness values
- ✅ Try recommended Seeds (42, 777, 1337)
- ✅ Export for laser cutting or 3D printing
- ✅ Save DNA codes for your favorites
- ✅ Check out example files in `/examples`

### Advanced Topics
- [Manufacturing Guide](manufacturing-guide.md)
- [Batch Generation](batch-generation.md)
- [PRO Version Features](pro-version.md)

---

## 💎 Upgrade to PRO

Want more control? PRO version includes:
- 10+ parameter controls (arms, branches, distributions)
- Batch generation tools
- Database integration
- Commercial license

[Learn more about PRO →](https://ambrosinus.altervista.org)

---

**Happy Snowflake Making! ❄️**

Questions? Visit [ambrosinus.altervista.org](https://ambrosinus.altervista.org)
