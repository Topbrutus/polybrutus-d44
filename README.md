# Polybrutus 44D — Exact 49-point Euclidean metric and a 38-fold ideal graph mode

**Responsible human scientific author:** Gabriel St-Pierre, independent researcher.  
**Material AI assistance:** OpenAI ChatGPT (Astra) materially assisted exact rational calculations, two separately implemented verification programs, scientific manuscript and controlled publication. AI is not a scientific author.

## Exact Euclidean geometry at R=1

- **49 norm-one labelled points**, **1,176 unordered labelled squared distances**, exact minimum affine Euclidean realization dimension **44**.
- **1,128/1,128** parent squared pair distances with their original labels preserved from [frozen Polybrutus D43 v0.1.0](https://github.com/Topbrutus/polybrutus-d43/tree/v0.1.0), scientific commit `e435e38aed88e8c65d294eeee26bee6b89056fc8`, DOI [10.5281/zenodo.24415111](https://doi.org/10.5281/zenodo.24415111).
- One appended perpendicular norm-one vertex contributes **48** new squared distances, each **2R²**.
- Normalized exact histogram `k=4d²/R²`: `{4:6,7:2,8:1145,9:3,10:10,12:6,13:2,16:2}`. Exact sum of all pair squared distances at R=1: **9455/4**.
- The exact rational centered Euclidean Gram is positive semidefinite of rank **44**.
- A **separately stipulated ideal weighted complete graph** with unit scalar masses and weights `w_ij=R²/d_ij²` has weighted graph Laplacian eigenvalue **49/2** of multiplicity **38**, and **24** of multiplicity **4**. These are dimensionless chosen-model eigenvalues and **not measured frequencies**.
- Two separately implemented exact-rational checkers validate all 1,176 labelled pairs, all 1,128 predecessor labels, exact Euclidean ranks and selected graph eigenspaces. Four main adversarial controls pass.

## Exact reproducibility

```bash
python -m pip install sympy==1.14.0
python src/verify_d44.py
python tests/independent_d44.py
```

Both programs output the same deterministic SHA-256 for `results/certificate_d44.json`.

**Immutable complete scientific lineage:** The exact frozen D43 scientific tag including *all* ancestors is in `prior/d43/frozen_scientific_tag_v0.1.0.zip` (SHA-256 `a009bf83bbca8f3b343c29afb470f647a8dd8fdbde176051c8f3d1ad34b512e1`, 28 entries, CRC PASS). Original certificate `results/certificate_d43.json` is extracted byte-identically to `prior/d43/results/certificate_d43.json`; both programs check the ZIP, certificate, hashes and CRC. Compressed ancestral source avoids Windows MAX_PATH issues while preserving all original bytes, without Git submodules or nested repositories.

## Sources and limitations

- [Exact specification](SPECIFICATION_D44.md); [constructive proof and falsification controls](PREUVE_D44.md); [provenance and scientific boundaries](PROVENANCE.md); [parent source archive](prior/d43/ARCHIVE_PROVENANCE.md).
- [Scientific preprint PDF](publication/POLYBRUTUS_44D_NOTE.pdf); [editable scientific preprint](publication/POLYBRUTUS_44D_NOTE.md); [complete 1,176-pair certificate](results/certificate_d44.json).

These exact mathematical properties describe one *synthetic* Euclidean metric and one stipulated ideal weighted graph via established perpendicular extensions and uniform graph joins. This does **not** establish additional physical spacetime dimensions, measured resonances, particle discoveries, a new universal theorem, or independent human peer review.

**Licenses:** software MIT; scientific manuscript CC BY 4.0.
