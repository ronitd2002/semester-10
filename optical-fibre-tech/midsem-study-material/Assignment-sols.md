Below is a comprehensive “cheat‐sheet” of the key equations that appear across your assignments on optical, parallel‐plate, and metallic (rectangular) waveguides. (Note: Symbols are defined after each equation.) Use this list as a reference to ensure you cover every important relation on your test.

──────────────────────────────
1. Optical Waveguides

• **(a) Wave Equation in an Inhomogeneous Dielectric:**  
    
    ∇×(∇×𝐇) – (n²/c²) ∂²𝐇/∂t² = 0  
    
  **Symbols:**  
  • 𝐇 = magnetic field vector  
  • n = spatially varying refractive index  
  • c = speed of light in vacuum  
  • t = time  

• **(b) TE Mode – Wave Equation for Eᵧ:**  
    
    d²Eᵧ/dx² + [k₀² n² – β²] Eᵧ = 0  
    
  **Symbols:**  
  • Eᵧ = y-component of the electric field  
  • x = transverse coordinate  
  • k₀ = 2π/λ₀ (free-space wavenumber; λ₀ = free-space wavelength)  
  • n = refractive index  
  • β = propagation constant  

• **(c) TM Mode – Wave Equation for Hᵧ:**  
    
    d/dx [ (1/n²) dHᵧ/dx ] + [k₀² – β²/n²] Hᵧ = 0  
    
  **Symbols:**  
  • Hᵧ = y-component of the magnetic field (for TM modes)  
  • Other symbols as defined above  

• **(d) Transcendental Equations for a Symmetric Step‐Index Planar Waveguide:**  
  Define:  
    kₓ = √(k₀² n₁² – β²)                       and   κ = √(β² – k₀² n₂²)  
  Then, for the modes in a core (index n₁, width d) with cladding index n₂:  
    – **Symmetric (even) modes:** tan(kₓ d/2) = κ/kₓ  
    – **Anti‐symmetric (odd) modes:** –cot(kₓ d/2) = κ/kₓ  
    
  **Symbols:**  
  • d = core width  
  • n₁ = core refractive index  
  • n₂ = cladding refractive index  

• **(e) V-Parameter (Normalized Frequency):**  
    
    V = k₀ d √(n₁² – n₂²)  
    
  **Symbols:** As above.

• **(f) Polarization Beat Length and Circular Polarization Length:**  
    
    L_B = 2π/(β_TE – β_TM)                     and  L = L_B/4  
    
  **Symbols:**  
  • β_TE, β_TM = propagation constants for the TE and TM modes, respectively  

• **(g) Helmholtz Equation in a Given Layer:**  
    
    d²ψ/dx² + [k₀² n² – β²] ψ = 0  
    
  **Symbols:**  
  • ψ = any relevant field component (e.g. Eᵧ or Hᵧ) in a layer of uniform n

• **(h) Power Flow for TM Modes (Asymmetric Waveguide):**  
  A derived expression (from the TM field profiles and Poynting’s theorem) is  
    
    P = ½ [ (κ n₁² + γ n₂²)/n₁² ] · (ω ε A²/β)  
    
  **Symbols:**  
  • P = power carried by the mode  
  • ω = angular frequency  
  • ε = permittivity of the medium  
  • A = field amplitude  
  • γ = decay constant in the (other) cladding region (if asymmetric)  
  • (Other symbols as defined above)  

*(See Optical Fiber Technology assignment citeturn0file0 for details.)*

──────────────────────────────
2. Parallel-Plate Waveguides

• **(a) Cutoff Frequency for TE Modes:**  
    
    f_c = m c/(2d)  
    
  **Symbols:**  
  • f_c = cutoff frequency  
  • m = mode index (an integer, m ≥ 1)  
  • c = speed of light in vacuum  
  • d = separation between the plates

• **(b) Propagation Constant:**  
    
    β = √[k² – (mπ/d)²]                      
    
  **Symbols:**  
  • k = ω/c = free-space wavenumber  
  • ω = angular frequency

• **(c) Phase Velocity:**  
    
    v_p = ω/β = c/√[1 – (f_c/f)²]  
    
  **Symbols:**  
  • f = operating frequency

• **(d) Wave Impedance (for completeness):**  
  For TE modes: Z_TE = ωμ/β  
  For TM modes: Z_TM = β/(ωε)  
    
  **Symbols:**  
  • μ = permeability; ε = permittivity

*(Standard relations as covered in the Parallel Plate Waveguides assignment citeturn0file1.)*

──────────────────────────────
3. Metallic (Rectangular) Waveguides

• **(a) Cutoff Frequency for the Dominant TE₁₀ Mode:**  
    
    f_c = c/(2a)                      
    
  **Symbols:**  
  • a = broad dimension (width) of the rectangular waveguide

• **(b) Cutoff Wavelength:**  
    
    λ_c = 2a

• **(c) Propagation Constant:**  
    
    β = √[k² – (π/a)²]  
    
  **Symbols:**  
  • k = ω/c, as defined earlier

• **(d) Field Distribution for the TE₁₀ Mode:**  
  Magnetic Field (dominant component):  
    H_y = H₀ cos(πx/a) e^(–jβz)  
  Electric Field (primary component):  
    E_x = –j (βπ/(ωε a)) sin(πx/a) e^(–jβz)  
    
  **Symbols:**  
  • H₀ = amplitude of the magnetic field  
  • x = coordinate across the broad dimension  
  • z = propagation direction

• **(e) General Cutoff Condition for TEₘₙ or TMₘₙ Modes:**  
    
    k_c² = (mπ/a)² + (nπ/b)²  
    
  **Symbols:**  
  • m, n = mode indices (integers)  
  • a, b = the broad and narrow dimensions of the waveguide

• **(f) Phase and Group Velocities:**  
  Phase Velocity: v_p = ω/β = c/√[1 – (λ/λ_c)²]  
  Group Velocity: v_g = c √[1 – (λ/λ_c)²]  
    
  **Symbols:**  
  • λ = operating wavelength

• **(g) Power Flow (via the Poynting Vector):**  
    
    P = ½ Re{ ∫_S (𝐄 × 𝐇* )·ẑ dS }  
    
  **Symbols:**  
  • 𝐄 = electric field, 𝐇 = magnetic field  
  • S = cross-sectional area  
  • ẑ = unit vector in the z (propagation) direction

*(These are the standard relations for rectangular (metallic) waveguides as reflected in the Metallic Waveguides assignment citeturn0file2.)*

──────────────────────────────
Use these equations as the backbone for your study—they are derived from Maxwell’s equations with appropriate boundary conditions and are central to solving problems in waveguide theory. Good luck acing your test!