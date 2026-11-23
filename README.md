# On the Local Commutation Limits of Phase-Modulated Sieve Operators

**Author:** Benjamin Stanley Frohman
([ORCID 0009-0006-7068-3718](https://orcid.org/0009-0006-7068-3718)),
Independent Researcher, Texas, United States.

**Status: this is a no-go result. It is not a proof of the twin-prime
conjecture, and it does not claim an improvement on the established
unconditional bound \(H_1\le 246\).**

Phase-modulated contour operators built from truncated prime-factor
counts, with a phase that depends on \(n\) only through a fixed modulus
(\(42/208\)), cannot isolate twin primes. Embedding Selberg weights in
the same contour commutes: the integral factors off as a function of
the residue class and leaves the quadratic weight unchanged, so it does
not raise Maynard's \(\rho\).

The established unconditional bound remains \(H_1\le 246\), due to
Maynard and Polymath8b. Stadlmann's arXiv:2608.31126 (31 August 2026)
is cited as a preprint announcing \(240\); no priority claim is made,
and that preprint is not treated as the established record.

Earlier numerical claims (\(\rho\approx 1.0422\), \(H_1\le 208\) at
\(k=196\)), including the 13 September 2026 note
`breaking_the_parity_barrier_v2.pdf` (a conditional \(208\) under the
generalized Elliott–Halberstam conjecture), are **not theorems of the
written weights**. The canonical preprint states this explicitly.

There is no Lean formalization in this repository and no
machine-checked certificate is claimed. A successful LaTeX build only
shows that the source compiles.

## Canonical source

- `paper/Frohman_Sieve_Barrier_Preprint_2026.tex` — canonical source,
  dated 8 November 2026. SHA-256 matches the handoff hash
  `da8461a616a38343cba84c13f866f1d7fa78f43d01167b0d9e340af0e8f1bbd7`.
- `paper/Frohman_Sieve_Barrier_Preprint_2026.pdf` — the official PDF
  deposited with that source on Zenodo (version DOI
  [10.5281/zenodo.24064752](https://doi.org/10.5281/zenodo.24064752),
  9 November 2026; concept DOI
  [10.5281/zenodo.24064751](https://doi.org/10.5281/zenodo.24064751)).
  See `PROVENANCE.md` for a hash note: the PDF SHA-256 of this deposited
  file differs from one hash recorded in the archival handoff; the paper
  content was not altered to force a match.

Please cite the DOI above, or the metadata in `CITATION.cff`. The text
of the preprint still contains a deposition-status remark written before
the 9 November 2026 upload; that remark is left unchanged.

## Repository layout

| Path | What it is |
| --- | --- |
| `paper/` | Current (8 November 2026) source, official PDF, and the Nov 8 bundle |
| `paper/archive/2026-09-13/` | Earlier 13 September Local Sieve NoGo note, and the historical parity-barrier v2 PDF |
| `Sieve-Barrier-Lemma.md` | 13 September lemma note (also packed in the Nov 8 bundle) |
| `PROVENANCE.md` | File-by-file dates, SHA-256 hashes, and theorem vs. superseded-claim status |
| `LICENSE-paper` | CC BY 4.0 |
| `NOTICE` | Authorship, credit, and citation request |

## License

The materials in this repository are licensed under
[CC BY 4.0](LICENSE-paper). Credit Benjamin Stanley Frohman as the
author and, if you use the work, please cite it.

## Continuous integration

The Actions workflow compiles the canonical `.tex` in a side directory
and checks the committed archival hashes. A green run is not a
mathematical certificate. The official deposited PDF is the file in
`paper/`, not a CI rebuild (engine differences can change pagination).
