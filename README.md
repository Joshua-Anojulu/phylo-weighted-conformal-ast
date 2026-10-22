# Phylogeny-weighted conformal prediction for genomic antibiotic susceptibility testing: four failures of a natural idea

Code and result tables for the paper by Joshua Anojulu and Varun Puttagunta, presented at the workshop I Can't Believe
It's Not Better (ICBINB): Failure Modes of AI in Biology, NeurIPS 2026.

## What is here

- `icbinb51_release.zip`: the release bundle (2,337,326 bytes, 85 files), sha256
  `0a72bea93c59a16b103ad3fd4cf58240d3f8dd3a82881ec288a95cb4dbec6d66`.
  Unzip it to get `icbinb51_release/`; its `README.md` explains every folder, how to rebuild the paper's numbers and
  figures from the result tables, and how to rebuild the result tables from the public data.
- `LICENSE`: the MIT license, which covers the code.

To check a download:

    sha256sum icbinb51_release.zip      # on macOS: shasum -a 256 icbinb51_release.zip
    unzip icbinb51_release.zip
    cd icbinb51_release && sha256sum -c MANIFEST.sha256

## Data

All data come from the CRyPTIC consortium's public June 2022 release, which needs no credentials:
https://ftp.ebi.ac.uk/pub/databases/cryptic/release_june2022/ . Please cite The CRyPTIC Consortium (2022), PLOS Biology
20(8): e3001721 and e3001755. The tables in the bundle are derived from that release and stay under its terms. The
cophenetic distance matrix is too large to host; a script in the bundle rebuilds it from the public tree, and the
bundle records its checksum.
