# PhysicalColors

A Mathematica package that provides better visible spectrum and blackbody radiation color.

## Requirements

Mathematica or free [Wolfram Engine](https://www.wolfram.com/engine/). Should be compatible for all modern versions (8.0+).

## Installation
Install with:

```Mathematica
PacletInstall["https://github.com/wjxway/PhysicalColors/releases/download/0.1.0/PhysicalColor-0.1.0.paclet"]
```

If you are using versions with paclet functionalities.

If you are using older versions, please download the **PhysicalColor.wl** file directly, rename it to **PhysicalColor.m**, open Mathematica and execute ```SystemOpen@FileNameJoin[{$UserBaseDirectory,"Applications"}]```, then create a folder named as PhysicalColor under this directory and drop the .m file inside.

## Functions

This pacakge contains four functions:

**SpectrumExcitation**[*wvl*] returns the linear XYZ excitation of light at wavelength *wvl*.

**SpectrumColor**[*wvl*] returns XYZColor of light at wavelength *wvl*.

**TemperatureColor**[*temp*] returns RGBColor of a blackbody at temperature *temp*.

**TemperatureIntensity**[*temp*] returns relative light intensity of a blackbody at temperature *temp*.

----
### MISC

Data for the first two functions are directly imported from CIE 1931 standard.

Data for the last two is imported from [this place](http://www.vendian.org/mncharity/dir3/blackbody/), which used CIE 1931 2 degree CMFs with Judd Vos corrections and D65 white point, thanks a lot @Mitchell Charity!

All data are interpolated based on physical rules so that they could accept data from 0 to Infinity.
