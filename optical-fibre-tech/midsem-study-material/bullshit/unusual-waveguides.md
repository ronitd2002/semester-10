Below is a consolidated list of the key equations you can use to solve numerical problems for various slab waveguide profiles. Each subsection gives the governing differential equations, the general solutions in the core (or graded‐region) and cladding (or outer regions), and the eigenvalue (dispersion) conditions you’d use to determine the propagation constant, mode number, or field distribution. All variables are labeled with their typical units.

──────────────────────────────
**1. 3‐Layer Symmetric Slab Waveguide**

*Structure:*  
A core of thickness $d$ and refractive index $n_1$ is sandwiched between two identical claddings with index $n_2$ (with $n_1 > n_2$). The coordinate $x$ is taken transverse to the propagation direction $z$.

**(a) In the Core $(|x|\le d/2)$:**  
The field (e.g. $\psi(x)$ representing a component of the electric or magnetic field) satisfies the Helmholtz equation  
$\frac{d^2 \psi}{dx^2} + \left(k_0^2 n_1^2 - \beta^2\right)\psi = 0,$
with general solution  
$\psi(x) = A \cos\left(k_x x\right) + B \sin\left(k_x x\right),$
where  
$k_x = \sqrt{k_0^2 n_1^2 - \beta^2}\quad \text{(rad/m)}.$

**(b) In the Cladding $(|x|> d/2)$:**  
The field decays exponentially:
$\frac{d^2 \psi}{dx^2} - \left(\beta^2 - k_0^2 n_2^2\right)\psi = 0,\quad \psi(x) = C\,e^{-\kappa|x|},$
with  
$\kappa = \sqrt{\beta^2 - k_0^2 n_2^2}\quad \text{(1/m)}.$

**(c) Eigenvalue (Dispersion) Equations:**  
By enforcing the continuity of $\psi(x)$ and its derivative at $x=\pm d/2$, the following conditions result:

- For **symmetric (even) modes:**
  $\tan\left(\frac{k_x d}{2}\right) = \frac{\kappa}{k_x}.$

- For **antisymmetric (odd) modes:**
  $\cot\left(\frac{k_x d}{2}\right) = -\frac{\kappa}{k_x}.$

*Variables & Units:*  
- $k_0 = \frac{2\pi}{\lambda_0}$ (rad/m), where $\lambda_0$ is the free-space wavelength (m).  
- $\beta$ is the propagation constant (1/m).  
- $d$ is the core thickness (m).

──────────────────────────────
**2. 3‐Layer Asymmetric Slab Waveguide**

*Structure:*  
The core (index $n_1$, thickness $d$) is bounded by two different claddings: the lower cladding with index $n_0$ and the upper cladding with index $n_2$ (with $n_1 > n_0,\, n_2$ and $n_0\ne n_2$).

**(a) In the Core $(|x|\le d/2)$:**  
Same as before,
$\frac{d^2 \psi}{dx^2} + \left(k_0^2 n_1^2 - \beta^2\right)\psi = 0,\quad \psi(x)=A\cos(k_x x)+B\sin(k_x x),$
with  
$k_x = \sqrt{k_0^2 n_1^2 - \beta^2}.$

**(b) In the Claddings:**

- For $x > d/2$ (upper cladding, index $n_2$):
  $\frac{d^2 \psi}{dx^2} - \left(\beta^2 - k_0^2 n_2^2\right)\psi = 0,\quad \psi(x)=C\,e^{-\kappa_2\,(x-d/2)},$
  where  
  $\kappa_2 = \sqrt{\beta^2 - k_0^2 n_2^2}.$

- For $x < -d/2$ (lower cladding, index $n_0$):
  $\frac{d^2 \psi}{dx^2} - \left(\beta^2 - k_0^2 n_0^2\right)\psi = 0,\quad \psi(x)=D\,e^{\kappa_0\,(x+d/2)},$
  with  
  $\kappa_0 = \sqrt{\beta^2 - k_0^2 n_0^2}.$

**(c) Eigenvalue Equation:**  
After applying the boundary conditions (continuity of $\psi$ and its derivative at $x=\pm d/2$), a commonly used form is
$k_x\,d + \tan^{-1}\!\left(\frac{k_x}{\kappa_0}\right) + \tan^{-1}\!\left(\frac{k_x}{\kappa_2}\right) = m\pi,\quad m=0,1,2,\ldots$
For TM modes, the phase shifts are modified by the ratios of refractive indices (i.e., factors of $n_1^2/n_0^2$ and $n_1^2/n_2^2$) in the inverse tangent terms.

