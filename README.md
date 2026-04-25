# corroshield-predictor
CorroShield – an interactive web tool that predicts corrosion inhibition efficiency of any molecule or element on various metals, using a local cheminformatics engine. No API keys required – runs entirely in your browser.
# 🧪 CorroShield – Corrosion Inhibitor Predictor

**Predict corrosion inhibition efficiency of any molecule, element, or SMILES string – directly in your browser.**

CorroShield is a cheminformatics web application that analyzes molecular structures (heteroatoms, aromatic rings, LogP, etc.) and estimates how well a compound protects metals like iron, steel, copper, aluminum, zinc, or nickel in different corrosive environments (acidic, saline, alkaline, neutral, industrial). No server, no API keys – all calculations are local and instant.

![Screenshot](screenshot.png) <!-- optional: add a screenshot later -->

## 🔬 Features

- **Instant predictions** – type any molecule (e.g., *Benzotriazole*, *Quinoline*, *NaCl*, *Fe*) and get efficiency score (0–100%)
- **Metal & environment selection** – choose from 6 metals and 5 corrosive media
- **Rich molecular descriptors** – shows heteroatom count, aromatic rings, LogP, molecular weight, and adsorption affinity
- **AI‑style analysis** – detailed verdict, mechanism explanation, and improvement suggestions
- **Gauge & bar visualisations** – intuitive feedback on inhibition performance
- **Preset examples** – quickly test known inhibitors and poor performers
- **Fully local** – no external API calls, works offline after first load

## 🚀 Live Demo

👉 [corroshield-predictor](https://YOUR_USERNAME.github.io/REPO_NAME/)  
*(replace with your actual GitHub Pages link)*

## 🛠️ How it works

The tool extracts chemical features from the input name (e.g., identifies nitrogen/sulfur atoms, aromatic rings, molecular weight) and applies a rule‑based scoring algorithm that mimics expert knowledge:

- Heteroatoms (N,S,O) → strong metal binding
- Aromatic rings → π‑stacking adsorption
- Metal compatibility modifiers (e.g., triazoles on copper)
- Environmental adjustments (e.g., basic N atoms in acidic media)

The result is a scientifically plausible inhibition efficiency, plus actionable suggestions to improve performance.

## 📋 Usage

1. Enter a molecule name, element symbol, or SMILES string (e.g., `Benzotriazole`, `Fe`, `c1ccccc1`).
2. Select the **metal surface** and **environment**.
3. Click **⚡ ANALYZE INHIBITION**.
4. View the inhibition score, molecular properties, and detailed analysis.

> **Examples to try:**
> - `Benzotriazole` + Copper + Saline → Excellent inhibitor (90%+)
> - `Benzene` + Iron + Acidic → Poor inhibitor (<20%)
> - `Imidazole` + Steel + Acidic → Good inhibitor

## 📁 Project structure

Only one file – `index.html` – contains all HTML, CSS, and JavaScript. No build steps, no dependencies (except Google Fonts). Perfect for quick deployment or embedding.

## 🌐 Deployment on GitHub Pages

1. Fork or clone this repository.
2. Ensure the main file is named `index.html`.
3. Go to **Settings → Pages**.
4. Set branch to `main` and folder to `/ (root)`.
5. Your site will be live at `https://<username>.github.io/<repository>/`.

## 📜 License

MIT – free to use, modify, and distribute.

## 🤝 Contributing

Ideas to improve the scoring algorithm? Open an issue or pull request. New environment types, metal surfaces, or molecular descriptors are welcome.

## ⚠️ Disclaimer

This tool is for **educational and demonstration purposes** only. Real corrosion inhibition depends on many additional factors (concentration, temperature, surface preparation, etc.). Always validate with experimental data for critical applications.

---

**Built with ❤️ using HTML/CSS/JS – no backend needed.**
