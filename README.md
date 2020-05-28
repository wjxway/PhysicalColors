# PhysicalColors
A Mathematica package that provides better visible spectrum and blackbody radiation color.

This pacakge contains three functions:

**SpectrumExcitation**[*wvl*] which returns the linear XYZ excitation of light at wavelength *wvl*.

**SpectrumColor**[*wvl*] which returns XYZColor of light at wavelength *wvl*.

**TemperatureColor**[*temp*] which returns RGBColor of a blackbody at temperature *temp*.

**TemperatureIntensity**[*temp*] returns relative light intensity of a blackbody at temperature *temp*.

----

Data for the first two functions are directly imported from CIE 1931 standard.

Data for the last two is imported from [this place](http://www.vendian.org/mncharity/dir3/blackbody/), which used CIE 1931 2 degree CMFs with Judd Vos corrections, thanks a lot @Mitchell Charity!

All data are interpolated based on physical rules so that they could accept data from 0 to Infinity.
