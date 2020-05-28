# PhysicalColors
A Mathematica package that provides better visible spectrum and blackbody radiation color.

This pacakge contains three functions:

**SpectrumExcitation**[*wvl*] which returns the linear XYZ excitation of light at wavelength *wvl*.
**SpectrumColor**[*wvl*] which returns XYZColor of light at wavelength *wvl*.
**TemperatureColor**[*temp*] which returns RGBColor of a blackbody at temperature *temp*.

The first two is directly imported from CIE 1931 standard.
The last is imported from [this place](http://www.vendian.org/mncharity/dir3/blackbody/), thanks a lot @Mitchell Charity!
