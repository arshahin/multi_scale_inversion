# multi_scale_inversion

A MATLAB package for multi-scale and multi-physics VFSA optimization customized for the inversion of core, log, and seismic data. 

I will place the codes in this repo soon. For now, enjoy reading the follwoing paper. The PDF is provided too.  

Shahin, A., Myers, M.T., Stoffa, P.L., Hathon, L.A., 2021, Multi-scale inversion of subsurface data aimed at characterizing heterogeneous carbonate reservoirs, Journal of Seismic Exploration, Volume 30, Issue 4. [Link]


Inverting single-scale subsurface data have been adequately addressed in literature. Nevertheless, multi-scale inversion have not been broadly studied to fully
characterize heterogeneous carbonate reservoirs. To address multi-scale inversion for carbonates, our research deals with core plugs, well logs and seismic data in the
following three sequential stages:

• On the core scale, we make three independent porosity measurements (Archimedes, μCT, and NMR). Measuring electrical resistivity, P- & S-wave velocities on brine
saturated core plugs along with joint modeling of the same properties using staged differential effective medium (SDEM) theory, help us to fine tune the model parameters
through a global optimization algorithm. Core-calibrated multi-physics rock model provides micro- & macro-porosities which are consistent with NMR and μCT derived
porosities.

• Next, we extend the technique from core to well log scale and demonstrate it using constructed logs from a real carbonate formation. In this stage, we integrate mass balance equations to model bulk density and SDEM theory to model elastic and electrical resistivity of dual-porosity carbonates. We design a stochastic global algorithm to simultaneously invert petrophysical properties. By constructing a dual-porosity formation, we demonstrate that the proposed workflow recovers the petrophysical
properties.

Finally in the third stage, we propose an inversion algorithm in seismic scale to simultaneously retrieve P&S-wave velocities and density. Similar to core- & log-scale
stages, Very fast simulated annealing (VFSA) is the special global optimization algorithm employed to minimize objective function. The optimization algorithm is stochastic in nature and is enable to estimate uncertainty in model parameters. Unlike commercial software, no assumption is made on correlations between P&S-wave velocities and density. No smoothed background model is needed and only bounds on model parameters are necessary.
