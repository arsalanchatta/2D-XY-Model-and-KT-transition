# 2D-XY-Model-and-KT-transition
Simulating Kosterlitz-Thouless phase transition using 2D short-range Ising model
The purpose of this project was to simulate and observe the Kosterlitz-Thouless phase transition, which entailed observing a rapid change in the symmetry of the system while still adhering to the Mermin-Wagner theorem, which states that continuous symmetries cannot be spontaneously broken at finite temperature in systems with sufficiently short-range interactions in dimensions d ≤ 2.
Whereas, our system shows some sudden changes around a critical temperature despite having 2D short-range interaction; which means particles can only be effected by their neighbouring spins.
This change was studied by doing the data analysis of Temperature Dependence of Magnetization, Energy, Susceptibility and Specific Heat values of the different lattice systems.
While the data itself was randomly generated by applying Leapfrog integrator on the equations of motion and then applying the “Hamiltonian Monte Carlo algorithm” (HMC algorithm) to get the “markove chains” which contained the data values for Magnetization, Energy, Susceptibility and Specific Heat.
Then applied data fitting using these “markove chains” and the defined "Lorentzian" function given to “Model” class as “gmodel = Model(Lorentzian)”, imported from “lmfit” Python package. And then parametrizing using gmodel.make_params() and gmodel.fit(), which also provided Fit Statistics using result.fit_report() method. And then, at last, plotting all the data using “matplotlib.pyplot” functions.
For complete background theory, calculations and results open "Report.pdf".
It took around 5 days on my system to completely run this code.
