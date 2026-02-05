\# ΛCDM Cosmology — Numerical Expansion History of the Universe



This project numerically studies the expansion history of the universe within the

framework of \*\*flat ΛCDM cosmology\*\* by solving the Friedmann equation and deriving

key cosmological observables.



The evolution of the scale factor, density parameters, and the deceleration

parameter are computed and analyzed from the early radiation-dominated era

to the far future.



A) Physical Model



We consider a spatially flat universe with radiation, matter, and a cosmological

constant (Λ). The Friedmann equation is



(d a / d t) / a = H(a)



with



H(a) = H₀ √( Ωᵣ a⁻⁴ + Ωₘ a⁻³ + Ω\_Λ )



where:

\- Ωᵣ : radiation density parameter  

\- Ωₘ : matter density parameter  

\- Ω\_Λ : dark energy density parameter  



Planck-2018–like cosmological parameters are used.



---



B) Numerical Method



Instead of directly integrating `a(t)` as a stiff ODE, cosmic time is computed via

quadrature:



t(a) = ∫ da / (a H(a))



This approach is:

\- numerically stable across many decades in scale factor

\- physically transparent

\- standard in modern cosmology codes



The integration is performed on a logarithmic scale-factor grid using

cumulative trapezoidal integration.



C) Derived Quantities



From the numerical solution, the following quantities are computed:



\- Scale factor a(t)

\- Redshift z = 1/a − 1

\- Time-dependent density parameters Ωᵣ(t), Ωₘ(t), Ω\_Λ(t)

\- Deceleration parameter



q(t) = ½ Ωₘ(t) + Ωᵣ(t) − Ω\_Λ(t)



Key cosmological epochs are identified numerically:

\- Matter–radiation equality

\- Onset of accelerated expansion (q = 0)

\- Dark-energy domination (Ω\_Λ > Ωₘ)



The cosmic time is normalized so that a = 1 corresponds to an age of 13.8 Gyr.



D) Results



The simulation reproduces all standard ΛCDM features:



\- Radiation-dominated expansion at early times

\- Matter-dominated era with decelerated expansion

\- Transition to accelerated expansion at z ≈ 0.6–0.8

\- Dark-energy domination at late times



The deceleration parameter correctly changes sign, indicating the onset of

cosmic acceleration.



F)Tools \& Libraries



\- Python  

\- NumPy  

\- SciPy  

\- Matplotlib  



\## Author ##---



Nishant Thakur



