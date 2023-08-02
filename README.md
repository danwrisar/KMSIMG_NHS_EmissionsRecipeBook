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

The *NHS Emission Quantification Recipe Book* is a transparent, collaborative and evidence-based approach to establishing a standardised means of calculating emissions associated with NHS Carbon Footprint and Carbon Footprint Plus themes set out by the [Greener NHS](https://www.england.nhs.uk/greenernhs/) in October 2020 (Figure 1). The NHS Emissions Quantification Recipe Book has been developed by Dr Dan Wright of the Sustainability Team at [Kent Community Health NHS Foundation Trust](https://www.kentcht.nhs.uk/) in collaboration with members of the NHS Kent & Medway Integrated Care System.

Key to the methodologies specified is the recognition that NHS organisations are at different stages in their emissions quantification journey. To support this journey and provide an innovative means to report in a methodologically-transparent way, each theme provides three options for calculation:

* A *Reduced Calculation* (RC) is intended to be an approach to calculating a ballpark figure emission impact using data that should be easily accessible by someone stepping into an emissions reporting role.
* A *Standard Calculation* (SC) is intended to feature the minimum data that NHS organisations should be working towards sourcing and handling, for example, periodical energy consumption data.
* An *Optimal Calculation* (OC) is intended to feature 'best in class' approaches to calculating accurate emissions, this may include using advanced tooling or higher resolution data, for example, half-hourly energy consumption data.

By being transparent around which methodological approach has been used, either RC, SC or OC, this supports 'comparing apples to apples' both within and between [Integrated Care Systems](https://www.england.nhs.uk/integratedcare/what-is-integrated-care/). To demonstrate, here is a worked example for an RC approach to calculating emissions from natural gas use:

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
* [01 Fossil fuels](/Chapters/001_kmsimg_fossilfuels.md)
* 02 NHS Facilities (coming soon!)
* [03 Anaesthetics](/Chapters/003_kmsimg_anaesthetics.md)
* [04 NHS Fleet & leased vehicles](/Chapters/004_kmsimg_fleet.md)
* [05 Electricity](/Chapters/005_kmsimg_electricity.md)
* [06 Energy (well-to-tank)](/Chapters/006_kmsimg_welltotank.md)
* [07 Business travel (public transport, greyfleet etc.)](/Chapters/007_kmsimg_businesstravel.md)
* [08 Waste](/Chapters/008_kmsimg_waste.md)
* [09 Water](/Chapters/009_kmsimg_water.md)
* 10 Metred dose inhalers (coming soon!)

**NHS Carbon Footprint Plus**
* [11 Medical devices](/Chapters/011_kmsimg_medicaldevices.md)
* [12 Freight transport](/Chapters/012_kmsimg_freighttransport.md)
* [13 Business services](/Chapters/013_kmsimg_businessservices.md)
* [14 Construction](/Chapters/014_kmsimg_construction.md)
* [15 Manufacturing](/Chapters/015_kmsimg_manufacturing.md)
* [16 Medicines](/Chapters/016_kmsimg_medicines.md)
* [17 Food & catering](/Chapters/017_kmsimg_food_catering.md)
* [18 Commissioned health services outside NHS](/Chapters/018_kmsimg_commissioned_health.md)
* [19 ICT](/Chapters/019_kmsimg_ICT.md)
* 20 Staff commuting (coming soon!)
* 21 Patient and visitor travel (coming soon!)


## Get involved

The NHS Emission Quantification Recipe Book has been designed to be a resilient and community-led endeavour that can be easily updated and kept relevant. The GitHub platform is an ideal way to facilitate this functionality. In the video below, Dr Dan Wright provides a quick overview of how you can get involved with the ongoing development of the NHS Emission Quantification Recipe Book through the GitHub forking, pull and commenting functions.

https://user-images.githubusercontent.com/8417968/199349858-cedfdbd8-598f-4d08-b261-8d88dd1a8d99.mp4

## Emailware

The NHS Emission Quantification Recipe Book is [emailware](https://en.wiktionary.org/wiki/emailware). Meaning, if you liked using this tool or it has helped you in any way, please send us an email at <kentchft.sustainability@nhs.net> with any feedback. We really appreciate it!

## Acknowledgements

### Authors and CRediT statement

Dan Wright<sup>1</sup>: Conceptualisation, Methodology, Validation, Formal Analysis, Investigation, Writing - Original Draft, Writing - Reviewing and Editing, Visualisation, and Project Administration.

Guy Wing<sup>7</sup>: Methodology, Writing - Original Draft and Resources.

Vicky Cooper<sup>2</sup> and Stu Meades<sup>3</sup>: Methodology and Resources.

James Bate<sup>4</sup>, Sirina Blankson<sup>2</sup>, Emma Clarke<sup>5</sup>, Paul Davis<sup>6</sup>, Julia Hart<sup>6</sup>, Emma Lee-Jarman<sup>1</sup> and Alison Watson<sup>6</sup>: Methodology.

Finn Nightingale<sup>1</sup>: Project Administration.

1. Kent Community Health NHS Foundation Trust
2. Kent and Medway NHS and Social Care Mental Health Trust 
3. Greener Edge Ltd.
4. Greener NHS
5. Kent County Council
6. NHS Kent and Medway
7. Sharpsmart UK
   
### Credits

- Version badge created on [Shields.io](https://shields.io/)
- The documents have been developed in [GitHub-flavoured MarkDown](https://github.github.com/gfm/). 

## You may also like...

- [Context of Vehicle Emissions (COVE) Tool](https://github.com/dvsa)
- [Contributor Roles Taxonomy (CRediT)](https://www.elsevier.com/authors/policies-and-guidelines/credit-author-statement)
- [Kent Community Health NHS Foundation Trust](https://kentcht.nhs.uk)
- [NHS Python Community (PyCom)](https://github.com/nhs-pycom/nhs.pycom)

## License

MIT

## Change log

* 04/01/2022 - The NHS Emission Quantification Recipe Book was shared with members of the Future NHS discussion forum.
* 27/12/2022 - Updated to include authors in readme.md alongside a CRediT statement for transparency.
* 04/11/2022 - The first externally-accesible release of the NHS Emission Quantification Recipe Book!
