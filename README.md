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

## Published 8 November 2026 version and current source

Both are kept. Neither replaces the other.

- `paper/archive/2026-11-08/Frohman_Sieve_Barrier_Preprint_2026.tex`
  and `.pdf` — the unaltered published 8 November 2026 standalone
  source and official Zenodo 24064752 PDF, kept byte-for-byte.
  SHA-256 `da8461a616a38343cba84c13f866f1d7fa78f43d01167b0d9e340af0e8f1bbd7`
  (tex) and
  `41380667606710be2b5f385ce0a95d3a71aa6e12ab6bc350f107214b284350b2`
  (PDF). These hashes are pinned in `SHA256SUMS`.
- `paper/Frohman_Sieve_Barrier_Preprint_2026.tex` — current source,
  dated 23 November 2026. It is that same standalone `.tex` (MD5
  `db31d976f1526f066ee44f0809c4b6d1`, including the subsection "The
  obstruction for Conjecture…"), updated only in metadata: the date,
  DOI in Remark 1, Stadlmann bibliography title, copyright line, and
  affiliation "Independent Researcher, Texas, United States."
- `paper/Frohman_Sieve_Barrier_Preprint_2026.pdf` — PDF rebuilt from
  the current source. The zip's older PDF was not reused (broken
  content streams). CI rebuilds this source in a side directory; a
  later TeX Live run may differ in bytes from the committed PDF.

Please cite version DOI
[10.5281/zenodo.24064752](https://doi.org/10.5281/zenodo.24064752)
(concept DOI
[10.5281/zenodo.24064751](https://doi.org/10.5281/zenodo.24064751)),
or the metadata in `CITATION.cff`. File-by-file hashes, including
handoff hashes that did not match, are in `PROVENANCE.md`.

## Repository layout

| Path | What it is |
| --- | --- |
| `paper/Frohman_Sieve_Barrier_Preprint_2026.tex` / `.pdf` | Current 23 November 2026 source and rebuilt PDF |
| `paper/archive/2026-11-08/` | Unaltered published 8 November 2026 source and official Zenodo PDF, byte-for-byte |
| `paper/Frohman_Sieve_Barrier_Preprint_2026_Nov8.zip` | Published 8 November 2026 bundle from Zenodo 24064752 (older tex/pdf inside; kept byte-for-byte) |
| `Frohman_Local_Sieve_NoGo_2026.tex` / `.pdf` | 13 September 2026 Local Sieve NoGo note (also under `paper/archive/2026-09-13/`) |
| `Sieve-Barrier-Lemma.md` | 13 September 2026 lemma note (also under `notes/`) |
| `attachments/breaking_the_parity_barrier_v2.pdf` and `paper/archive/2026-09-13/breaking_the_parity_barrier_v2.pdf` | **Superseded** 13 September 2026 document; not a theorem of the final weights |
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

The Actions workflow checks the archived 8 November 2026 files (and
the other committed sources listed in `SHA256SUMS`) against their
SHA-256 hashes, then rebuilds the current 23 November 2026 source
(and the 13 September NoGo source) in a side directory. It fails if
LaTeX reports an undefined reference. A green run is not a
mathematical certificate. The current PDF is built by CI; engine
differences can change those bytes, so the current PDF is not pin-hashed.
The published 8 November PDF remains pin-hashed under
`paper/archive/2026-11-08/`.
