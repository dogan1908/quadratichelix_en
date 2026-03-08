# From the Quadratic Sequence to the Conical Helix

**Von der quadratischen Folge zur Kegelhelix**

*Dogan Balban, 2026*

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo..svg)](https://doi.org/10.5281/zenodo.)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

---

## Overview

This work develops a complete analytical and geometric framework for the
quadratic integer sequence

$$k(n) = \frac{2n^2 + 3n + 1}{6},$$

which takes integer values precisely for $n \equiv 1, 5 \pmod{6}$.

From the difference structure of this sequence—via a proven
uniqueness statement—an Archimedean spiral with slope constant
$a = 6/\pi^2 = 1/\zeta(2)$ is derived. Its extension by a linear
height function yields a three-dimensional conical helix on a right
circular cone with half-angle $\alpha = \arctan(2/\pi) \approx 32.48°$.

The algebraic core of the construction is the fundamental identity
$(4n+3)^2 = 48\,k(n)+1$, which defines a universal quantity
$Q(k) = \sqrt{48k+1}$ from which all three helix coordinates
follow as exact closed functions.

As a corollary, **all primes $p > 3$** appear as a distinguished
subset of the integer points on the helix.

---

## Project Structure

```
.
├── main.tex                    # Main file (pdflatex + biber)
├── references.bib              # Bibliography
├── chapters/
│   ├── abstract.tex            # Abstract (EN)
│   ├── vorwort.tex             # Preface
│   ├── 01_einleitung.tex       # Introduction and motivation
│   ├── 02_arithmetik.tex       # Arithmetic foundations
│   ├── 02a_distances.tex       # Euclidean distances
│   ├── 02b_distanz_sequenzen.tex # Distance sequences
│   ├── 03_spirale.tex          # Archimedean spiral (uniqueness)
│   ├── 04_parametrisierung.tex # p-parametrisation
│   ├── 05_bogenlaenge.tex      # Arc length of the spiral
│   ├── 05a_bogenlaenge_spirale.tex # Arc length (detailed)
│   ├── 05b_bogenlaenge_parabel.tex # Arc length of the parabola
│   ├── 06_taylor.tex           # Taylor approximation
│   ├── 07_kegel.tex            # Conical form as 3D envelope
│   ├── 08_helix.tex            # The conical helix
│   ├── 08a_helixprimes.tex     # Prime numbers on the helix
│   ├── 08b_parabelhelix.tex    # Height function from the parabola
│   ├── 09_beispiele.tex        # Arc-length comparison
│   ├── 10_formelsammlung.tex   # Formula collection
│   ├── 11_zusammenfassung.tex  # Summary and outlook
│   ├── 12_grafiken.tex         # Figures and plots
│   ├── 13_visualisierung.tex   # Q-parametrisation and rays
│   ├── 14_kegelstrahlen.tex    # Geometry of the cone generators
│   └── appendix.tex            # Appendix (Python code, verification)
├── bilder/                     # Figures (JPEG/PNG)

```

## Compilation

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

Requirements: TeX Live 2023+ or MiKTeX with the packages
`amsmath`, `tcolorbox`, `booktabs`, `biblatex`, `hyperref`, `siunitx`,
`graphicx`, `geometry`, `babel` (english).

## Central Results

| Result | Formula |
|--------|---------|
| Spiral equation | $r(\theta) = \frac{6}{\pi^2}\,\theta$ |
| Radial difference | $\Delta R = \frac{12}{\pi}$ |
| Helix parametrisation | $\gamma(\theta) = \bigl(\frac{6}{\pi^2}\theta\cos\theta,\; \frac{6}{\pi^2}\theta\sin\theta,\; -\frac{3}{4}+\frac{3}{\pi}\theta\bigr)$ |
| Fundamental identity | $(4n+3)^2 = 48\,k(n)+1$ |
| Integer points | $\theta_n = \frac{\pi}{3}n + \frac{\pi}{4}$ |
| Half-angle | $\alpha = \arctan(2/\pi) \approx 32.48°$ |

## MSC 2020

11B25 (Arithmetic progressions) · 53A04 (Curves in Euclidean and related spaces) ·
11A41 (Primes) · 11B83 (Special sequences and polynomials)

## Interactive Visualisations

The spiral and helix can be explored interactively in
[Desmos](https://www.desmos.com/calculator).
Archimedean equidistant spiral: https://www.desmos.com/calculator/auwyillfll
Conical Helix Spiral: https://www.desmos.com/3d/drdt62xmz9
Quadratic curve: https://www.desmos.com/calculator/f71643ebff

## License

This work is licensed under the
[Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

## Citation

```bibtex
@misc{Balban2026,
  author       = {Balban, Dogan},
  title        = {From the Quadratic Sequence to the Conical Helix},
  year         = {2026},
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.18819019},
  url          = {https://doi.org/10.5281/zenodo.}
}
```

## Contact

- GitHub: [dogan1908](https://github.com/dogan1908)
