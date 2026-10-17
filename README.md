# Infinite Laplace Equation

## Project Overview

This repository contains candidate results on interior and boundary regularity for equations involving the infinite Laplacian, as well as on traveling wave solutions for such equations. The results were obtained by our team through extensive dialogue-based training with AI, following the same workflow as our previous work on the Lane–Emden-type conjecture. The team is currently working to verify all the results.

The infinite Laplacian, 

$$
\Delta_\infty u = \sum_{i,j=1}^{n} \frac{\partial u}{\partial x_i} \frac{\partial u}{\partial x_j} \frac{\partial^2 u}{\partial x_i \partial x_j},
$$

is a highly degenerate nonlinear elliptic operator that arises as the limit of the $p$-Laplacian as $p \to \infty$[reference:0]. It is the Euler–Lagrange equation of the $L^\infty$ variational problem for $|\nabla u|$, equivalently the absolutely minimizing Lipschitz extension (AMLE) problem[reference:1]. Because of its degeneracy, classical solution theories do not apply directly, and the equation is naturally studied through viscosity solutions. Regularity—both in the interior and at the boundary—remains a central and delicate issue, and traveling wave problems for nonlocal or degenerate variants introduce additional structural challenges. This repository documents our progress on these questions.

> **Status:** Draft. These are candidate results, not yet fully verified.

## Main Results

### 1. Boundary Regularity for the Homogeneous Infinite Laplace Equation

We consider the boundary regularity of viscosity solutions to the homogeneous infinite Laplace equation 

$$
\Delta_\infty u = 0
$$

on a domain $\Omega \subset \mathbb{R}^n$. While interior regularity for infinity harmonic functions is by now well understood, boundary behavior is substantially more subtle because the equation does not admit a standard weak formulation and boundary differentiability must be approached through comparison and cone-type arguments. The candidate proof addresses boundary regularity under natural geometric assumptions on $\Omega$ and the boundary data.

**Key features:**

- Boundary regularity is established for viscosity solutions of $\Delta_\infty u = 0$.
- The argument accounts for the degeneracy of the operator near the boundary.
- The result complements the known interior theory for infinity harmonic functions.

### 2. Boundary Regularity for the Inhomogeneous Infinite Laplace Equation

We extend the boundary regularity analysis to the inhomogeneous equation 

$$
\Delta_\infty u = f
$$

with a prescribed right-hand side $f$. The inhomogeneous term modifies the comparison and compactness arguments substantially, and the boundary behavior of solutions depends on the regularity and growth of $f$ near $\partial \Omega$. The candidate proof develops boundary estimates adapted to the presence of $f$.

**Key features:**

- Boundary regularity is treated for the inhomogeneous problem $\Delta_\infty u = f$.
- The proof handles the interaction between the source term and the degeneracy of the operator.
- The result is consistent with the homogeneous case in the limit $f \to 0$.

### 3. Interior Regularity for the Inhomogeneous Infinite Laplace Equation

We also study the interior regularity of viscosity solutions to $\Delta_\infty u = f$. The inhomogeneous term introduces new difficulties even in the interior, because the equation is no longer purely a comparison problem and the regularity of $u$ is tied to the regularity of $f$. The candidate proof establishes interior estimates under appropriate assumptions on $f$.

**Key features:**

- Interior regularity is proved for the inhomogeneous infinite Laplace equation.
- The proof incorporates the source term into the viscosity solution framework.
- Together with the boundary results, this provides a regularity picture for both the homogeneous and inhomogeneous problems.

### 4. Sharp Quartic Modica-Type Result for the Infinite Laplacian

We investigate a Modica-type sharp quartic estimate in the setting of the infinite Laplacian. Modica-type results are classical in the theory of phase transitions and gradient bounds; their analogues for the infinite Laplacian require a careful treatment of the degeneracy and of the $L^\infty$ variational structure. The candidate proof establishes a sharp quartic bound adapted to the infinite Laplacian.

**Key features:**

- A sharp quartic Modica-type estimate is obtained for the infinite Laplacian.
- The proof exploits the variational characterization of $\Delta_\infty$ and the AMLE structure.
- The result provides a degenerate-operator counterpart of classical Modica-type bounds.

## Proof Approach

The candidate proofs rely on the viscosity solution framework, which is the natural setting for the infinite Laplace equation, together with comparison principles and cone-type arguments[reference:2]. The main ingredients are:

1. **Viscosity formulation** – All results are stated and proved within the viscosity solution framework, which accommodates the degeneracy of $\Delta_\infty$.
2. **Comparison with cones** – Boundary and interior regularity are approached through comparison principles with cone functions, a standard tool in the theory of infinity harmonic functions[reference:3].
3. **Localization and scaling** – Boundary estimates are obtained by localization near $\partial \Omega$ and scaling arguments that respect the homogeneity of the operator.
4. **Sharp quartic analysis** – The Modica-type result combines the variational structure of the infinite Laplacian with a quartic estimate, requiring careful tracking of constants to ensure sharpness.

For the homogeneous problem, the absence of a source term allows comparison arguments to be pushed further; for the inhomogeneous problems, the source term is incorporated into the comparison and compactness steps. The sharp quartic result draws on the connection between the infinite Laplacian and $L^\infty$ variational problems.

## Repository Contents

| File | Description |
|---|---|
| [`infinity_homogeneous_boundary_regularity.pdf`](https://github.com/mingfeng87/Infinite-Laplace-equation/blob/main/infinity_homogeneous_boundary_regularity.pdf) | Candidate proof of boundary regularity for the homogeneous infinite Laplace equation $\Delta_\infty u = 0$. |
| [`infinity_inhomogeneous_boundary_regularity.pdf`](https://github.com/mingfeng87/Infinite-Laplace-equation/blob/main/infinity_inhomogeneous_boundary_regularity.pdf) | Candidate proof of boundary regularity for the inhomogeneous infinite Laplace equation $\Delta_\infty u = f$. |
| [`infinity_inhomogeneous_interiori_regularity.pdf`](https://github.com/mingfeng87/Infinite-Laplace-equation/blob/main/infinity_inhomogeneous_interiori_regularity.pdf) | Candidate proof of interior regularity for the inhomogeneous infinite Laplace equation. |
| [`sharp_quartic_modica_infinity_laplacian.pdf`](https://github.com/mingfeng87/Infinite-Laplace-equation/blob/main/sharp_quartic_modica_infinity_laplacian.pdf) | Candidate proof of a sharp quartic Modica-type estimate for the infinite Laplacian. |

## Verification Status

All four documents are marked as **drafts**. The results were generated with AI assistance and are currently under verification by our team. We welcome independent scrutiny and feedback from the mathematical community. In particular, we invite readers to check the comparison arguments in the boundary regularity proofs, the treatment of the inhomogeneous term, and the sharpness of the quartic Modica bound.

## License

This project is provided for academic and research purposes. Please contact the repository owner for licensing details.

## Contact

For questions or collaboration inquiries, please open an issue on GitHub.
