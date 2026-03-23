# PerovSearch

> A natural-language query and interpretation framework for cubic perovskite databases

[![React](https://img.shields.io/badge/React-18-61DAFB?logo=react)](https://reactjs.org/)
[![Anthropic](https://img.shields.io/badge/AI-Claude%20Sonnet%204-orange)](https://anthropic.com)

The app opens at `(https://perov-search.vercel.app/)`.
---

## Overview

PerovSearch lets researchers describe their ideal perovskite in plain English and translates it into structured screening queries over **18,928 ABX₃ cubic perovskites** from the Computational Materials Repository (CMR).

> Associated paper: *PerovSearch: A natural-language query and interpretation framework for cubic perovskite databases*, submitted to Computational Materials Science.

---

## Features

- Natural language search (e.g. *"Lead-free stable oxide for water splitting"*)
- Rule-based constraint extraction — band gap, stability, element exclusion, anion type
- Multi-criteria candidate ranking
- AI-assisted explanation via Claude Sonnet 4
- Band alignment diagram vs. NHE for top candidates
- Manual numeric filter mode

---

## Database

| Property | Value |
|---|---|
| Total compounds | 18,928 |
| Elements | 52 |
| Anion systems | 7 (O₃, O₂N, O₂F, O₂S, ON₂, OFN, N₃) |
| Water-splitting candidates | 24 |

Source: CMR cubic perovskite dataset. Properties computed with the GLLB-SC functional.

---

## Getting Started

### Prerequisites

- Node.js ≥ 18

### Install and run

```bash
git clone https://github.com/YOUR_USERNAME/PerovSearch.git
cd PerovSearch
npm install
npm start
```

### Anthropic API key

The app calls Claude to generate expert analysis. Create a `.env` file in the project root:

```
REACT_APP_ANTHROPIC_KEY=sk-ant-...
```

> **Never commit your `.env` file.** It is already listed in `.gitignore`.

---

## Repository Structure

```
PerovSearch/
├── public/
│   └── index.html
├── src/
│   ├── index.jsx          # React entry point
│   └── PerovSearch.jsx    # Main app (database embedded)
├── .gitignore
├── package.json
└── README.md
```

---

## Citation

```
PerovSearch: A natural-language query and interpretation framework
for cubic perovskite databases. Computational Materials Science.
```

---

## Acknowledgements

- Database: Computational Materials Repository (CMR)
- AI explanation: [Anthropic Claude](https://anthropic.com)
- Electronic structure: GLLB-SC functional
