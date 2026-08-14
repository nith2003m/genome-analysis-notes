# Assembly Quality Control
Genome assembly quality should be evaluated before downstream
taxonomic and functional analysis.

## Key Metrics

| Metric | Purpose |
|---|---|
| Genome size | Estimates total assembled sequence |
| Contig count | Indicates assembly fragmentation |
| N50 | Measures assembly continuity |
| GC content | Helps identify unusual sequence composition |
| BUSCO completeness | Evaluates conserved gene recovery |
| CheckM2 completeness | Estimates genome completeness |
| CheckM2 contamination | Estimates possible contamination |

## Recommended Tools

- QUAST — assembly statistics
- BUSCO — conserved gene completeness
- CheckM2 — genome completeness and contamination

## Basic Workflow

```text
Assembly
   ↓
QUAST
   ↓
BUSCO
   ↓
CheckM2
   ↓
Review genome quality
   ↓
Downstream analysis