*Variables & Units:*  
- $n_0,\,n_1,\,n_2$ are unitless refractive indices.  
- Other symbols as defined in the symmetric case.

──────────────────────────────
**3. Parabolic Slab Waveguide**

*Structure:*  
A graded-index waveguide where the refractive index varies parabolically across the transverse direction. A typical profile is
$n(x)^2 = n_0^2\left(1 - 2\Delta\,\frac{x^2}{d^2}\right),$
or equivalently,  
$n(x) = n_0\left[1 - \Delta\,\frac{x^2}{d^2}\right],$
for $|x|$ within the guiding region. Here, $\Delta$ is a small positive parameter (unitless) and $d$ characterizes the width.

**(a) Wave Equation:**  
The scalar wave equation becomes
$\frac{d^2 \psi}{dx^2} + \left[k_0^2 n_0^2\left(1 - 2\Delta\,\frac{x^2}{d^2}\right) - \beta^2\right]\psi = 0.$
By a suitable change of variable (e.g., $\xi = x/x_0$, with $x_0$ determined by the curvature), this can be transformed into the standard harmonic oscillator (Hermite) differential equation:
$\frac{d^2 \psi}{d\xi^2} + \left(\lambda - \xi^2\right)\psi = 0.$

**(b) Eigenvalue Relation:**  
The quantization condition is  
$\lambda = 2m+1,\quad m=0,1,2,\ldots,$
which leads to an expression for the propagation constant such as
$\beta_m \approx k_0 n_0 \left[1 - \frac{(2m+1)}{2}\left(\frac{1}{k_0 n_0}\sqrt{\frac{2\Delta}{d^2}}\right)\right],$
or, equivalently,
$\beta_m = k_0 n_0 - \left(m+\frac{1}{2}\right)\Delta\beta,$
where $\Delta\beta$ (in 1/m) is determined by the index curvature.

*Variables & Units:*  
- $n_0$ is the peak refractive index (unitless).  
- $k_0 = \frac{2\pi}{\lambda_0}$ (rad/m).  
- $\Delta$ is unitless; $d$ (m) sets the scale of the index variation.  
- $m$ is the mode number (integer).

──────────────────────────────
**4. Triangular Slab Waveguide**

*Structure:*  
A waveguide with a linearly varying refractive index, often modeled as
$n(x) = n_0 - \gamma\,|x|,$
where $\gamma$ (in units of m$^{-1}$) is the gradient. This profile creates a “triangular” potential for the optical field.

**(a) Wave Equation:**  
The scalar wave equation is
$\frac{d^2 \psi}{dx^2} + \left[k_0^2\left(n_0 - \gamma\,|x|\right)^2 - \beta^2\right]\psi = 0.$
For appropriate scaling, this equation can be recast into the form of the Airy differential equation.

**(b) Airy Function Solution and Eigenvalue Condition:**  
The general solution is expressed in terms of Airy functions, $\mathrm{Ai}(x)$ and $\mathrm{Bi}(x)$. Imposing the decaying (bound) condition (typically eliminating $\mathrm{Bi}$) and applying boundary conditions yields an eigenvalue relation of the form
$\mathrm{Ai}(-\zeta_m)=0,$
with the propagation constant given by
$\beta_m = k_0 n_0 - \left(\frac{k_0^2 \gamma}{2}\right)^{1/3}\zeta_m.$
Here, $\zeta_m$ is the $m$-th zero of the Airy function $\mathrm{Ai}(x)$ (with $\zeta_0 \approx 2.3381$, $\zeta_1 \approx 4.0879$, etc.).

*Variables & Units:*  
- $n_0$ is the maximum refractive index (unitless).  
- $\gamma$ (1/m) is the index gradient.  
- $k_0 = \frac{2\pi}{\lambda_0}$ (rad/m).  
- $\beta_m$ is the propagation constant (1/m).  
- $\zeta_m$ are dimensionless constants (zeros of Ai).

──────────────────────────────
**Summary**

For each profile the strategy is similar:
- **Write down the appropriate wave equation** using the local index profile $n(x)$.  
- **Solve for the field distribution** (oscillatory in the guiding region; exponential/Airy in the cladding or turning regions).  
- **Apply continuity (or boundary) conditions** to obtain the eigenvalue (dispersion) equation that quantizes the allowed modes.