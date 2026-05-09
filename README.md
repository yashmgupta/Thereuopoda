# Cave biodiversity and cryptic diversity in a Southeast Asian centipede (*Thereuopoda* sp.): integrative mitogenomic and phylogenetic evidence for a new species from Thailand

This repository provides the complete mitochondrial genome sequence and reproducible analysis code supporting the description of a new cave-dwelling *Thereuopoda* species (Chilopoda: Scutigeromorpha) from Nam Sai Cave, Phitsanulok Province, Thailand.

---

## Study Overview

Cave-dwelling arthropods in mainland Southeast Asia represent some of the most taxonomically neglected invertebrates in one of the world's most threatened biodiversity hotspots. *Thereuopoda* (Chilopoda: Scutigeromorpha: Scutigeridae) is widely distributed across tropical Asia, yet no molecular data previously existed for any Thai population. We assembled the complete mitochondrial genome of a cave-collected specimen and integrated mitogenomic, phylogenetic, and morphological evidence to formally characterise a new species — the first scutigeromorph centipede described from Thailand using molecular data.

Key findings:
- Complete mitogenome assembled from Illumina paired-end sequencing (14,900 bp; 37 genes)
- Genome is strongly AT-biased (A+T = 66.72%) with conserved scutigeromorph gene order identical to *T. clunifera* and *Scutigera coleoptrata*
- Maximum Likelihood and Bayesian Inference phylogenies (COI + concatenated whole-mitogenome PCGs) consistently place the Thai lineage as sister to *T. chinensis* (ML bootstrap ≥ 97%; BI posterior probability ≥ 0.994)
- Combined molecular and morphological evidence supports recognition as a new species of *Thereuopoda*
- Extends documented cryptic diversity in Thereuoneminae beyond China into the Indochinese Peninsula
- Provides the first molecular reference for any Thai scutigeromorph, establishing a baseline for barcoding and biodiversity monitoring

---

## Repository Contents

| File | Description |
|---|---|
| `sequence.gb` | Annotated complete mitochondrial genome in GenBank format |
| `Thereuopoda_Mitogenome_Final_Analysis_v2.ipynb` | Jupyter Notebook with the full mitogenomic analysis pipeline |

---

## Genome Summary

| Feature | Value |
|---|---|
| Organism | *Thereuopoda* sp. nov. (Scutigeromorpha: Scutigeridae) |
| Collection locality | Nam Sai Cave, Phitsanulok Province, Thailand |
| Genome size | 14,900 bp |
| Topology | Circular |
| A+T content | 66.72% |
| Genetic code | Invertebrate mitochondrial (NCBI Table 5) |
| Protein-coding genes | 13 |
| tRNA genes | 22 |
| rRNA genes | 2 |
| Control region | 1 |
| GC skew | −0.3444 |
| AT skew | −0.0849 |
| Gene order | Conserved; identical to *T. clunifera* and *S. coleoptrata* |

**Protein-coding genes:** *nad2, cox1, cox2, atp8, atp6, cox3, nad5, nad4L, nad6, nad1, nad3, nad4, cob*

---

## Analysis Pipeline

The notebook (`Thereuopoda_Mitogenome_Final_Analysis_v2.ipynb`) covers:

1. **Genome parsing** — GenBank file parsed with [Biopython](https://biopython.org/)
2. **Nucleotide composition** — Per-gene and whole-genome A/T/G/C content, GC skew, AT skew
3. **RSCU calculation** — Relative Synonymous Codon Usage under Invertebrate Mitochondrial Code (Table 5) for all 13 PCGs
4. **Amino acid composition** — Frequency analysis across all protein-coding genes
5. **Gene organization** — Feature counts, lengths, and strand distribution
6. **Figure generation** — Publication-quality figures (RSCU bar charts, codon usage heatmap, circular genome map, GC/AT skew plots)

### Dependencies

```
biopython
matplotlib
pandas
numpy
```

Install with:

```bash
pip install biopython matplotlib pandas numpy
```

---

## Usage

Clone the repository and open the notebook:

```bash
git clone https://github.com/yashmgupta/Thereuopoda.git
cd <your-repo>
jupyter notebook Thereuopoda_Mitogenome_Final_Analysis_v2.ipynb
```

The notebook reads `sequence.gb` from the same directory. No other external files are required.

---

## Data Availability

The annotated mitochondrial genome sequence (`sequence.gb`) is provided in this repository and can be cited directly for data availability statements. This repository serves as the primary data and methods reference for the associated publication.

---

## Citation

---

## License

Made available for academic and research use. MIT
