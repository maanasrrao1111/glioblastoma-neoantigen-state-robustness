# Cellular-State Escape Risk Among Clinically Prioritized Neoantigens in IDH-Wild-Type Glioblastoma

## Summary

Neoantigen vaccine design typically prioritizes MHC binding affinity and clonal prevalence but overlooks whether targeted antigens are expressed in transcriptionally stable or plastic tumor cell states. This project introduces the **State Robustness Index (SRI)** — a metric quantifying how consistently a neoantigen's source gene is expressed across GBM cellular states — and applies it to clinically selected vaccine candidates from three trials.

## Key datasets

- **Primary atlas:** Neftel et al. scRNA-seq (GSE131928) — IDH-wt GBM cellular states
- **Validation atlas:** Wang et al. scRNA-seq (GSE182109) — recurrent and newly diagnosed GBM
- **Clinical trials:** GNOS-PV01 (Johanns et al., *Nature Cancer* 2026), NeoVax (Keskin et al., *Nature* 2019), ZSNeo-DC (Zhang et al., *Nature Communications* 2026)

## Results

All result tables are in `results/`. Key files:

| File | Description |
|------|-------------|
| `state_robustness_index_full.csv` | SRI scores for 403 genes (Neftel atlas) |
| `wang_state_robustness_index.csv` | SRI scores computed on the Wang validation atlas |
| `sri_concordance.csv` | Cross-atlas SRI concordance |
| `gnos_pv01_final_candidates.csv` | GNOS-PV01 vaccine targets with SRI annotations |
| `immunogenicity_sri_merged.csv` | SRI vs immunogenicity analysis |
| `neovax_sri_results_full.csv` | NeoVax trial SRI analysis |
| `zsneo_sri_results_full.csv` | ZSNeo-DC trial SRI analysis |
| `ranking_comparison.csv` | How SRI re-ranks vaccine candidates vs standard prioritization |

## Data access

Raw scRNA-seq data (too large for GitHub) can be downloaded from GEO:
- Neftel et al.: [GSE131928](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE131928)
- Wang et al.: [GSE182109](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE182109)

## Note on analysis scripts

Analyses were conducted interactively on JHU Rockfish HPC. Standalone reproducible scripts are being reconstructed and will be added.

## Author

Maanas Rao — MS Biotechnology, Johns Hopkins University
