# Reversal — Signature-Based Drug Repurposing Demo

An interactive prototype demonstrating **computational drug repurposing**: instead of designing a new molecule from scratch, the app profiles a disease's gene-expression "signature," searches it against known diseases and their approved treatments, and ranks existing drugs by how strongly they *reverse* that signature.

This mirrors real methodology used in bioinformatics (Connectivity Map / LINCS L1000-style signature matching), the same logic behind real-world COVID-19 repurposing findings for drugs like dexamethasone and baricitinib.

## How it works

1. **Profile** — pick a disease scenario, or manually set a 12-gene expression signature
2. **Vectorize** — the signature becomes a numeric vector
3. **Match** — cosine similarity finds the closest known reference disease
4. **Validate** — approved drugs for that disease are ranked by reversal score (how strongly their known effect runs opposite the disease signature)

## Running it

This is a single self-contained `index.html` file — no build step, no dependencies. Open it in any browser, or deploy it as-is via GitHub Pages.

## ⚠️ Important

This is a research/educational prototype using a small **illustrative** dataset (not live clinical data). It is **not connected to real clinical databases**, and its output is **not medical advice**. Real drug repurposing candidates require laboratory and clinical validation before any use in patients.

## Stack

Plain HTML, CSS, and vanilla JavaScript. No frameworks, no build tools.
