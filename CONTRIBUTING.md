# Contributing to Project Lucid 💠

First off, thank you for considering contributing to Project Lucid! It is through the collective effort of designers, linguists, and developers that we can modernize Urdu orthography for the digital age.

By contributing, you agree to license your work under the [SIL Open Font License 1.1](LICENSE).

---

## 🏗️ Technical Standards

All contributions must adhere to the **Isometric Square Standard** to maintain the integrity of the monospaced engine.

### 1. Glyph Design (The 25mm Rule)
If you are proposing a new glyph or a stylistic variant:
- **Master Frame:** Every glyph must be designed within a perfect **25mm x 25mm** square.
- **Sidebearings:** Leave a minimum of **2.5mm (10%)** internal padding on the left and right edges to ensure characters do not touch when rendered.
- **Stroke Weight:** Maintain a consistent optical weight across all glyphs to ensure a uniform "texture" in long-form text.
- **Format:** Submit source files as high-fidelity **SVGs** with simplified paths (minimal anchor points).

### 2. Engineering (OpenType & GSUB)
If you are contributing to the font's logic:
- **Codepoints:** New glyphs must be mapped to the **Private Use Area (PUA)** starting at `U+E000`.
- **Feature Code:** All substitutions should be handled within the `calt` (Contextual Alternates) feature to ensure maximum compatibility across modern software.
- **Monospacing:** The **Advance Width** for every glyph must be set to exactly **1000 units** in FontForge.

---

## 🛠️ How to Contribute

### Step 1: Open an Issue
Before making a major change, please open an **Issue** to discuss your proposal. This ensures your work aligns with the project's goals (e.g., maintaining a 37-glyph atomic inventory).

### Step 2: Branching
1. Fork the repository.
2. Create a feature branch: `git checkout -b feature/new-glyph-name`.

### Step 3: Submission
- Ensure your SVG files are named according to their phonetic trigger (e.g., `noon-ghunna.svg` or `U_E01C.svg`).
- Update the `README.md` mapping table if you are introducing a new phonetic trigger.
- Submit a **Pull Request (PR)** with a clear description of the changes.

---

## 🎯 Our Focus Areas
We are specifically looking for help in the following areas:
- **Linguistic Auditing:** Ensuring the 37-glyph set covers all major Urdu dialects.
- **Code Editor Support:** Testing the font in VS Code, Vim, and Sublime Text to ensure RTL monospacing behaves correctly.
- **Documentation:** Expanding the **Lucid Manifesto** for our upcoming pitch to the Unicode Consortium.

---

## 📜 Code of Conduct
We follow a standard of mutual respect. Please be constructive in your feedback and patient with the review process.

**Let's build the future of Urdu, one square at a time.**
