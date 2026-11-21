# Polybrutus 44D — Exact rational Euclidean labelled squared-distance metric

## Immutable scientific parent and complete source lineage

Frozen source: `Topbrutus/polybrutus-d43@v0.1.0`, scientific commit `e435e38aed88e8c65d294eeee26bee6b89056fc8`, DOI `10.5281/zenodo.24415111`, certificate SHA-256 `339134e166ccf3322d9aff9244f9bd488de71013a3c27992297ae155d046c550`. Parent: 48 norm-one points and 1,128 unordered labelled squared-distance pairs.

The complete original scientific tag **including all ancestors** is preserved byte-identically in `prior/d43/frozen_scientific_tag_v0.1.0.zip`: SHA-256 `a009bf83bbca8f3b343c29afb470f647a8dd8fdbde176051c8f3d1ad34b512e1`, 28 ZIP entries and valid CRC. Its original `results/certificate_d43.json` is extracted to `prior/d43/results/certificate_d43.json`. Both independent checking implementations verify the full archive hash, CRC, byte-identical certificate entry and original certificate SHA-256.

## Exact orthogonal Euclidean construction

Embed all 48 predecessor norm-one points `p_i` as `q_i=(p_i,0)`. Append an additional perpendicular norm-one point `q49=e45`. Every old squared distance remains unchanged with its label, and each new pair obeys `||q49-q_i||²=1+1-2<q49,q_i>=2`. Therefore `C(49,2)=1176=1128+48` exact labelled unordered squared-distance pairs result.

The seven canonical original norm-one points form a rational rank-three Gram block with products `3*x_i*x_j+y_i*y_j+z_i*z_j`. Five centered regular-simplex unit points form an independent rank-four Gram block, unit diagonal and off-diagonal `-1/4`. Thirty-seven additional mutually perpendicular norm-one axes are orthogonal to both. Full Gram `G` has unit diagonal, is positive semidefinite by explicit Gram construction and has exact rational rank `3+4+37=44`.

Let `D_ii=0`, `D_ij=2-2G_ij` and projector `H=I-11ᵀ/49`. The unique centered Euclidean Gram for the complete labelled squared-distance matrix is `B=-(1/2)HDH=HGH`, exact rank **44**. An inherited antipodal pair places the origin in the affine hull, so the **minimum Euclidean affine realization dimension** for this specific complete labelled metric is exactly 44; ambient storage requires 45 coordinates.

## Exhaustive unit-radius invariants

```text
Norm-one labelled points                      49
Unordered labelled squared-distance pairs   1176
Frozen D43 labelled parent pairs preserved   1128/1128
New squared-distance pairs                   48 × 2
Histogram k=4*d²/R²                          4:6 7:2 8:1145 9:3 10:10 12:6 13:2 16:2
Sum of squared distances at R=1              9455/4
Minimum affine/centered Gram rank            44
Ambient coordinate storage count             45
```

## Ideal graph chosen separately from the metric

Choose a complete graph with unit scalar masses and symmetric weights `w_ij=R²/d_ij²`. The new point connects uniformly to all 48 earlier vertices with weight 1/2, yielding block weighted Laplacian:

```text
L44 = [ L43 + I48/2       -1_48/2 ]
      [ -1_48ᵀ/2                24 ].
```

Exact characteristic polynomial recurrence: `chi49(z)=z(z-49/2)chi48(z-1/2)/(z-1/2)`. Writing `f6(z)=chi_P7(z)/z` for the original canonical seven-point graph's nonzero factor, the model-specific closed expression is `chi49(z)=z(z-49/2)^38(z-24)^4*f6(z-21)`. Separate exact rational matrix nullity checks show `nullity(L44-49/2 I)=38` and `nullity(L44-24I)=4`. These are **dimensionless chosen-model eigenmodes**, not measured physical frequencies.
