# Provenance

All hashes below were computed on this computer (America/Chicago) on
23 November 2026. Dates of historical files are the timestamps stored
inside the Nov 8 2026 zip or on the published Zenodo records.

The handoff named `/home/workdir/artifacts/` and
`/home/workdir/attachments/` as the original locations. Those paths do
not exist on this computer. Google Drive searches for the same
filenames returned no hits. Files were recovered from the author's
already-published Zenodo records:

- [10.5281/zenodo.24064752](https://doi.org/10.5281/zenodo.24064752)
  (concept [10.5281/zenodo.24064751](https://doi.org/10.5281/zenodo.24064751))
  for the no-go preprint, the Nov 8 zip, and the 13 September Local
  Sieve NoGo / lemma files packed in that zip.
- [10.5281/zenodo.24190360](https://doi.org/10.5281/zenodo.24190360)
  for `breaking_the_parity_barrier_v2.pdf`.

Nothing was reconstructed in order to force a hash match. The paper
was not rewritten.

## Status (read this first)

This repository archives a **no-go result**.

- Phase-modulated contour operators built from truncated prime-factor
  counts, with a phase that depends on \(n\) only through a fixed
  modulus (\(42/208\)), cannot isolate twin primes.
- Embedding Selberg weights commutes and does not raise Maynard's
  \(\rho\).
- The established unconditional bound remains \(H_1\le 246\)
  (Maynard, Polymath8b). This note does **not** claim an improvement
  on 246.
- Stadlmann, arXiv:2608.31126 (31 August 2026), is cited as a
  preprint announcing 240. No priority claim is made, and that
  preprint is not treated as the established record.
- Earlier numerical values \(\rho\approx 1.0422\), \(H_1\le 208\) at
  \(k=196\), and the 13 September 2026 note
  `attachments/breaking_the_parity_barrier_v2.pdf` (a conditional 208
  under the generalized Elliott–Halberstam conjecture) are **not
  theorems of the written weights**. The canonical preprint states
  this explicitly (section "Claimed and not claimed," and Theorem 2).
- There is no Lean formalization here and no kernel certificate.

## Handoff hash check

| File named in the handoff | Expected SHA-256 | Result |
| --- | --- | --- |
| `Frohman_Sieve_Barrier_Preprint_2026.tex` (canonical standalone, 8 Nov 2026) | `da8461a616a38343cba84c13f866f1d7fa78f43d01167b0d9e340af0e8f1bbd7` | **Match.** The unaltered file is kept at `paper/archive/2026-11-08/` (MD5 `db31d976f1526f066ee44f0809c4b6d1`). It is also the parent of the current 23 November 2026 source. |
| Official Zenodo 24064752 PDF | `41380667606710be2b5f385ce0a95d3a71aa6e12ab6bc350f107214b284350b2` | **Match.** Kept unaltered at `paper/archive/2026-11-08/`. |
| Handoff PDF hash | `b5fb116ac2383984a752520aaa22ab1de7534f1b5ab0fffc692e533d91b74273` | **Not found.** Neither the official Zenodo PDF nor the PDF inside the Nov 8 zip has this hash. It was not reconstructed. |
| `Frohman_Sieve_Barrier_Preprint_2026_Zenodo.zip` | `42c5ac4d5786c545caedcec744b28593cd3a9d40cf275427c03b4a2c4fb7f0a7` | **Missing.** Not on this computer, in Drive, or among the files of Zenodo record 24064752. It was not reconstructed. The published archive is named `Frohman_Sieve_Barrier_Preprint_2026_Nov8.zip`. |

## Published 8 November 2026 files (`paper/archive/2026-11-08/`)

These are the published version, kept byte-for-byte and pin-hashed in
`SHA256SUMS`.

### `paper/archive/2026-11-08/Frohman_Sieve_Barrier_Preprint_2026.tex`

- Date in the source: 8 November 2026 (header comment still says
  13 September 2026; that line is left unaltered here).
- MD5: `db31d976f1526f066ee44f0809c4b6d1`
- SHA-256: `da8461a616a38343cba84c13f866f1d7fa78f43d01167b0d9e340af0e8f1bbd7`
- Size: 26657 bytes.
- Source: Zenodo record 24064752 standalone attachment.

### `paper/archive/2026-11-08/Frohman_Sieve_Barrier_Preprint_2026.pdf`

- Official deposited companion of that standalone source
  (Zenodo 24064752 default preview PDF).
- MD5: `19f05d1048da07b818a56481e3196f8d`
- SHA-256: `41380667606710be2b5f385ce0a95d3a71aa6e12ab6bc350f107214b284350b2`
- Size: 305380 bytes.

## Current preprint (23 November 2026 update)

Built from the standalone `.tex` attached to Zenodo 24064752 (MD5
`db31d976f1526f066ee44f0809c4b6d1`, SHA-256
`da8461a616a38343cba84c13f866f1d7fa78f43d01167b0d9e340af0e8f1bbd7`),
**not** from the older `.tex` inside the Nov 8 zip.

Edits relative to that standalone source, and only these:

- Header comment, `\date`, and the deposition remark set to
  23 November 2026. The remark now cites DOI
  `10.5281/zenodo.24064752` (concept `10.5281/zenodo.24064751`).
- Visible copyright line: `Copyright (c) 2026 Benjamin Stanley Frohman`.
- Affiliation: Independent Researcher, Texas, United States.
- Stadlmann bibliography title corrected to "Bounded gaps between
  primes" (arXiv:2608.31126v1, 31 August 2026 unchanged).
- Unresolved references in the previous preview PDF (`Zhang [?]`,
  `Lemma ??`, `Sections ??–??`) are resolved by a full LaTeX rebuild
  of this source. The standalone `.tex` already had the correct
  `\cite`/`\ref` keys and a `thebibliography` environment; the
  published preview PDF was out of sync.

A requested change of the numerical-check pair to `(167, 169)` was
**not** applied. In the source the pair is the mixed pair
`(167, 13^2)`: \(13^2=169\), so \(n=167\) is prime and \(n+2\) is a
square, contrasted with the twin pair `(41, 43)`. Both satisfy
\(\Omega_{11}=0,0\) and \(n\equiv 41\pmod{42}\). That is the example
used in the proof of the local sieve barrier (mixed pairs such as
\((p,q^2)\)), not a twin/prime-gap typo. PDF text extraction can
render `13^2` as `132`.

### `paper/Frohman_Sieve_Barrier_Preprint_2026.tex`

- Date in the source: 23 November 2026.
- MD5: `8046a55b112c540595f00e6e42c09ca8`
- SHA-256: `154fd381e864505f597917b30cc1fa8a12cb2f68a8226cbedbee9bc82d9a9d20`
- Size: 27129 bytes.
- This file is listed in `SHA256SUMS`. CI builds it; it does not
  replace the archived 8 November source.

### `paper/Frohman_Sieve_Barrier_Preprint_2026.pdf`

- Rebuilt from the current source above on 23 November 2026
  (pdfTeX 1.40.26, TeX Live 2025/dev/Debian). Not the official
  Zenodo 24064752 PDF and not the zip PDF.
- MD5: `c269fd40dbf3aca38aab59713ce076bc`
- SHA-256: `914d15e64784d95474aeebe952cb9d7ea92ff7d0c394988c9c6474b2d93a4812`
- Size: 326026 bytes.
- A later TeX Live rebuild may differ in bytes. CI compiles in a side
  directory and fails only on a compile error or an undefined
  reference, not on a current-PDF hash mismatch. The published
  8 November PDF remains pin-hashed under `paper/archive/2026-11-08/`.

## Nov 8 zip (byte-for-byte archival bundle)

### `paper/Frohman_Sieve_Barrier_Preprint_2026_Nov8.zip`

- SHA-256: `e7bbea3449eeeb13dddc50b99beffaf7f09bd94c82e0a9076c0ac5f422272525`
- MD5: `008011a80d25e16b3de7d277f549feb0`
- Size: 318719 bytes.
- Source: Zenodo 24064752.

Contents of the zip (not used as the canonical preprint):

| Inner file | Date in zip | MD5 | SHA-256 | Size | Notes |
| --- | --- | --- | --- | --- | --- |
| `Frohman_Sieve_Barrier_Preprint_2026.tex` | 8 Nov 2026, 23:30 | `56ab52c6d182e15c2784f6f27e22d4c0` | `298474ed3b6480256337749043659149f94f8e75abdbc8c2f0eadb2bae429e7b` | 25098 | Older source; missing the obstruction subsection. Not used. |
| `Frohman_Sieve_Barrier_Preprint_2026.pdf` | 8 Nov 2026, 23:30 | `755ceb284c50e97f69eb7fd93972b77a` | `18a4a0d2e98a49eb19d5b18d66b4dc43b74c3e5ce524dcb610a069566c4d28a2` | 305222 | Broken content streams. Not reused. |
| `Frohman_Local_Sieve_NoGo_2026.tex` | 13 Sep 2026, 16:49 | `b0eb68730d75943b1b58eccc568f98b2` | `0fb5eb737d15b23ceb31bfb9531ab90fad907f5d5720d071b7a232f362e430bb` | 11209 | Committed (see below). |
| `Frohman_Local_Sieve_NoGo_2026.pdf` | 13 Sep 2026, 14:53 | `f8726da0ea9832d35a3eacb00056fcbe` | `d81f6f68a65daad1c6590f67033e68dd31fa0c50e2980ab053658f7cc9124c6e` | 9188 | Committed (see below). |
| `Sieve-Barrier-Lemma.md` | 13 Sep 2026, 16:41 | `3fa87c7cb94a454f8e276918cbf8937e` | `3e3937854f688b09329b91f7cd5951470781717d07404a64e7d5998bc6e4379b` | 5730 | Committed (see below). |

## 13 September 2026 files (unchanged historical copies)

These dates are the original document dates and were not rewritten.
Copies at the repository root match the zip layout of record 24064752;
identical copies also sit under `paper/archive/2026-09-13/` and
`notes/`.

### `Frohman_Local_Sieve_NoGo_2026.tex` and `paper/archive/2026-09-13/Frohman_Local_Sieve_NoGo_2026.tex`

- SHA-256: `0fb5eb737d15b23ceb31bfb9531ab90fad907f5d5720d071b7a232f362e430bb`
- MD5: `b0eb68730d75943b1b58eccc568f98b2`
- Size: 11209 bytes.
- Status: earlier (13 September 2026) no-go note. Not the canonical
  23 November 2026 preprint.

### `Frohman_Local_Sieve_NoGo_2026.pdf` and `paper/archive/2026-09-13/Frohman_Local_Sieve_NoGo_2026.pdf`

- SHA-256: `d81f6f68a65daad1c6590f67033e68dd31fa0c50e2980ab053658f7cc9124c6e`
- MD5: `f8726da0ea9832d35a3eacb00056fcbe`
- Size: 9188 bytes.

### `Sieve-Barrier-Lemma.md` and `notes/Sieve-Barrier-Lemma.md`

- SHA-256: `3e3937854f688b09329b91f7cd5951470781717d07404a64e7d5998bc6e4379b`
- MD5: `3fa87c7cb94a454f8e276918cbf8937e`
- Size: 5730 bytes.
- Status: 13 September 2026 lemma note packed in the Nov 8 zip.

## Superseded attachment

### `attachments/breaking_the_parity_barrier_v2.pdf` and `paper/archive/2026-09-13/breaking_the_parity_barrier_v2.pdf`

- SHA-256: `0b0e75ccbd2419d075de03c130b972bea72f0283522ba1c11bfab93e259efe29`
- MD5: `b508303c4f8c063a0366e19751c50d25`
- Size: 284737 bytes.
- Source: Zenodo [24190360](https://zenodo.org/records/24190360).
- Status: **superseded.** 13 September 2026 sequence formalization
  claiming a conditional 208 under GEH. Not a theorem of the written
  weights of the canonical preprint. See `attachments/README.md`.

## GitHub starting point

`BenFrohman/sieve-barrier-phase-modulated` at
`0220ac557d5a932a752ab28a3587116fd1fe9d77` (created 23 November 2026,
15:27 America/Chicago) contained 11-byte `PLACEHOLDER` stubs for the
paper files, except `README.md`. Those stubs are replaced by this
branch. The existing public visibility of the repository was not
changed.
