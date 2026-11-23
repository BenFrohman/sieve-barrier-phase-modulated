# Provenance

All hashes below are SHA-256, computed on this machine after the files
were copied and before they were committed. Paper sources and PDFs were
not edited.

The handoff named `/home/workdir/artifacts/` and
`/home/workdir/attachments/` as the original locations. Those paths do
not exist on this computer. Files were recovered from the author's
already-published Zenodo records and, where packed, from
`Frohman_Sieve_Barrier_Preprint_2026_Nov8.zip`. Drive searches for the
same filenames returned no hits.

## Handoff hash check

| File named in the handoff | Expected SHA-256 | Result |
| --- | --- | --- |
| `Frohman_Sieve_Barrier_Preprint_2026.tex` (canonical, 8 Nov 2026) | `da8461a616a38343cba84c13f866f1d7fa78f43d01167b0d9e340af0e8f1bbd7` | **Match.** This is the committed `paper/*.tex`. |
| `Frohman_Sieve_Barrier_Preprint_2026.pdf` | `b5fb116ac2383984a752520aaa22ab1de7534f1b5ab0fffc692e533d91b74273` | **Not found.** Neither the official Zenodo PDF nor the PDF inside the Nov 8 zip has this hash. The paper was not altered to force a match. |
| `Frohman_Sieve_Barrier_Preprint_2026_Zenodo.zip` | `42c5ac4d5786c545caedcec744b28593cd3a9d40cf275427c03b4a2c4fb7f0a7` | **Missing.** The file was not on this computer, in Drive, or among the files of Zenodo record 24064752. It was not reconstructed. |

The Nov 8 bundle is a different zip than the missing `*_Zenodo.zip`.
Its hash is recorded below and was not expected to equal the Zenodo.zip
hash.

## Current files (`paper/`)

### `paper/Frohman_Sieve_Barrier_Preprint_2026.tex`

