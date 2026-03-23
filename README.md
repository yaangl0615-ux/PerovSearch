# PerovSearch

A computational framework for natural-language interrogation and screening of perovskite materials databases.

## Overview

PerovSearch is a lightweight workflow for translating natural-language materials queries into structured screening constraints, retrieving candidate perovskites from a database, ranking the results, and generating concise explanations for the returned candidates.

This repository accompanies the manuscript:

**PerovSearch: A Computational Framework for Natural-Language Interrogation and Screening of Perovskite Materials Databases**

## Repository contents

```text
.
├── src/
│   ├── parser.py
│   ├── retrieval.py
│   ├── ranking.py
│   ├── explanation.py
│   └── evaluate.py
├── data/
│   ├── sample_perovskites.csv
│   └── sample_queries.json
├── examples/
│   ├── demo_input.txt
│   └── demo_output.json
├── requirements.txt
├── LICENSE
└── README.md
