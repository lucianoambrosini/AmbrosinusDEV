# 📂 GitHub Repository Structure

## Complete folder structure for snowflakes-maker repository

```
snowflakes-maker/
│
├── .github/                          # GitHub specific files
│   ├── workflows/                    # CI/CD (optional)
│   └── ISSUE_TEMPLATE/               # Issue templates (optional)
│
├── .system/                          # 🔐 SYSTEM FILES (stealth mode)
│   ├── registry.dat                  # ← SPECIAL CODES DATABASE (encrypted)
│   └── manifest.json                 # ← Dummy file (distraction)
│
├── docs/                             # Documentation
│   ├── getting-started.md            # Quick start guide
│   ├── api-reference.md              # (future) API docs
│   ├── faq.md                        # (future) FAQ
│   └── troubleshooting.md            # (future) Common issues
│
├── examples/                         # Example Grasshopper files
│   ├── README.md                     # Examples index
│   ├── basic-snowflake.gh            # (future) Basic example
│   ├── multiple-variations.gh        # (future) Batch example
│   └── laser-cutting-export.gh       # (future) Export example
│
├── assets/                           # Images and media
│   ├── logo.png                      # (future) Project logo
│   ├── icon.png                      # (future) Component icon
│   ├── preview.jpg                   # (future) Preview image
│   └── screenshots/                  # (future) Screenshots
│
├── releases/                         # (optional) Binary releases
│   └── README.md                     # Release notes
│
├── .gitignore                        # Git ignore file
├── LICENSE                           # License file
└── README.md                         # Main documentation

```

---

## 🔐 CRITICAL FILES

### `.system/registry.dat`
**Purpose**: Encrypted special codes database  
**Security**: SHA256 hash + AES encryption  
**Format**: `HASH|ENCRYPTED_MESSAGE`  
**Updates**: Weekly (via Git commit)  
**Visibility**: Public but useless without SECRET_KEY

### `.system/manifest.json`
**Purpose**: Dummy file for distraction  
**Content**: Generic system metadata  
**Effect**: Makes `.system/` look like normal config folder

---

## 📝 INITIAL SETUP STEPS

### 1. Create Repository
```bash
# On GitHub.com
New Repository → snowflakes-maker
Description: "Parametric snowflake generator for Grasshopper"
Public repository
Initialize with README: NO (you'll add custom one)
```

### 2. Clone Locally
```bash
git clone https://github.com/AmbrosinusDEV/snowflakes-maker.git
cd snowflakes-maker
```

### 3. Add Files
```bash
# Copy all files from this package to repo folder
# Maintain folder structure exactly as shown above
```

### 4. Create Folders
```bash
mkdir -p .system docs examples assets releases
```

### 5. Initial Commit
```bash
git add .
git commit -m "Initial commit: Snowflakes Maker v3.0.0"
git push origin main
```

---

## 🔄 UPDATE WORKFLOW

### Adding New Special Code

1. **Generate GitHub Line** (using helper tool)
   ```
   TC: SFC-xyz...
   Message: "🏆 Special Message"
   → Output: hash|encrypted
   ```

2. **Update registry.dat**
   ```bash
   cd .system
   nano registry.dat
   # Add new line at end
   # Save and exit
   ```

3. **Commit & Push**
   ```bash
   git add .system/registry.dat
   git commit -m "Add December Code Hunt #3"
   git push origin main
   ```

4. **Verify URL**
   ```
   https://raw.githubusercontent.com/AmbrosinusDEV/
   snowflakes-maker/main/.system/registry.dat
   
   Should show updated file immediately
   ```

5. **Share Code**
   ```
   Post TC on social media
   Users insert → Easter egg appears!
   ```

---

## 📊 GITHUB PAGES (Optional)

Enable GitHub Pages for documentation hosting:

```bash
# Settings → Pages
Source: Deploy from branch
Branch: main
Folder: /docs
```

Then docs will be available at:
```
https://ambrosinusdev.github.io/snowflakes-maker/
```

---

## 🎯 RECOMMENDED BADGES

Add to README.md:

```markdown
[![License](https://img.shields.io/badge/License-All%20Rights%20Reserved-red.svg)](LICENSE)
[![Grasshopper](https://img.shields.io/badge/Grasshopper-Compatible-brightgreen.svg)](https://www.grasshopper3d.com/)
[![Rhino](https://img.shields.io/badge/Rhino-7%2B-blue.svg)](https://www.rhino3d.com/)
[![Version](https://img.shields.io/badge/Version-3.0.0-blue.svg)](https://github.com/AmbrosinusDEV/snowflakes-maker/releases)
[![Downloads](https://img.shields.io/github/downloads/AmbrosinusDEV/snowflakes-maker/total.svg)](https://github.com/AmbrosinusDEV/snowflakes-maker/releases)
```

---

## 🔒 SECURITY NOTES

### Public Files (Safe)
- ✅ README.md - General info
- ✅ LICENSE - Terms
- ✅ docs/ - Documentation
- ✅ examples/ - Sample files
- ✅ .system/registry.dat - Encrypted data

### Private Files (NEVER commit)
- ❌ Source code (.cs files)
- ❌ SECRET_KEY
- ❌ Build artifacts (.dll, .gha)
- ❌ Personal notes
- ❌ Database credentials

### .gitignore Protection
Already configured to exclude:
- Build folders
- Binary files
- IDE settings
- Sensitive data

---

## 📈 GROWTH STRATEGY

### Phase 1: Launch (Week 1)
```
- Upload all base files
- Add initial registry.dat (10 codes)
- Create release v3.0.0
- Announce on social media
```

### Phase 2: Content (Month 1)
```
- Add example .gh files
- Create video tutorials
- Add screenshots to assets/
- Write FAQ and troubleshooting docs
```

### Phase 3: Engagement (Month 2+)
```
- Weekly registry.dat updates
- Monthly code hunts
- Community showcase
- Issue/PR management
```

---

## 🎨 ASSETS TO ADD LATER

### Priority 1 (Launch)
- [ ] Component icon (24x24 PNG)
- [ ] Preview image (1200x630 for social)
- [ ] Basic example .gh file

### Priority 2 (Month 1)
- [ ] Logo design
- [ ] Screenshots collection
- [ ] Video tutorial
- [ ] GIF animations

### Priority 3 (Month 2+)
- [ ] Advanced examples
- [ ] Template library
- [ ] Preset collection
- [ ] Style guide

---

## 📞 MAINTENANCE

### Weekly Tasks
- Check for issues/questions
- Update registry.dat (new codes)
- Monitor social media mentions
- Respond to comments

### Monthly Tasks
- Review analytics
- Update documentation
- Add new examples
- Plan next code hunt

### Quarterly Tasks
- Major version updates
- Feature additions
- Marketing campaigns
- Community contests

---

**Repository ready to launch! 🚀**

Follow this structure for professional, organized GitHub presence.
