# Polybrutus 44D: Exact 49-point Euclidean distance geometry and a thirty-eightfold ideal graph mode

**Gabriel St-Pierre** — Independent researcher  
**21 November 2026**  
**Exact mathematical case study / scientific preprint**  
**Material AI assistance:** OpenAI ChatGPT (Astra) assisted exact rational mathematics, two separately implemented checkers, scientific writing and controlled publication. AI is not a scientific author.

## Abstract

We construct one exact Euclidean labelled squared-distance metric on 49 norm-one points by conservatively adjoining one perpendicular unit vertex to frozen Polybrutus 43D. All 1,128 predecessor labelled squared distances remain unchanged and 48 new squared distances of value 2 arise at unit radius, giving 1,176 unordered labelled pairs. The exact rational centered Euclidean Gram matrix is positive semidefinite with rank 44, demonstrating minimum affine Euclidean realization dimension 44 for this specific metric. For a separately stipulated complete ideal unit-mass weighted graph with weights w_ij=1/d_ij², the weighted Laplacian has eigenvalue 49/2 of multiplicity 38, and eigenvalue 24 of multiplicity 4. Two distinct exact-rational checking programs verify each labelled pair, full predecessor conservation, Euclidean rank and graph nullities. None of these mathematical calculations establishes physical extra spacetime dimensions or experimentally measured resonances.

## 1. Frozen source parent and complete protected lineage

The immutable scientific parent is Topbrutus/polybrutus-d43 at v0.1.0, scientific commit e435e38aed88e8c65d294eeee26bee6b89056fc8, DOI 10.5281/zenodo.24415111. Its original certificate covers 48 norm-one points, 1,128 unordered labelled squared pair distances, SHA-256 339134e166ccf3322d9aff9244f9bd488de71013a3c27992297ae155d046c550.

The entire D43 scientific source tag with all previous ancestral source archives is preserved without modification at prior/d43/frozen_scientific_tag_v0.1.0.zip: exactly 2,046,815 bytes, 28 entries, valid ZIP CRC and SHA-256 a009bf83bbca8f3b343c29afb470f647a8dd8fdbde176051c8f3d1ad34b512e1. The original certificate member is extracted byte-identically to prior/d43/results/certificate_d43.json. Both verifier implementations check ZIP checksum, CRC, certificate byte equality and original certificate SHA-256. Compressed archival ancestry avoids Windows maximum path length failures without changing earlier scientific work.

Zero-extend each original unit point p_i to q_i=(p_i,0), i=1,...,48, and adjoin a new perpendicular norm-one point q49=e45. All old inner products and squared distances remain unchanged with their pair labels. Each new squared distance equals ||q49-q_i||²=1+1-2<q49,q_i>=2. Therefore C(49,2)=1176=1128+48 unordered labelled pairs.

## 2. Exact rational Euclidean Gram and minimal realization

Seven original canonical unit vertices form a rational Gram block of rank three with pair products 3*x_i*x_j+y_i*y_j+z_i*z_j. Five centered simplex unit vertices form an independent rank-four Gram block with diagonal one and off-diagonal entries -1/4. Thirty-seven further mutually perpendicular unit coordinate vectors are orthogonal to the two blocks. Full exact rational Gram G is PSD with unit diagonal and rank 3+4+37=44.

Define squared-distance matrix D by D_ii=0 and D_ij=2-2G_ij. With H=I-(1/49)11^T the centered Euclidean Gram B=-(1/2)HDH=HGH is positive semidefinite of exact rank 44. The original antipodal canonical pair places the origin in their affine hull. Consequently every realization of this specific complete labelled Euclidean metric requires at least 44 affine dimensions; the explicit construction attains 44.

## 3. Exhaustive exact labelled squared distances

For unit radius define normalized class k=4d²/R². Precisely eight classes occur: k=4 on six pairs; k=7 on two; k=8 on 1,145; k=9 on three; k=10 on ten; k=12 on six; k=13 on two; k=16 on two. Total counts equal 1,176 labelled unordered pairs. Their squared distances sum exactly to 9455/4 for R=1.

All 1,128 previous pair values are checked with original labels against the authenticated D43 certificate. A histogram-preserving label permutation cannot pass full labelled conservation and is explicitly rejected.

## 4. Ideal graph stipulated independently

Choose a separate abstract complete graph with scalar unit masses and symmetric weights w_ij=1/d_ij². The new perpendicular unit point joins each of 48 predecessor points with weight 1/2. The weighted graph Laplacian is

L44 = [ L43+(1/2)I48          -(1/2)1_48 ]
      [ -(1/2)1_48^T                    24 ].

The uniform-join recurrence is chi49(z)=z(z-49/2)chi48(z-1/2)/(z-1/2). Let f6(z)=chi_P7(z)/z be the inherited nonzero seven-point canonical graph factor. The model-specific closed expression is chi49(z)=z(z-49/2)^38(z-24)^4*f6(z-21).

Two exact rational matrix computations verify nullity(L44-49/2 I)=38 and nullity(L44-24I)=4. These dimensionless eigenvalues are properties of this stipulated mathematical graph, not observed acoustic or particle frequencies, physical resonance or extra physical dimensions.

## 5. Two separate exact verifiers and adversarial tests

The primary program src/verify_d44.py constructs the complete exact rational Gram and 1,176 squared-distance labels, authenticates the complete frozen D43 archive and certificate, checks all inherited 1,128 pairs and centered Euclidean and graph eigenspace ranks. Four main adversarial controls detect a corrupted squared distance, duplicate point, nonorthogonal tilt and histogram-preserving relabelling.

Independently, tests/independent_d44.py reconstructs all 1,176 pair distances using Python fractions.Fraction structural rules, without importing the primary Gram generator. It checks the same parent ZIP and original certificate by SHA and CRC, independently compares 1,128 old labels and all present pairs, and confirms exact Euclidean and ideal graph ranks. Both programs output an identical SHA-256 for results/certificate_d44.json. Public GitHub Actions reruns them and checks deterministic exact certificate bytes.

To reproduce: Python with sympy==1.14.0; run python src/verify_d44.py and python tests/independent_d44.py. Full frozen D43 scientific source and previous ancestors are retained in prior/d43/frozen_scientific_tag_v0.1.0.zip.

## 6. Scientific scope and references

Orthogonal Euclidean extensions and uniform joins of weighted graphs are well-established methods. This preprint documents one synthetic metric and one freely chosen ideal graph; it does not claim a novel universal theorem or experimental proof of 44 physical spacetime dimensions, resonances, particles or independently human peer-reviewed physics.

References: Gabriel St-Pierre, Polybrutus 43D (2026), DOI 10.5281/zenodo.24415111; frozen parent github.com/Topbrutus/polybrutus-d43 tag v0.1.0; original canonical seven-point geometry github.com/Topbrutus/polybrutus.
