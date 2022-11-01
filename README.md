> A transparent, collaborative and evidence-based approach to establishing a standardised means of calculating emissions associated with NHS Carbon Footprint and Carbon Footprint Plus themes set out by the [Greener NHS](https://www.england.nhs.uk/greenernhs/) in October 2020. The NHS Emissions Quantification Recipe Book has been developed by Dr Dan Wright of the Sustainability Team at [Kent Community Health NHS Foundation Trust](https://www.kentcht.nhs.uk/) in collaboration with members of the Kent & Medway Sustainability Impacts and Methodologies Group (KMS-IMG).

<h1 align="center">
  <br>
  <img src="https://github.com/danwrisar/KMSIMG_NHS_EmissionsCookbook/blob/main/Images/recipebook.png" alt="NHS Emission Recipe Book Logo" width="200">
  <br>
  The NHS Emission Quantification Recipe Book
  <br>

[![GitHub Release](https://img.shields.io/badge/Version-22%2F23-blue)]()  
</h1>

<p align="center">
  <a href="#how-to-use">How To Use</a> •
  <a href="#get-involved">Get Involved</a> •
  <a href="#license">License</a> •
  <a href="#change-log">Change log</a>
</p>

## How to use

This repository features a series of documents developed in [GitHub-flavoured MarkDown](https://github.github.com/gfm/) to collate best practice around quantification of emissions within Greener NHS themes (Fig 1). 

Each document features:
* A definition of what is included within the theme
* A data map highlighting which data are requried for the details methods.
* An overview of calculation approaches including:
  * Reduced Calculation (RC)
  * Standard Calculation (SC)
  * Optimal Calculation (OC)
* Worked examples of calculating emissions using the RC, SC and OC methods. 

**NHS Carbon Footprint**
* [Fossil fuels](/Chapters/001_kmsimg_fossilfuels.md)
* [NHS Facilities](/Chapters/002_kmsimg_facilities.md)
* [Anaesthetics](/Chapters/003_kmsimg_anaesthetics.md)
* [NHS Fleet &  leased vehicles](/Chapters/004_kmsimg_fleet.md)
* [Electricity](/Chapters/005_kmsimg_electricity.md)
* [Energy (well to tank)](/Chapters/006_kmsimg_welltotank.md)
* [Business travel (public transport, greyfleet etc.)](/Chapters/007_kmsimg_businesstravel.md)
* [Waste](/Chapters/008_kmsimg_waste.md)
* [Water](/Chapters/009_kmsimg_water.md)
* [Metred Dose Inhalers](/Chapters/010_kmsimg_inhalers.md)

**NHS Carbon Footprint Plus**
* [Medical devices](/Chapters/011_kmsimg_medicaldevices.md)

<p align="center">
    <img src="https://github.com/danwrisar/KMSIMG_NHS_EmissionsCookbook/blob/main/Images/NZR-Scopes.png" alt="Greener NHS Net Zero Scopes" width="500">
</p>

Fig 1. A summary of the themes considered to be within scope for reduction to zero by 2040 (NHS Carbon Footprint) and 2045 (NHS Carbon Footprint Plus) published by the [Greener NHS](https://www.england.nhs.uk/greenernhs/a-net-zero-nhs/).

## Get involved

The best way to get involved is to address the issue log and create a pull request with fixes...

## Emailware

The NHS Emission Quantification Recipe Book is [emailware](https://en.wiktionary.org/wiki/emailware). Meaning, if you liked using this tool or it has helped you in any way, please send us an email at <kentcht.sustainability@nhs.net> with any feedback. We really appreciate it!

## Credits

This software uses the following packages:

- [Pandas](https://pandas.pydata.org/)
- [Numpy](https://numpy.org/)
- [Plotly](https://pypi.org/project/plotly/)
- Version badge: [Shields.io](https://shields.io/)

## You may also like...

- [Driver & Vehicle Standards Agency](https://github.com/dvsa)
- [NHS PyCom](https://github.com/nhs-pycom/nhs.pycom)
- [Kent Community Health NHS Foundation Trust](https://kentcht.nhs.uk)

## License

MIT

## Change log

* Context of Vehicle Emissions (COVE) Tool v1.0 - 28 June 2022
  - Initial public release sharing 1) The means of implementation to contextualise mileage claim datasets with the DoT's Vehicle Enquiry Service API, and 2) An approach to wrangling mileage claim data to facilitate contextualisation.