- Date in the source: 8 November 2026.
- SHA-256: `da8461a616a38343cba84c13f866f1d7fa78f43d01167b0d9e340af0e8f1bbd7`
- Size: 26657 bytes.
- Source: Zenodo record [24064752](https://zenodo.org/records/24064752)
  (`md5:db31d976f1526f066ee44f0809c4b6d1`, confirmed).
- Status: **canonical source of the no-go preprint.** Theorem content is
  the local sieve barrier and the commutation statement that the written
  contour and penalty families do not raise Maynard's \(\rho\). The
  established unconditional bound remains \(H_1\le 246\). Earlier
  numerical values \(0.0211\), \(1.0422\), \(k=196\), and \(H_1\le 208\)
  are stated in the text as not theorems of those weights.

### `paper/Frohman_Sieve_Barrier_Preprint_2026.pdf`

- Official deposited companion of the canonical source above.
- SHA-256: `41380667606710be2b5f385ce0a95d3a71aa6e12ab6bc350f107214b284350b2`
- Size: 305380 bytes. 8 pages. Producer: pdfTeX-1.40.25. CreationDate:
  8 November 2026, 17:30:32 CST (America/Chicago).
- Source: the same Zenodo record (`md5:19f05d1048da07b818a56481e3196f8d`,
  confirmed).
- Status: **official PDF of the no-go preprint.** A later TeX Live
  rebuild of the same `.tex` may differ in pagination; CI compiles in a
  side directory and does not replace this file.
- The handoff expected SHA-256
  `b5fb116ac2383984a752520aaa22ab1de7534f1b5ab0fffc692e533d91b74273`
  was not located anywhere this archival pass could reach.

### `paper/Frohman_Sieve_Barrier_Preprint_2026_Nov8.zip`

- SHA-256: `e7bbea3449eeeb13dddc50b99beffaf7f09bd94c82e0a9076c0ac5f422272525`
- Size: 318719 bytes.
- Source: the same Zenodo record (`md5:008011a80d25e16b3de7d277f549feb0`,
  confirmed).
- Status: **archival bundle**, kept byte-for-byte. It contains an
  earlier 8 November 23:30 snapshot of the preprint (tex 25098 bytes,
  sha256 `298474ed3b6480256337749043659149f94f8e75abdbc8c2f0eadb2bae429e7b`;
  pdf 305222 bytes, sha256
  `18a4a0d2e98a49eb19d5b18d66b4dc43b74c3e5ce524dcb610a069566c4d28a2`)
  together with the 13 September Local Sieve NoGo source/PDF and
  `Sieve-Barrier-Lemma.md`. The zip-internal preprint `.tex` differs
  from the canonical deposited `.tex` by the addition, in the
  deposited source, of a `proposition` environment and the subsection
  “The obstruction for Conjecture (weight).” Those inner files are not
  also unpacked under `paper/` so that “current” stays unambiguous.

## Earlier and historical files

### `Sieve-Barrier-Lemma.md`

- File date inside the Nov 8 zip: 13 September 2026, 16:41.
- SHA-256: `3e3937854f688b09329b91f7cd5951470781717d07404a64e7d5998bc6e4379b`
- Size: 5730 bytes.
- Source: extracted unchanged from `Frohman_Sieve_Barrier_Preprint_2026_Nov8.zip`.
- Status: **early write-up of the local sieve barrier and commutation
  no-go** (same negative conclusion as the later preprint). Not a claim
  of \(H_1=2\) and not an improvement on 246.

### `paper/archive/2026-09-13/Frohman_Local_Sieve_NoGo_2026.tex`

- File date inside the Nov 8 zip: 13 September 2026, 16:49.
- SHA-256: `0fb5eb737d15b23ceb31bfb9531ab90fad907f5d5720d071b7a232f362e430bb`
- Size: 11209 bytes.
- Source: extracted unchanged from the Nov 8 zip.
- Status: **earlier (13 September) no-go note**, superseded as the
  canonical write-up by the 8 November preprint, but already a negative
  result. The text states that it does not claim \(H_1\le 208\).

### `paper/archive/2026-09-13/Frohman_Local_Sieve_NoGo_2026.pdf`

- File date inside the Nov 8 zip: 13 September 2026, 14:53.
- SHA-256: `d81f6f68a65daad1c6590f67033e68dd31fa0c50e2980ab053658f7cc9124c6e`
- Size: 9188 bytes.
- Source: extracted unchanged from the Nov 8 zip.
- Status: **PDF companion of the 13 September no-go note.**

### `paper/archive/2026-09-13/breaking_the_parity_barrier_v2.pdf`

- PDF CreationDate: 13 September 2026, 11:51:04 CDT (America/Chicago).
- SHA-256: `0b0e75ccbd2419d075de03c130b972bea72f0283522ba1c11bfab93e259efe29`
- Size: 284737 bytes. 6 pages. Producer: pdfTeX-1.40.24.
- Source: the handoff path
  `/home/workdir/attachments/breaking_the_parity_barrier_v2.pdf` was
  not present. The file of this exact name was retrieved from the
  author's later deposit
  [10.5281/zenodo.24190360](https://doi.org/10.5281/zenodo.24190360)
  (published 17 November 2026 under the title “Breaking the Parity
  Barrier: Non-Symmetric Sieve Weights with Directional Phase Shift
  (v2, 2026)”; `md5:b508303c4f8c063a0366e19751c50d25`, confirmed). The
  PDF date matches the 13 September 2026 handoff description.
- Status: **historical / superseded numerical claim, not a theorem of
  the written weights in the canonical preprint.** The note claims,
  conditionally on the generalized Elliott–Halberstam conjecture, that
  \(\rho=1.0422>1\) and \(H_1\le 208\) at \(k=196\). The 8 November
  preprint explicitly rejects those figures as theorems of the written
  contour and penalty families.

## Missing file

- `Frohman_Sieve_Barrier_Preprint_2026_Zenodo.zip`, expected SHA-256
  `42c5ac4d5786c545caedcec744b28593cd3a9d40cf275427c03b4a2c4fb7f0a7`.
  Not found. Not recreated.

## Related public records (not copied in as “current”)

These already exist and are listed only for orientation. They are not
the 8 November canonical source archived in `paper/`.

- [10.5281/zenodo.24064752](https://doi.org/10.5281/zenodo.24064752) —
  the canonical preprint (this repository’s official artifact).
- [10.5281/zenodo.24190360](https://doi.org/10.5281/zenodo.24190360) —
  historical v2 “Breaking the Parity Barrier” PDF archived above.
- [10.5281/zenodo.24191003](https://doi.org/10.5281/zenodo.24191003) and
  [10.5281/zenodo.24191007](https://doi.org/10.5281/zenodo.24191007) —
  later (13 November 2026) related notes under nearby titles. Not treated
  here as replacements for the 8 November source.

A public GitHub repository for this title already existed as
[BenFrohman/sieve-barrier-phase-modulated](https://github.com/BenFrohman/sieve-barrier-phase-modulated)
(created 23 November 2026). Its `main` branch held 11-byte
`PLACEHOLDER` stand-ins for the paper files and a short README. This
archival work is a branch and pull request on that repository; `main`
history is not rewritten.
