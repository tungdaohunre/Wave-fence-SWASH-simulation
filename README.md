# Numerical models

Numerical models have been applied in many fields, and it is more important to apply them to solve the coastal hydraulic problem thank to the rapid development of computing technology. The numerical technique can be based on the finite element method, finite difference method , boundary element method, finite volume method and Eulerian-Lagrangian method. The time-stepping algorithm can be implicit, semi-implicit, explicit, or characteristic-based. The shape function can be of the first order, second order, or a higher order. The modelling can be simplified into different spatial dimensions, i.e., a one-dimensional (1D) model, two-dimensional (2D) depth-integrated model, 2D lateral-integrated model, 2D layered model and 3D model [(Coastal Wiki)](http://www.coastalwiki.org/wiki/Modelling_coastal_hydrodynamics).

1. SWASH

The [SWASH](https://swash.sourceforge.io/) (an acronym of Simulating WAves till SHore) is a non-hydrostatic wave-flow model and is intended to be used for predicting transformation of dispersive surface waves from offshore to the beach for studying the surf zone and swash zone dynamics, wave propagation and agitation in ports and harbours, rapidly varied shallow water flows typically found in coastal flooding resulting from e.g. dike breaks, tsunamis and flood waves, density driven flows in coastal waters, and large-scale ocean circulation, tides and storm surges. Many studies have applied this model to solve coastal problem, including the nearzone, sediment transport, and vegetation interaction. The related publication can be found [here](https://swash.sourceforge.io/references/references.htm).

The SWASH model have been applied in wave propagation to the shore and was validated in many studies, for example, wave attenuation and wave breaking processes in the swash-zone [(Smit, Zijlema, and Stelling, 2013)](https://www.sciencedirect.com/science/article/abs/pii/S0378383913000215?via%3Dihub). Furthermore, most of studies which consider wave reduction due to vegetation are also taken into account the SWASH model with the vegetation implementation as a good tools. 

The PhD thesis of [Phan, L.K. (2019)](https://research.tudelft.nl/en/publications/wave-attenuation-in-coastal-mangroves-mangrove-squeeze-in-the-mek), including a study of the effect of nonlinear wave reduction by vegetation, present an example of applying SWASH model. Moreover, [Cao 2016](https://bioone.org/journals/journal-of-coastal-research/volume-75/issue-sp1/SI75-167.1/Numerical-Modeling-of-Wave-Transformation-and-Runup-Reduction-by-Coastal/10.2112/SI75-167.1.short) studied wave transformation and run up reduction by coastal vegetation and especially the consideration of both horizontal and vertical components of mangroves in SWASH model in study of [Suzuki et al. (2019)](https://www.sciencedirect.com/science/article/abs/pii/S0378383917304179?via%3Dihub) brings to the new explaination for wave attenuation inside an mangrove area. 

Eventually, [Dao et al., 2021](https://journals.open.tudelft.nl/jchs/article/view/5612) validated and calibrated the SWASH model using experimental data of wave damping due to wooden fence by applying the new vegetation implementation equation in [Suzuki et al. 2019](https://www.sciencedirect.com/science/article/pii/S0378383917304179).

The mentioned examples are proven the trust of using this model for further simulations, especially in the laboratory condition, even though it is even more confident if validating the model with the field measurement data. Thus, this model can be a good computational laboratory for studying purpose.

2. Alternative models

Moreover, [SWAN](https://swanmodel.sourceforge.io/) is a third-generation wave model, developed at Delft University of Technology, that computes random, short-crested wind-generated waves in coastal regions and inland waters. Many related publications that taken into account SWAN to solve ocean issues can be found [here](https://swanmodel.sourceforge.io/references/references.htm).

SWAN accounts for the following physics:
  * Wave propagation in time and space, shoaling, refraction due to current and depth, frequency shifting due to currents and non-stationary depth.
  * Wave generation by wind.
  * Three- and four-wave interactions.
  * Whitecapping, bottom friction and depth-induced breaking.
  * Dissipation due to aquatic vegetation, turbulent flow and viscous fluid mud.
  * Wave-induced set-up.
  * Propagation from laboratory up to global scales.
  * Transmission through and reflection (specular and diffuse) against obstacles.
  * Diffraction.

There are also many numerical models that can be suitable for simulating coastal hydralic problems, such as Sbeach, Xbeach, Duros Plus, Litpack, Genesis, Unibest-CL, Delft3D, Telemac, EFDC.

3. SWASH Exercises

Before practicing, it is recommendedn that users should read the User Manual and examples on the official website of SWASH. Also, the brief guideline for installation, interpretation of commnand files and bathymetry for 1D simulation can be found [here](https://colab.research.google.com/drive/1M7YrSOv6xSdRSPI2K2ttvPI689O7bMaU).

In this practice, users successfully run 1D test of wave propagation to the shore from the water depth of 10 m. The forshore slope is 1:10, uniform and rectangular. Still water level is 0.0 m. The wave conditions are regular with Hrms = 1.0 m, and T = 5.5 seconds.

The outputs are wave height at 8 m, 5 m, and 1 m water depth. And calculating wave heights, wavelengths, and wave periods at the same locations from elevation results.

The python scripts will be given in the Exercise 02 directory.
