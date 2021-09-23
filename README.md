# DiffCS_strange

This V 1.0.0 version of the newest differential cross section calculator for exclusive single kaon electroproduction allows you to evaluate the differential cross section value for the large invariants' scales and any <a href="https://www.codecogs.com/eqnedit.php?latex=\cos{\theta}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\cos{\theta}" title="\cos{\theta}" /></a> values. Relatively fast and effective procedures make this program a convenient and reliable choice for data analysis in particle physics.

### Formalism 
The differential cross section of the kaons electroproduction off proton in the one-photon approximation:

<a href="https://www.codecogs.com/eqnedit.php?latex=\dfrac{d\sigma}{dE_fd\Omega_{e}d\Omega}&space;=&space;\Gamma&space;\dfrac{d\sigma}{d\Omega}_{\gamma^*}&space;\;\;\;\;\;\;\;\;&space;\Gamma&space;=&space;\dfrac{\alpha}{2\pi^2Q^2}\dfrac{(W^2&space;-&space;m^2)E_f}{2mE_i}\dfrac{1}{1&space;-&space;\epsilon}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\dfrac{d\sigma}{dE_fd\Omega_{e}d\Omega}&space;=&space;\Gamma&space;\dfrac{d\sigma}{d\Omega}_{\gamma^*}&space;\;\;\;\;\;\;\;\;&space;\Gamma&space;=&space;\dfrac{\alpha}{2\pi^2Q^2}\dfrac{(W^2&space;-&space;m^2)E_f}{2mE_i}\dfrac{1}{1&space;-&space;\epsilon}" title="\dfrac{d\sigma}{dE_fd\Omega_{e}d\Omega} = \Gamma \dfrac{d\sigma}{d\Omega}_{\gamma^*} \;\;\;\;\;\;\;\; \Gamma = \dfrac{\alpha}{2\pi^2Q^2}\dfrac{(W^2 - m^2)E_f}{2mE_i}\dfrac{1}{1 - \epsilon}" /></a>

<a href="https://www.codecogs.com/eqnedit.php?latex=\dfrac{d\sigma}{d\Omega}_{\gamma^*}&space;=&space;\dfrac{d\sigma_T}{d\Omega}&space;&plus;&space;\varepsilon\dfrac{d\sigma_L}{d\Omega}&space;&plus;&space;\sqrt{\varepsilon(1&plus;\varepsilon)}\dfrac{d\sigma_{LT}}{d\Omega}\cos{\varphi}&space;&plus;&space;\varepsilon\dfrac{d\sigma_{TT}}{d\Omega}\cos{2\varphi}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\dfrac{d\sigma}{d\Omega}_{\gamma^*}&space;=&space;\dfrac{d\sigma_T}{d\Omega}&space;&plus;&space;\varepsilon\dfrac{d\sigma_L}{d\Omega}&space;&plus;&space;\sqrt{\varepsilon(1&plus;\varepsilon)}\dfrac{d\sigma_{LT}}{d\Omega}\cos{\varphi}&space;&plus;&space;\varepsilon\dfrac{d\sigma_{TT}}{d\Omega}\cos{2\varphi}" title="\dfrac{d\sigma}{d\Omega}_{\gamma^*} = \dfrac{d\sigma_T}{d\Omega} + \varepsilon\dfrac{d\sigma_L}{d\Omega} + \sqrt{\varepsilon(1+\varepsilon)}\dfrac{d\sigma_{LT}}{d\Omega}\cos{\varphi} + \varepsilon\dfrac{d\sigma_{TT}}{d\Omega}\cos{2\varphi}" /></a>

