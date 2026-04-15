# pdt-arithmetic-geometry
Verification code for "Arithmetic Geometry at the Pisot Boundary" — five arithmetic theorems and the Dimensional Norm-Hodge Theorem for the PDT polynomials
# Arithmetic Geometry at the Pisot Boundary

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stalex444/pdt-arithmetic-geometry/blob/main/pdt_arithmetic_geometry.ipynb)

Companion repository for:

**"Arithmetic Geometry at the Pisot Boundary: Galois Groups, Class Fields, and Implications for Physical Geometry and Loop Quantum Gravity"**  
Stephanie Alexander, Baryonix Corp., April 2026  
Zenodo DOI: https://doi.org/10.5281/zenodo.19561374

---

## What This Repository Contains

| File | Description |
|------|-------------|
| `pdt_arithmetic_geometry.py` | Python script — proves and verifies all six theorems |
| `pdt_arithmetic_geometry.ipynb` | Jupyter notebook — same script, runnable in one click via Colab |
| `VERIFIED_OUTPUT.txt` | Complete verified output from Google Colab (Python 3.12.13, SymPy 1.14.0) |

---

## Results Verified

The script proves five theorems in algebraic number theory and one arithmetic-geometric theorem for the two Pisot polynomials:

```
x³ - x - 1 = 0    root ρ ≈ 1.32472    (ρ-sector polynomial, degree 3)
x⁴ - x - 1 = 0    root Q ≈ 1.22074    (Q-sector polynomial, degree 4)
```

| Theorem | Result |
|---------|--------|
| 1 | N(ρ) = +1, N(Q) = −1 (unit norms, forced by polynomial structure) |
| 2 | Gal(ℚ(ρ)/ℚ) = S₃, Gal(ℚ(Q)/ℚ) = S₄ (maximal Galois groups) |
| 3 | disc(x³−x−1) = −23 (prime), disc(x⁴−x−1) = −283 (prime) |
| 4 | Splitting field of x³−x−1 = Hilbert class field of ℚ(√−23) |
| 5 | h(ℚ(√−23)) = h(ℚ(√−283)) = 3 (equal class numbers — established computationally) |
| 6 | N(αₙ) = (−1)ⁿ⁺¹ = ★² in n-dimensional physical geometry |

**Physical corollaries:**

| Corollary | Result |
|-----------|--------|
| A | Barbero–Immirzi parameter γ_BI = λ₄ × ρ = 0.239545... (zero free parameters) |
| B | Artin L-function of std₂-rep of S₃ = weight-1 newform of level 23 (Langlands) |

---

## How to Run

### Option 1: One-click in browser (no installation)
Click the **Open in Colab** badge above. Run all cells. Takes under 60 seconds.

### Option 2: Local Python
```bash
pip install sympy
python3 pdt_arithmetic_geometry.py
```

### Option 3: Read the output
See `VERIFIED_OUTPUT.txt` for the complete output from a verified Colab run.

**Verified environments:**
- Google Colab: Python 3.12.13, SymPy 1.14.0
- Local: Python 3.12.3, SymPy 1.14.0

No dependencies beyond sympy.

---

## Sample Output

```
====================================================================
  THEOREM 4: SPLITTING FIELD OF x^3-x-1 = HILBERT CLASS FIELD OF Q(sqrt(-23))
====================================================================
  h(Q(sqrt(-23))) = 3

  *** THEOREM 4 VERIFIED ***
  The splitting field of x^3-x-1 = Hilbert class field of Q(sqrt(-23)).
  rho generates the class field of Q(sqrt(-23)) (class number 3).
  rho is arithmetically equivalent to a special value of the j-function.

====================================================================
  PHYSICAL COROLLARY A: BARBERO-IMMIRZI PARAMETER OF LQG
====================================================================
  gamma_BI = lambda_4 * rho = 0.2395454187

  Published values from black hole entropy matching:
    Meissner (2004):            gamma = 0.2375
    Domagala-Lewandowski (2004):gamma = 0.2427
    PDT derivation:             gamma = 0.2395

  Match to Meissner:  99.14%
  Match to DL:        98.70%
```

---

## Connection to PDT

Pisot Dimensional Theory derives fundamental physical constants from the algebraic boundary between x³=x+1 and x⁴=x+1. The arithmetic properties established here — prime discriminants, maximal Galois groups, unit norms ±1, Hilbert class field structure, and equal class numbers — provide the number-theoretic foundation for why these two polynomials organize physical reality.

**Key connections:**
- N(Q) = −1 = ★² on 2-forms in 4D Lorentzian spacetime → arithmetic origin of Ashtekar's self-dual/anti-self-dual decomposition in LQG
- N(ρ) = +1 = ★² in 3D Riemannian space → arithmetic origin of the spatial sector
- γ_BI = λ₄ρ → Barbero–Immirzi parameter derived with zero free parameters
- Splitting field of x³−x−1 = Hilbert class field of ℚ(√−23) → ρ is a CM value of the j-function
- Level 23 newform → PDT enters the Langlands program at the prime |disc(x³−x−1)|

For the full PDT framework see:
- GRF Essay 2026: "The Dimensional Origin of Newton's Constant" — 2026 Gravity Research Foundation Essay Contest


---

## Citation

```bibtex
@misc{alexander2026arithmetic,
  author    = {Alexander, Stephanie},
  title     = {Arithmetic Geometry at the Pisot Boundary: Galois Groups, 
               Class Fields, and Implications for Physical Geometry 
               and Loop Quantum Gravity},
  year      = 2026,
  publisher = Zenodo,
  doi       = https://doi.org/10.5281/zenodo.19561374
  url       = https://zenodo.org/records/19582084
}
```

---

## License

MIT License — free to use, verify, and build on with attribution.
