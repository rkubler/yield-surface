# Changelog

## Unreleased

- Loading paths: each path chip is now a show/hide toggle for its curves (3D view, plane stress and compaction plots), with show all / hide all; the path to animate is chosen in a list next to Run path. The choice is remembered. In the full view, clicking a legend entry hides or shows that curve.
- Full view for every plot (⤢ button on the π-plane, plane-stress, meridian, Lode and compaction plots): a full-window viewer with wheel zoom (shift: x only, alt: y only), drag to pan, pinch on touch screens, typed axis ranges, equal scale, linear or log x for the compaction plots, a readout of the nearest data point, PNG export, an "Open in new window" button that opens the same viewer as a separate page, and (in the claude.ai view) "Save as page" to keep the plot as a standalone HTML file.
- Compaction plots: switch between a linear stress axis ‖σ‖ (default) and log ‖σ‖; the choice is remembered.
- Compaction plots: the compacity axis runs up to full density 1 with labels every 0.1, and the strain axis uses round tick steps. Fixed the compaction plot collapsing to zero height for SANISAND (five plot tiles on a wide screen).
- Parameters to identify shown in purple in every yield function, with their number on each model button and in a panel under the equations (meaning of each parameter, state variables listed apart), and an Overview per family listing the models, their typical uses and their parameters. For models with an internal variable (Modified Cam-Clay, GTN, the caps, SANISAND), the constants of the evolution law are counted too (e.g. Cam-Clay: M + λ, κ, e_N; GTN: σ₀, q₁, q₂ + f_N, ε_N, s_N, f_c, δ) and shown in purple in the evolution equations; the GTN nucleation rate A_N (Chu and Needleman, 1980) is written out.
- Lode dependence ρ(θ) plot for the 12 criteria that use J₃, a Lode-angle arc on the π-plane and a pointer probe giving θ and ρ.
- Yield functions shown in both forms where they exist: the classical form (principal stresses or invariants) first, then the Lode-angle form, for the 12 Lode-dependent criteria and von Mises.
- Tresca sub-page `tresca.html`, linked from the Tresca equations: the polynomial form in J₂ and J₃ (Lubliner, 1990), a 3D view of its six planes, the two triangular prisms and their hexagonal intersection, π-plane and plane-stress sections with a probe giving the three factors and F, and the condition 3J₂ ≤ σ₀² that keeps only Tresca.
- Meridian plot switch between ξ–ρ and p–q (mean stress p = I₁/3, von Mises stress q = √(3J₂)), with p–q as default for cap, porous and granular models, and a p–q note under Conventions.
- Hoek–Brown: definitions of σ′₁, σ′₃, σc, m and s, and the generalized 2002 form (m_b, s and a from GSI and D) with its reference.
- Classical σ₁σ₂σ₃ view tab for the 3D plot: σ₁ horizontal to the right, σ₂ vertical upward, σ₃ toward the viewer, in a parallel (cabinet oblique) projection.
- Meridian plot: values on the vertical axis (ρ or q, both meridians), and characteristic points with their values: radii at ξ = 0 on both meridians, apex and cap ends, uniaxial tensile and compressive strengths, written with the symbols of the yield function where a closed form exists.
- Ottosen: classical form in I₁, J₂ and J₃ without the Lode angle (cubic in λ, largest root), shown before the Lode-angle form.
- Taller 3D view (one third higher) and the introduction across the full page width.
- Phone layout: hidden tiles stay hidden and the I₁, J₂, J₃ chips show under the yield function.

## 1.6 (11 October 2026)

- New models: Cazacu–Barlat (2004) tension–compression asymmetry for HCP metals, and Bai–Wierzbicki (2008) pressure- and Lode-dependent metal plasticity for ductile fracture.
- Convexity warning for Cazacu–Barlat (|c| > 3√3/4) and Bai–Wierzbicki (Lode factors), shown under the description.
- GoatCounter visit statistics (rkubler.goatcounter.com), with an optional visit count after the credits.
- Introduction, author and version shown next to the title.
- Original paper reference under each model description.
- Dilatant loading paths: the compacity can now fall (loosening, void growth) for all cap, porous and granular models.
- Gurson (GTN): void growth in uniaxial and equibiaxial tension.
- One-screen dashboard layout on desktop, with larger 2D plots in the center.
- Clearer WebGL message, with a retry using lighter settings.