## Usage
1. Install [Root Cern](https://root.cern.ch/building-root)
2. Git the program: git clone https://github.com/Maksaska/Diff_cros_strange.git
3. Type command: chmod +x Run
4. Compile with "Run",i.e. ./Run
5. Start the compiled file with ./start

Requirements: [Root Cern](https://root.cern/)

## Options for program start:
* The energy of the incident electron:
You should add "-e X", where X in GeV, to the "./start" command to specify the beam energy.
* The program is written for two channels. The default is <a href="https://www.codecogs.com/eqnedit.php?latex=K\Lambda" target="_blank"><img src="https://latex.codecogs.com/gif.latex?K\Lambda" title="K\Lambda" /></a>. That is if you don't take any additional action.
To work with <a href="https://www.codecogs.com/eqnedit.php?latex=K\Sigma^0" target="_blank"><img src="https://latex.codecogs.com/gif.latex?K\Sigma^0" title="K\Sigma^0" /></a> channel, you should add "--KSigma0" to "./start" command like "./start --KSigma0"

* 2 modes of operation are initialized in the program:
  * Cross section calculation at the given point <a href="https://www.codecogs.com/eqnedit.php?latex=(W,&space;Q^2,&space;\cos{\theta},&space;\varphi)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?(W,&space;Q^2,&space;\cos{\theta},&space;\varphi)" title="(W, Q^2, \cos{\theta}, \varphi)" /></a>
  * Average cross section calculation for a given area of <a href="https://www.codecogs.com/eqnedit.php?latex=W" target="_blank"><img src="https://latex.codecogs.com/gif.latex?W" title="W" /></a>, <a href="https://www.codecogs.com/eqnedit.php?latex=Q^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?Q^2" title="Q^2" /></a>, and <a href="https://www.codecogs.com/eqnedit.php?latex=\cos{\theta}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\cos{\theta}" title="\cos{\theta}" /></a>. As we are fitting the data along the <a href="https://www.codecogs.com/eqnedit.php?latex=\cos{\theta}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\cos{\theta}" title="\cos{\theta}" /></a> axis, you can use any value from [-1, 1]. 

Below you can find 2 graphs with an accessible area of <a href="https://www.codecogs.com/eqnedit.php?latex=(W,&space;Q^2)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?(W,&space;Q^2)" title="(W, Q^2)" /></a> for each channel.
Each mode needs its own input. In the first case, it's <a href="https://www.codecogs.com/eqnedit.php?latex=W" target="_blank"><img src="https://latex.codecogs.com/gif.latex?W" title="W" /></a>, <a href="https://www.codecogs.com/eqnedit.php?latex=Q^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?Q^2" title="Q^2" /></a>, <a href="https://www.codecogs.com/eqnedit.php?latex=\cos{\theta}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\cos{\theta}" title="\cos{\theta}" /></a>, and <a href="https://www.codecogs.com/eqnedit.php?latex=\varphi" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\varphi" title="\varphi" /></a>(in degrees) variable values, in the second - intervals for <a href="https://www.codecogs.com/eqnedit.php?latex=W" target="_blank"><img src="https://latex.codecogs.com/gif.latex?W" title="W" /></a>, <a href="https://www.codecogs.com/eqnedit.php?latex=Q^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?Q^2" title="Q^2" /></a>, and <a href="https://www.codecogs.com/eqnedit.php?latex=\cos{\theta}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\cos{\theta}" title="\cos{\theta}" /></a> variables. When working with one of the modes, you don't need to add input variable values for the other.

## Point-like calculation
(It's the default mode for the program) To work with this mode, when starting the program, you need to add the following:
* --W=X, where X is an invariant mass of the final hadron system in <a href="https://www.codecogs.com/eqnedit.php?latex=GeV" target="_blank"><img src="https://latex.codecogs.com/gif.latex?GeV" title="GeV" /></a>
* --Q2=X, where X is photon virtuality in <a href="https://www.codecogs.com/eqnedit.php?latex=GeV^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?GeV^2" title="GeV^2" /></a>
* --cos=X, where X is the cosine value of the kaon polar angle in c.m. frame
* --phi=X, where X is the value of the kaon azimuth angle in c.m. frame

The default values of these variables are zero, so you always need to specify the point you want.
 
> An example: ./start -e 6.5 --W=1.8 --Q2=0.9 --cos=0.1 --phi=180
> 
> Meaning: <a href="https://www.codecogs.com/eqnedit.php?latex=K\Lambda" target="_blank"><img src="https://latex.codecogs.com/gif.latex?K\Lambda" title="K\Lambda" /></a> channel, point-like cross section calculation, <a href="https://www.codecogs.com/eqnedit.php?latex=E_{beam}&space;=&space;6.5\;\text{GeV},\;W&space;=&space;1.8\;\text{GeV},\;Q^2&space;=&space;0.9\;\text{GeV$^2$},\;\cos{\theta}=0.1,\;\varphi&space;=&space;180^{\degree}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?E_{beam}&space;=&space;6.5\;\text{GeV},\;W&space;=&space;1.8\;\text{GeV},\;Q^2&space;=&space;0.9\;\text{GeV$^2$},\;\cos{\theta}=0.1,\;\varphi&space;=&space;180^{\degree}" title="E_{beam} = 6.5\;\text{GeV},\;W = 1.8\;\text{GeV},\;Q^2 = 0.9\;\text{GeV$^2$},\;\cos{\theta}=0.1,\;\varphi = 180^{\degree}" /></a>

## Average calculation
To work with averaging, you need to add the following:
* --average

For this mode of operation, the program requires the boundaries values of the <a href="https://www.codecogs.com/eqnedit.php?latex=W,\;Q^2,\;\cos{\theta}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?W,\;Q^2,\;\cos{\theta}" title="W,\;Q^2,\;\cos{\theta}" /></a> intervals. They are all zero by default.
* --W_min=X
* --W_max=X
* --Q2_min=X
* --Q2_max=X
* --cos_min=X
* --cos_max=X

> An example: ./start -e 6.5 --average --W_min=1.75 --W_max=1.95 --Q2_min=0.65 --Q2_max=0.7 --cos_min=-1 --cos_max=1 --KSigma0
> 
> Meaning: <a href="https://www.codecogs.com/eqnedit.php?latex=K\Sigma^0" target="_blank"><img src="https://latex.codecogs.com/gif.latex?K\Sigma^0" title="K\Sigma^0" /></a> channel, average cross section calculation, <a href="https://www.codecogs.com/eqnedit.php?latex=E&space;=&space;6.5\;\text{GeV},\;W\in[1.75,1.95]\;\text{GeV},Q^2&space;\in&space;[0.65,0.7]\;\text{GeV$^2$},\cos{\theta}&space;\in&space;[-1,1]" target="_blank"><img src="https://latex.codecogs.com/gif.latex?E&space;=&space;6.5\;\text{GeV},\;W\in[1.75,1.95]\;\text{GeV},Q^2&space;\in&space;[0.65,0.7]\;\text{GeV$^2$},\cos{\theta}&space;\in&space;[-1,1]" title="E = 6.5\;\text{GeV},\;W\in[1.75,1.95]\;\text{GeV},Q^2 \in [0.65,0.7]\;\text{GeV$^2$},\cos{\theta} \in [-1,1]" /></a>.

## Availables areas of (W, Q2) for each channel
<a href="https://www.codecogs.com/eqnedit.php?latex=K\Lambda" target="_blank"><img src="https://latex.codecogs.com/gif.latex?K\Lambda" title="K\Lambda" /></a>:
<img src="/pic/KL_int.jpg" alt="KL"/>
<a href="https://www.codecogs.com/eqnedit.php?latex=K\Sigma^0" target="_blank"><img src="https://latex.codecogs.com/gif.latex?K\Sigma^0" title="K\Sigma^0" /></a>:
<img src="/pic/KS_int.jpg" alt="KS"/>

<p align="left"> <img src="https://komarev.com/ghpvc/?username=maksaska&label=Profile%20views&color=0e75b6&style=flat" alt="maksaska" /> <img src="https://img.shields.io/badge/MSU-SINP-blue" /> <img src="https://img.shields.io/badge/JLab-red" /> </p>
