Below is a consolidated “cheat‐sheet” of the most important equations from your assignments. Each section is organized by waveguide type, with the equations written in LaTeX. Every variable is defined along with its unit (if applicable). You can use this as a ready reference for your test.

──────────────────────────────
**1. Optical Waveguides**

**(a) Wave Equation in an Inhomogeneous Dielectric:**  
$\nabla \times \left(\nabla \times \mathbf{H}\right) - \frac{n^2}{c^2}\frac{\partial^2 \mathbf{H}}{\partial t^2} = 0$

- $\mathbf{H}$ = magnetic field (A/m)$
- $n$) = refractive index (unitless)
- $c$ = speed of light in vacuum ($\mathrm{m/s}$)  
- $t$ = time (s)

**(b) TE Mode – Equation for $E_y$:**  
$\frac{d^2 E_y}{dx^2} + \left(k_0^2\, n^2 - \beta^2\right) E_y = 0$
- $E_y$ = $y$-component of the electric field (V/m)  
- $x$ = transverse coordinate (m)  
- $k_0 = \frac{2\pi}{\lambda_0}$ = free-space wavenumber (rad/m) with $\lambda_0$ the free-space wavelength (m)  
- $\beta$ = propagation constant (1/m)

**(c) TM Mode – Equation for $H_y$:**  
$\frac{d}{dx}\left(\frac{1}{n^2}\frac{dH_y}{dx}\right) + \left(k_0^2 - \frac{\beta^2}{n^2}\right) H_y = 0$
- $H_y$ = $y$-component of the magnetic field (A/m)

**(d) Transcendental Equations for a Symmetric Step‐Index Planar Waveguide:**  
Define:
$k_x = \sqrt{k_0^2\, n_1^2 - \beta^2}, \quad \kappa = \sqrt{\beta^2 - k_0^2\, n_2^2}$
Then, the modal conditions are:  
- **Symmetric (even) modes:**  
  $\tan\left(\frac{k_x\, d}{2}\right) = \frac{\kappa}{k_x}$
- **Anti-symmetric (odd) modes:**  
  $-\cot\left(\frac{k_x\, d}{2}\right) = \frac{\kappa}{k_x}$
- $d$ = core width (m)  
- $n_1$ = core refractive index (unitless)  
- $n_2$ = cladding refractive index (unitless)

**(e) V-Parameter (Normalized Frequency):**  
$V = k_0\, d\, \sqrt{n_1^2 - n_2^2}$
- $V$ is unitless

**(f) Polarization Beat Length and Circular Polarization Length:**  
$
L_B = \frac{2\pi}{\beta_{\mathrm{TE}} - \beta_{\mathrm{TM}}}, \quad L = \frac{L_B}{4}
$
- $\beta_{\mathrm{TE}}$ and $\beta_{\mathrm{TM}}$ = propagation constants for TE and TM modes (1/m)  
- $L_B$ and $L$ = lengths (m)

**(g) Helmholtz Equation in a Layer:**  
$\frac{d^2 \psi}{dx^2} + \left(k_0^2\, n^2 - \beta^2\right)\psi = 0$
- $\psi$ = relevant field component (V/m or A/m depending on context)

**(h) Power Flow for TM Modes (Asymmetric Waveguide):**  
$P = \frac{1}{2}\left[\frac{\kappa\, n_1^2 + \gamma\, n_2^2}{n_1^2}\right]\left(\frac{\omega\, \varepsilon\, A^2}{\beta}\right)$
- $P$ = power (W)  
- $\omega$ = angular frequency (rad/s)  
- $\varepsilon$ = permittivity (F/m)  
- $A$ = field amplitude (unit depends on normalization)  
- $\gamma$ = decay constant in the cladding region (1/m)

──────────────────────────────
**2. Parallel-Plate Waveguides**

**(a) TE Mode – Cutoff Frequency:**  
$f_c = \frac{m\, c}{2\, d}$
- $f_c$ = cutoff frequency (Hz)  
- $m$ = mode index (integer, $m\ge1$)  
- $c$ = speed of light in vacuum ($\mathrm{m/s}$)  
- $d$ = plate separation (m)

**(b) Propagation Constant:**  
$\beta = \sqrt{k^2 - \left(\frac{m\pi}{d}\right)^2}$
- $k = \frac{\omega}{c}$ = free-space wavenumber (1/m)  
- $\omega$ = angular frequency (rad/s)

**(c) Phase Velocity:**  
$v_p = \frac{\omega}{\beta} = \frac{c}{\sqrt{1 - \left(\frac{f_c}{f}\right)^2}}$
- $v_p$ = phase velocity (m/s)  
- $f$ = operating frequency (Hz)

**(d) Wave Impedance:**  
For TE modes:  
$Z_{\mathrm{TE}} = \frac{\omega\, \mu}{\beta}$
For TM modes:  
$Z_{\mathrm{TM}} = \frac{\beta}{\omega\, \varepsilon}$
- $\mu$ = permeability (H/m)  
- $\varepsilon$ = permittivity (F/m)

──────────────────────────────
**3. Metallic (Rectangular) Waveguides**

**(a) TE$_{10}$ Mode – Cutoff Frequency:**  
$f_c = \frac{c}{2\, a}$
- $a$ = broad dimension (width) of the waveguide (m)

**(b) Cutoff Wavelength:**  
$\lambda_c = 2\, a$
- $\lambda_c$ = cutoff wavelength (m)

**(c) Propagation Constant:**  
$\beta = \sqrt{k^2 - \left(\frac{\pi}{a}\right)^2}$
- $k = \frac{\omega}{c}$ = free-space wavenumber (1/m)

**(d) Field Distribution for the TE$_{10}$ Mode:**  

*Magnetic Field:*  
$H_y(x,z) = H_0 \cos\left(\frac{\pi x}{a}\right) e^{-j\beta z}$

*Electric Field:*  
$E_x(x,z) = -j \frac{\beta \pi}{\omega\, \varepsilon\, a} \sin\left(\frac{\pi x}{a}\right) e^{-j\beta z}$
- $H_0$ = amplitude of the magnetic field (A/m)  
- $x$ = transverse coordinate (m)  
- $z$ = propagation direction (m)  
- $j = \sqrt{-1}$ is the imaginary unit

**(e) General Cutoff Condition for TE$_{mn}$ or TM$_{mn}$ Modes:**  
$k_c^2 = \left(\frac{m\pi}{a}\right)^2 + \left(\frac{n\pi}{b}\right)^2$
- $m,\, n$ = mode indices (integers)  
- $a,\, b$ = waveguide dimensions (m)

**(f) Phase and Group Velocities:**  

*Phase Velocity:*  
$v_p = \frac{\omega}{\beta} = \frac{c}{\sqrt{1 - \left(\frac{\lambda}{\lambda_c}\right)^2}}$

*Group Velocity:*  
$v_g = c\, \sqrt{1 - \left(\frac{\lambda}{\lambda_c}\right)^2}$
- $\lambda$ = operating wavelength (m)

**(g) Power Flow (Poynting Vector):**

$P = \frac{1}{2} \Re \left\{ \int_S \left(\mathbf{E} \times \mathbf{H}^*\right) \cdot \hat{z}\, dS \right\}$
- $P$ = power (W)  
- $\mathbf{E}$ = electric field (V/m)  
- $\mathbf{H}$ = magnetic field (A/m)  
- $S$ = cross-sectional area (m$^2$)  
- $\hat{z}$ = unit vector in the propagation (z) direction  
- $\Re\{\cdot\}$ denotes the real part, and $*$ is the complex conjugate

---