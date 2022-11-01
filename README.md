<h1 align="center">
  <br>
  <img src="https://github.com/danwrisar/KMSIMG_NHS_EmissionsCookbook/blob/main/Images/recipebook.png" alt="NHS Emission Recipe Book Logo" width="200">
  <br>
  The NHS Emission Quantification Recipe Book
  <br>

[![GitHub Release](https://img.shields.io/badge/Version-v1.0_22%2F23-blue)]()  
</h1>

<p align="center">
  <a href="#about">About</a> •
  <a href="#contents">Contents</a> •
  <a href="#get-involved">Get Involved</a> •
  <a href="#license">License</a> •
  <a href="#change-log">Change Log</a>
</p>

## About

The *NHS Emission Quantification Recipe Book* is transparent, collaborative and evidence-based approach to establishing a standardised means of calculating emissions associated with NHS Carbon Footprint and Carbon Footprint Plus themes set out by the [Greener NHS](https://www.england.nhs.uk/greenernhs/) in October 2020 (Figure 1). The NHS Emissions Quantification Recipe Book has been developed by Dr Dan Wright of the Sustainability Team at [Kent Community Health NHS Foundation Trust](https://www.kentcht.nhs.uk/) in collaboration with members of the Kent & Medway Sustainability Impacts and Methodologies Group (KMS-IMG).

Key to the methodologies specified is the recognition that NHS organisations are at different stages in their emissions quantification journey. To support this journey and provide an innovative means to report in a methodologically-transparent way, each theme provides three options for calculation:

* A *Reduced Calculation* (RC) is intended to be an approach to calculating a ballpark figure emission impact using data that should be easily accessible by someone stepping into an emissions reporting role.
* A *Standard Calculation* (SC) is intended to feature the minimum data that NHS organisations should be working towards sourcing and handling, for example, periodical energy consumption data.
* An *Optimal Calculation* (OC) is intended to feature 'best in class' approaches to calculating accurate emissions, this may include using advanced tooling or higher resolution data, for example, half-hourly energy consumption data.

By being transparent around which methodological approach has been used, either RC, SC or OC, this supports 'comparing apples to apples' both within and between [Integrated Care Systems](https://www.england.nhs.uk/integratedcare/what-is-integrated-care/). To demonstrate, here is a worked example for an RC approach to calculating emissions from natual gas use:

> Stu sources the Display Energy Certification (DEC) for the building they are interested in using the [energy certificate repository](https://www.gov.uk/find-energy-certificate). Using information from the Building Energy Use figure, Stu multiplies the annual energy use of *other fuels* (328) by the *total useful floor area* for the building (2778.54). The calculated annual total consumption (911,361.12) is presented in kWh. 
>
> By using the [BEIS Conversion Factors dataset for the year they are interested in (2019)](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2019), Stu is able to source a value for emissions per kWh of natural gas use assuming gross calorific value (0.18385kgCO<sub>2</sub>e/kWh). Stu wants to report in tonnes, therefore divides the sum by 1,000 and then rounds to two decimal places. Along with adding their units (tCO<sub>2</sub>e), Stu adds the [RC] tag to support transparency around how this figure was calculated. The final value added to Stu’s report on emissions associated with natural gas consumption is 167.55tCO<sub>2</sub>e [RC].
>
> *Equation 1.4* An example of an RC approach to calculating emissions associated with natural gas consumption.
>
> $$ 
> \frac{\left( 328 \times 2778.54 \right) \times 0.18385}
> {1000} = 167.55\text{tCO}_2\text{e} \text{ [RC]}
> $$

<p align="center">
    <img src="https://github.com/danwrisar/KMSIMG_NHS_EmissionsCookbook/blob/main/Images/NZR-Scopes.png" alt="Greener NHS Net Zero Scopes" width="500">
</p>

Fig 1. A summary of the themes considered to be within scope for reduction to zero by 2040 (NHS Carbon Footprint) and 2045 (NHS Carbon Footprint Plus) published by the [Greener NHS](https://www.england.nhs.uk/greenernhs/a-net-zero-nhs/).

## Contents 

**NHS Carbon Footprint**
* [Fossil fuels](/Chapters/001_kmsimg_fossilfuels.md)
* [NHS Facilities](/Chapters/002_kmsimg_facilities.md)
* [Anaesthetics](/Chapters/003_kmsimg_anaesthetics.md)
* [NHS Fleet & leased vehicles](/Chapters/004_kmsimg_fleet.md)
* [Electricity](/Chapters/005_kmsimg_electricity.md)
* [Energy (well-to-tank)](/Chapters/006_kmsimg_welltotank.md)
* [Business travel (public transport, greyfleet etc.)](/Chapters/007_kmsimg_businesstravel.md)
* [Waste](/Chapters/008_kmsimg_waste.md)
* [Water](/Chapters/009_kmsimg_water.md)
* [Metred Dose Inhalers](/Chapters/010_kmsimg_inhalers.md)

**NHS Carbon Footprint Plus** (coming soon!)
* Medical devices
* Freight transport
* Business services
* Construction
* Manufacturing (products, chemicals, gases)
* Medicine
* Food & catering
* Commissioned health services outside NHS
* ICT
* Staff commuting
* Patient and visitor travel

## Get involved

The NHS Emission Quantification Recipe Book has been designed to be a resilient and community-led endeavour that can be easily updated and kept relevant. The GitHub platform is an ideal way to facilitate this functionality. In the video below, Dr Dan Wright provides a quick overview of how you can get involved with the ongoing development of the NHS Emission Quantification Recipe Book through the GitHub forking, pull and commenting functions.

https://user-images.githubusercontent.com/8417968/199349858-cedfdbd8-598f-4d08-b261-8d88dd1a8d99.mp4

## Emailware

The NHS Emission Quantification Recipe Book is [emailware](https://en.wiktionary.org/wiki/emailware). Meaning, if you liked using this tool or it has helped you in any way, please send us an email at <kentcht.sustainability@nhs.net> with any feedback. We really appreciate it!

## Acknowledgements




## Credits

- Version badge created on [Shields.io](https://shields.io/)
- The documents have been developed in [GitHub-flavoured MarkDown](https://github.github.com/gfm/). 

## You may also like...

- [The Context of Vehicle Emissions (COVE) Tool](https://github.com/dvsa)
- [NHS PyCom](https://github.com/nhs-pycom/nhs.pycom)
- [Kent Community Health NHS Foundation Trust](https://kentcht.nhs.uk)

## License

MIT

## Change log

* 04/11/2022 - The first externally-accesible release of the NHS Emission Quantification Recipe Book! The .pdf and .epub versions for general consumption will be released in December 2022. 
