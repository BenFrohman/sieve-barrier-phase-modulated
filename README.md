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
Maynard and Polymath8b. Stadlmann's arXiv:2608.31126 (31 August 2026),
titled "Bounded gaps between primes," is cited as a preprint announcing
\(240\); no priority claim is made, and that preprint is not treated as
the established record.

Earlier numerical claims (\(\rho\approx 1.0422\), \(H_1\le 208\) at
\(k=196\)), including the 13 September 2026 note
`attachments/breaking_the_parity_barrier_v2.pdf` (a conditional \(208\)
under the generalized Elliott–Halberstam conjecture), are **not
theorems of the written weights**. The canonical preprint states this
explicitly.

There is no Lean formalization in this repository and no
machine-checked certificate is claimed. A successful LaTeX build only
shows that the source compiles.

## Canonical source

- `paper/Frohman_Sieve_Barrier_Preprint_2026.tex` — canonical source,
  dated 23 November 2026. It is the standalone `.tex` from Zenodo
  record [24064752](https://doi.org/10.5281/zenodo.24064752) (MD5
  `db31d976f1526f066ee44f0809c4b6d1`, including the subsection "The
  obstruction for Conjecture…"), updated only in metadata, the
  Stadlmann bibliography title, the copyright line, and the deposition
  remark (which now cites the DOI).
- `paper/Frohman_Sieve_Barrier_Preprint_2026.pdf` — PDF rebuilt from
  that source on 23 November 2026. The zip's older PDF was not reused
  (broken content streams). The previous Zenodo preview PDF was out of
  sync with the standalone source and is not the committed file.

Please cite version DOI
[10.5281/zenodo.24064752](https://doi.org/10.5281/zenodo.24064752)
(concept DOI
[10.5281/zenodo.24064751](https://doi.org/10.5281/zenodo.24064751)),
or the metadata in `CITATION.cff`. File-by-file hashes, including
handoff hashes that did not match, are in `PROVENANCE.md`.

## Repository layout

| Path | What it is |
| --- | --- |
| `paper/Frohman_Sieve_Barrier_Preprint_2026.tex` / `.pdf` | Canonical 23 November 2026 source and rebuilt PDF |
| `paper/Frohman_Sieve_Barrier_Preprint_2026_Nov8.zip` | Published 8 November 2026 bundle from Zenodo 24064752 (older tex/pdf inside; kept byte-for-byte) |
| `Frohman_Local_Sieve_NoGo_2026.tex` / `.pdf` | 13 September 2026 Local Sieve NoGo note (also under `paper/archive/2026-09-13/`) |
| `Sieve-Barrier-Lemma.md` | 13 September 2026 lemma note (also under `notes/`) |
| `attachments/breaking_the_parity_barrier_v2.pdf` | **Superseded** 13 September 2026 document; not a theorem of the final weights |
| `PROVENANCE.md` | File-by-file dates, MD5 and SHA-256, and theorem vs. superseded-claim status |
| `LICENSE-paper` | CC BY 4.0 (paper, notes, and PDFs) |
| `LICENSE` | Apache-2.0 (repository code, including CI) |
| `NOTICE` | Authorship, credit, and citation request |

The NoGo source/PDF and the lemma note are at the repository root so
the tree includes the same named files as the 24064752 zip.

## License

Papers, notes, and PDFs are licensed under
[CC BY 4.0](LICENSE-paper). Repository code, including GitHub Actions
workflows, is licensed under [Apache-2.0](LICENSE). Credit Benjamin
Stanley Frohman as the author and, if you use the work, please cite it.

## Continuous integration

The Actions workflow checks committed archival hashes in `SHA256SUMS`,
rebuilds the canonical preprint (and the 13 September NoGo source) in
a side directory, and fails if LaTeX reports an undefined reference.
A green run is not a mathematical certificate. Engine differences can
change the PDF bytes; the committed official PDF is the file in
`paper/`.
