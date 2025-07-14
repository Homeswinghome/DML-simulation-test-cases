# DML-simulation-test-cases
Test cases for DML simulation development

Here are files to test DML simulators.

For each test cases, 3 files are provided :
* XXXX.txt : case parameters (see below)
* EFR_XXXX.txt : SPL at 1m measured with REW
* Z_XXXX.txt : electrical impedance measured with REW

## Test cases

* Isotropic materials :
  * EPS : Expended Polystyrene
  * PMMA : Acrylic
* Orthotropic materials :
  * PWD5 : Poplar plywood (3 cases with various boundary conditions, exciter positions)

## Parameter file :

**note : plate dimensions LXMM, LYMM in mm, other in SI units**

* CASETITLE = short description
* BCOND = boundary conditions (S simply supported, C clamped, F free edge), North (top), West (left), South (bottom), East (right)
* LXMM = x axis (horizontal) plate dimension in mm (North and South edge)
* LYMM = y axis (vertical) plate dimension in mm (West and East edge)
* H = plate thickness in m
* EX = x axis Young Modulus in Pa
* EY = y axis Young Modulus in Pa
* GXY = shear modulus in Pa
* RHO = density in kg/m³
* NUX = x axis Poisson's ratio
* NUY = y axis Poisson's raitio
* ZETAMD = modal damping coefficient (=1/2Q, Q modal quality factor) 
* EXTMODEL = exciter model
* POSX = x axis exciter position (decimal value from 0 = full West to 1 = full East)
* POSY = y axis exciter position (decimal value from O = full North to 1 full South)
