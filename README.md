# PRNF
Code for Paper "A PSEUDO-REVERSIBLE NORMALIZING FLOW FOR
STOCHASTIC DYNAMICAL SYSTEMS WITH VARIOUS INITIAL
DISTRIBUTIONS"   
https://arxiv.org/pdf/2306.05580.pdf


Example 5.1 Verification of algorithm accuracy: "Ex1bmt05.zip"
  Training part: "nf_BM1D_train.py", where variable "C_rev" is tuning hyperparameter \lambda in Section 3.3 of Paper.
  Evaluation part: "eval_initial.py" where the four initial different samples are generated by the inverse CDF method in 
  "inverse_cdf.py".
  Corss emtropy is plotted by "plot_entropy.py"
  KL-divergence is computed by "nf_BM1D_KL.py" and plotted by "plot_kl.py" 
  

Example 5.2 Generation of runaway electrons in magnetically confined nuclear fusion plasmas: "RE2D_thermal.zip"
    Runaway electrons initial and terminal positions (SDE) are generated by "RE2D_datagenerate.py".
    Training part: "nf_RE2D.py"
    Evaluation part (for different Maxwellian distribution): "eval_valid.py". Plotted by "plot_evalValid.py".
    Production Rate is plotted by "plot_physics.py".
    
    

Example 5.3 Passive scalar advection-diffusion transport in a 3D chaotic flow: "FF3D.zip"
    Fluid partiles initial and terminal positions (SDE) are generated by "FF3D_datagenerate.py"
    Training part: "nf_FF3D.py"
    Initial conditions are generated by inverse CDF method: "inverse_cdf.py" & "inverse_cdf_grid (21*21 initial conditions).
    Evaluation part: eval_density.py
    Plots files: plot_density (PRNF method to plot Fig10) and plot)eval_Valid.py (Fig9).
