# 💠 Project Lucid: The Isometric Urdu Orthography

**Project Lucid** is a structural modernization of the Urdu writing system. It introduces an atomic, monospaced, and non-joining neography designed specifically for the digital age.

By bypassing the computational "shaping" requirements of traditional Nastaliq, Lucid allows for phonetic Urdu typing on any standard QWERTY keyboard with zero additional software installation, utilizing a rigorous **25mm x 25mm isometric grid**.

---

## 👁️ The Vision

Traditional Urdu (Nastaliq) is a masterpiece of calligraphy but a challenge for digital engineering. **Lucid** offers a "Third Way"—preserving the phonetic soul and Right-to-Left (RTL) flow of Urdu while adopting the ergonomic efficiency of monospaced Latin scripts.

* **One Sound, One Glyph:** No initial, medial, or final forms.
* **Monospaced Geometry:** Every character is a perfect square.
* **Searchable Data:** Internally stored as standard phonetic Latin; externally displayed as Lucid glyphs.
* **Zero-Setup:** Works in any RTL-aware environment (Word, Browsers, IDEs) via OpenType substitution.

---

## 🛠️ Technical Specifications

### 1. The 25mm Standard

Every glyph in this repository is designed within a **25mm x 25mm master square**.

* **Units Per Em (UPM):** 1000
* **Advance Width:** 1000 (Strict Monospace)
* **Source Assets:** 37 high-fidelity vector glyphs.

### 2. The Phonetic Engine

Project Lucid utilizes the **OpenType `calt` (Contextual Alternates)** feature to map standard QWERTY input to the 37-glyph inventory.

| Input | Glyph PUA | Phoneme | Logic |
| --- | --- | --- | --- |
| `a` | `U+E014` | ا | Short Vowel |
| `b` | `U+E000` | ب | Labial Plosive |
| `T` | `U+E003` | ٹ | Retroflex |
| `~` | `U+E01C` | ں | Nasalization |

---

## 📂 Repository Structure

```text
├── assets/             # Original 25mm SVG Master Sheet
├── build/              # Compiled .OTF and .TTF files
├── source/             # FontForge (.sfd) project files
├── docs/               # The Lucid Manifesto (Full Documentation)
├── OFL.txt             # SIL Open Font License 1.1
├── README.md           # Project Overview & Documentation
└── CONTRIBUTING.md     # Guidelines for Contributors

```

---

## 🚀 How to Use

1. **Install** the `LucidUrdu.otf` font.
2. **Open** any text editor (MS Word, VS Code, Browser).
3. **Select** the "Lucid Urdu" font.
4. **Enable** Right-to-Left (RTL) paragraph direction.
5. **Type** phonetically (e.g., typing `p a k i s t a n` renders the Lucid isometric symbols).

---

## ⚖️ License

This project is licensed under the **[SIL Open Font License 1.1](OFL.txt)**. You are free to use, study, modify, and redistribute the font, provided you do not sell the font by itself.

Derived from the original 37-glyph research at [font.shehroz.pk](https://font.shehroz.pk/) and the [Shehroz Font Project](https://github.com/xehroz/Shehroz-Font).

---

## 🤝 Contributing

We welcome developers, linguists, and designers to contribute to the **Lucid Manifesto**.

1. Fork the repo.
2. Propose changes to the `calt` mapping or glyph geometry.
3. Submit a Pull Request.

---

**Project Lead:** Shehroz Kaleem

**Documentation:** Still under development. 

**"Simplicity is the ultimate sophistication."** Testing

---
