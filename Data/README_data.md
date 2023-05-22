# Data in support of “Correlations of Near-Infrared Spectra to Bulk Properties in Polyolefins, using Principal Component Analysis”

## Background

The data here is in support of a submitted manuscript:

> Bradley P. Sutliff, Shailja Goyal, Tyler B. Martin, Peter A. Beaucage,
> Debra J. Audus, and Sara V. Orski, "Correlations of Near-Infrared Spectra
> to Bulk Properties in Polyolefins, using Principal Component Analysis."
> *Macromolecular Rapid Communications* **NUM** (2023) PAGES. DOI: .

This submitted publication explores using machine learning to enhance the
characterization potential of near-visible infrared spectroscopy when applied
to polyolefin materials. It describes a methodology for correlating a NIR
spectra with physical properties such as crystallization, density, and short
chain branching of polyolefin species.

Data is provided both for reproducibility and to enable prototyping of the
concepts discussed in the submitted manuscript. A code repository is provided
at [nir_corr_po](https://github.com/usnistgov/nir_corr_po), which includes a
notebook illustrating the concepts within the submitted
manuscript. Reproduction of the figures from the submitted manuscript including
plotting of the data contained herein is also provided.

## Data descriptions

### Sample Information

The `SampleInformation.csv` file provides the original resin code from the
manufacturer (where appropriate), the source, the sample code used to identify
materials in this work, the major and minor polyolefin class as reported by the
source, the physical form/shape of the sample when tested, and additional notes
such as BigSMILES and alternative names.

This file is also used by the `nir-corr-po.ipynb` to generate a list of files
for the code to automatically read into the document and generate an Xarray
dataset.

### NIR

The `NIR` folder contains the spectroscopic information for the NIR
measurements, after background subtraction was automatically applied by the
instrument. They are labeled as `<SampleCode>_<Replicate>.csv` where each
sample was measured 6 times, with the sample being shaken between each
replicate measurement. Samples were characterized at wavelengths between
approximately $4000 \mathrm{cm}^{-1}$ and $12000 \mathrm{cm}^{-1}$,
and the intensity is given in terms of % reflectance.

### Additional Measurements

The `AdditionalMeasurements.csv` file provides a summary of the additional
characterizations that were performed on the materials and that can be used to
find correlations. Density was calculated using Archimedes principal and is
provided with the standard error of the mean, Crystallinity was determined
using the enthalpy of melting from differential scanning calorimetry, and all
other measurements we taken from a variety of sensors on a high-temperature
size exclusion chromatography instrument. For Crystallinity, a 10 °C/min
temperature ramp was used, and values were extracted from heating. References
of 293.6 J/g and 207.1 J/g are used for PE and PP, respectively. Where
possible, averaged (mean) values are provided along with the standard error of
the mean (SEM).

For other measurements not used in the submitted manuscript:

* Mw(IR) is the molecular weight as determined by an inline infrared (IR)
  spectrometer attached to the high-temperature size exclusion chromatography
  instrument.
* Dispersity(IR) is the molecular weight dispersity as determined by the inline
  IR.
* Mw(MALS) is the molecular weight as determined by an inline multi-angle light
  scattering (MALS) detector attached to the high-temperature size exclusion
  chromatography instrument.
* Dispersity(MALS) is the molecular weight as determined by MALS.
* Mw(Viscometer) is the molecular weight as determined by an inline a
  four-capillary differential viscometer attached to the high-temperature size
  exclusion chromatography instrument.
* Dispersity(MALS) is the molecular weight as determined by the inline
  viscometer.
* MHa is the calculated exponential power of the Mark-Houwink equation based on
  intrinsic viscosity.
* MHK is the calculated scaling factor of the Mark-Houwink equation based on
  intrinsic viscosity.
* LCBf_per_1000C is the long chain branch content as determined by MALS.

More details on how these measurement were obtained can be found in the
corresponding submitted paper:

> Bradley P. Sutliff, Shailja Goyal, Tyler B. Martin, Peter A. Beaucage,
> Debra J. Audus, and Sara V. Orski, "Correlations of Near-Infrared Spectra
> to Bulk Properties in Polyolefins, using Principal Component Analysis."
> *Macromolecular Rapid Communications* **NUM** (2023) PAGES. DOI: .

## Contact

Bradley P. Sutliff, PhD  
Materials Science and Engineering Division  
Material Measurement Laboratory  
National Institute of Standards and Technology  

Email: Bradley.Sutliff@nist.gov  
GithubID: @bpsut  
Staff website: <https://www.nist.gov/people/bradley-sutliff>  

## How to cite

If you use the code, please cite our submitted manuscript once
published:

> Bradley P. Sutliff, Shailja Goyal, Tyler B. Martin, Peter A. Beaucage,
> Debra J. Audus, and Sara V. Orski, "Correlations of Near-Infrared Spectra
> to Bulk Properties in Polyolefins, using Principal Component Analysis."
> *Macromolecular Rapid Communications* **NUM** (2023) PAGES. DOI: .

If you use the data, please cite:

> Sutliff, Bradley; Goyal, Shailja; Martin, Tyler; Beaucage, Peter;
> Audus, Debra; Orski, Sara. Correlations of Near-Infrared Spectra to
> Bulk Properties in Polyolefins, using Principal Component Analysis,
> National Institute of Standards and Technology (2023),
> <https://doi.org/10.18434/NUM> (Accessed YYYY-MM-DD)
