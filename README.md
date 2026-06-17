# H3N2 Hemagglutinin Evolution (2020–2024)

A Colab notebook tracking seasonal antigenic drift in influenza A H3N2 via
pairwise nucleotide identity analysis of hemagglutinin (segment 4) sequences
pulled live from NCBI GenBank.

## What it does
- Queries NCBI for human H3N2 HA sequences across five flu seasons
- Filters to full-length sequences (~1,700 bp), balanced across years
- Computes an n×n pairwise identity matrix
- Visualises evolutionary clustering (heatmap + UPGMA dendrogram)
- Estimates divergence rate and benchmarks it against the ~1–2%/year
  published for H3N2 HA

## Run it
Open in Google Colab — all dependencies install in the first cell.
NCBI queries are rate-limited; the full run takes ~2–3 minutes.

## Background
H3N2 undergoes the fastest antigenic drift of any seasonal strain,
driving annual vaccine reformulation more than any other subtype.
This notebook provides a reproducible, code-first look at that drift.

## Next steps
- Translate HA → amino acids, analyse antigenic sites (HA1 145, 155–159, 189, 193)
- Run MAFFT alignment before identity calculation
- Build a maximum-likelihood phylogeny with IQ-TREE
- Compare circulating strains vs WHO vaccine recommendations

---
*Data: NCBI GenBank. Reference: Krammer et al., Nature 2018.*
*Author: [@gravityeffect1](https://github.com/gravityeffect1)*
