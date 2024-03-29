A pipeline to gather snoRNA and RBP interactions to perform a sno-RBP interaction network analysis.

**Dependencies:**
- snakemake

**Author:** Kristina Sungeun Song kristina.song@usherbrooke.ca

**Inputs:**
- RBP data downloaded from ENCODE
    - Target category: select 'RNA binding protein'
- snoGloBe predictions against all protein coding biotypes
- snoDB: all snoRNAs that have protein coding host genes
- HTRRI
- list of snoRNAs (Ensembl_id, name, type)
- list of RBPs (protein_id, name, type)

**Types of snoRNA-RBP Interactions:**
- Overlap of target sites:
    - snoRNA-RBP
- Direct binding interactions:
    - RBP binds to snoRNA transcript
- Interactions from external database:
    - STRING RBP-RBP binding interactions
    - High-throughput RNA-RNA interactions: PARIS, SPLASH, LIGR-seq

**Requirements 2023**
- Obtain snoGloBe predictions https://github.com/scottgroup/snoGloBe/tree/master