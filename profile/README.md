Welcome! I am a graduate student at Stony Brook University studying cosmological tensions. I started this project in February 2022. This is the repository containing code for the work on my (currently unnamed) thesis.

# Introduction
The standard model of cosmology is $\Lambda$ 
cold dark matter (
$\Lambda$
CDM). In this theory, dark matter behaves as a a cosmological constant, which appears as 
$\Lambda$ in Einstein's equation. 
The *cold* property of dark matter means it is non-relativistic and dark meaning it is weakly coupled to the standard model of particle physics. 
$\Lambda$ CDM has a 6-dimensional parameterization as follows:
- $\Omega_b$, the ratio of baryon density to critical density.
- $\Omega_c$, the ratio of dark matter density to critical density.
- $H_0$, the Hubble constant.
- $\tau$, the optical depth at reionization
- $n_s$, the matter power spectrum spectral index
- $\log(A_s)$, the amplitude of matter fluctuations

This parameterization is not unique, however. These are the parameters which we sample in this project.

From these parameters there are two that are in notable tension. The most well-known is the Hubble tension. 
Experiments measuring $H_0$ from the 'early' universe using the cosmic microwave background (CMB) yield different results that experiments from the 'late' universe using weak lensing.

The tension in $H_0$ is about $4 \sigma$, large but not enough to claim new physics.

Another tension is for the parameter $S_8$.
Let $\Omega_m = \Omega_b+\Omega_c$ be the total matter density. 
From $\log(A_s)$ one can determine the root-mean-square of metter fluctions today from linear theory, 
denoted $\sigma_8$.
Define $S_8 = \sigma_8 (\Omega_m/0.3)^{0.5}$
$S_8$ is also in tension at about 2-3$\sigma$.

The goal of this project is to quantify tensions using the full 5 dimensional parameter space and the uncertainty in the tension. 
Tension metrics themselves are not error bars, they are estimators of the difference between two data sets. 
Because of experimental noise these estimators should have some intrinsic error.

Beyond just experiments, as long as one can create a fiducial cosmology for different cosmological theories one could do this analysis to check if a theory is compatible with the data.
We hope to extend the analysis here to include different extensions to $\Lambda$ CDM that are being studied by others in DES.

# Repositories
In each repository you can find more information about the code. Here I will give a breif description of what you can find in each of them.
- tension_calibration: Standardized implementation of tension metrics. Example notebooks for each metric and notebook with proof-of-concept of error bars.
- LSST_emulation: An emulator for LSST data vectors forked from LSST_y1_tutorial. Includes likelihoods and notebooks containing noise realization $\chi^2$, MCMC sampling, autocorrelation analysis, and analysis of number of samples on the normalizing flow.
- comsopower_emcee: An emulator of the CMB power spectrum forked from cosmopower to work with the emcee sampler. Includes autocorrelation analysis, sampling, and likelihoods.
- jupyter_notebooks: Instructional notebooks and personal testing notebooks.
- notes: Personal LaTeX notes on cosmology and computing.

