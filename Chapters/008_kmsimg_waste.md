# 08 Waste

<p align="center">
  <a href="#dependencies">Dependencies</a> •
  <a href="#definition">Definition</a> •
  <a href="#methodology">Methodology</a> •
  <a href="#examples">Examples</a>
</p>

## Dependencies

* [The Department for Environment, Food and Rural Affairs (DEFRA) UK and England's carbon footprint to 2019: UK Full dataset 1990 - 2019, including conversion factors by SIC code](https://www.gov.uk/government/statistics/uks-carbon-footprint) (Accessed: 03 November 2022)
* [Department for Business, Energy and Industrial Strategy (BEIS) conversion factors for company reporting](https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting) (Accessed: 22 July 2022)
* Chantelle Rizan, Mahmood F. Bhutta, Malcom Reed, Rob Lillywhite, The carbon footprint of waste streams in a UK hospital, Journal of Cleaner Production, Volume 286, 2021
(https://doi.org/10.1016/j.jclepro.2020.125446) (Accessed: 15 June 2023)

[Rizan et al The carbon footprint of waste streams in a UK hospital (003).pdf](https://github.com/danwrisar/KMSIMG_NHS_EmissionsRecipeBook/files/11759553/Rizan.et.al.The.carbon.footprint.of.waste.streams.in.a.UK.hospital.003.pdf)



## Definition

Emissions associated with the transport, treatment and end-of-life disposal of materials at any sites where the reporter holds billing responsibility.

## Methodology

**Data map**

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Waste management billing (£) | X |  |  |
| Waste disposal quantities by waste stream (tonnes) |  | X |  |
| Waste disposal quantities by waste stream (tonnes) <br>  Supplier treatment emission factors by waste stream (kgCO2e/ tonne)<br>  Supplier transport emission by waste stream (kgCO2e/ tonne) |  |  | X |

**Reduced calculation: Waste**

*Equation 8.1* The RC approach for calculating emissions associated with the disposal of waste.

$$
\frac{\left(\text{Waste1Cost} \times \text{WasteSICFac} \right) + \left(\text{Waste2Cost} \times \text{WasteSICFac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* Waste*n*Cost = The cost of disposal of the waste type, with the first waste type being denoted 'Waste1' (£).
* WasteSICFac = The value assigned to "waste collection, treatment and disposal services; materials recovery services" from a date relevant dataset (kgCO<sub>2</sub>e/£).

**Standard calculation: Waste**

*Equation 8.2* The SC approach for calculating emissions associated with the disposal of waste.

$$
\frac{\left(\text{Waste1Weight} \times \text{Waste1Fac} \right) + \left(\text{Waste2Cost} \times \text{Waste2Fac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* Waste*n*Weight = The weight of the waste type disposed of, with the first waste type being denoted 'Waste1' (tonnes).
* Waste*n*Fac = The value assigned to the disposal of the waste type by means of disposal from a date relevant dataset (kgCO<sub>2</sub>e/tonne).

**Optimal calculation: Waste**

*Equation 8.3* The OC approach for calculating emissions associated with the disposal of waste.

$$
\frac{\left(\text{Waste1Weight} \times \text{SupplierWaste1TreatFac}) + (\text{Waste1Weight} \times \text{SupplierWaste1TransFac}) + (\text{Waste2Weight} \times \text{SupplierWaste2TreatFac}) + (\text{Waste2Weight} \times \text{SupplierWaste2TransFac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* Waste*n*Weight = The weight of the waste type disposed of, with the first waste type being denoted 'Waste1' (tonnes).
* Waste*n*Fac = The value assigned to the disposal of the waste type by means of disposal from a date relevant dataset (kgCO<sub>2</sub>e/tonne).
* SupplierWastenTreatFac = The value assigned to the treatment of the waste type, specific to the supplier's treatment process, calculated using Equation 8.4 (kgCO<sub>2</sub>e/tonne)
* SupplierWastenTransFac = The value assigned to the transport of the waste type, specific to the supplier's distance and vehicle type , calculated using Equation 8.5(kgCO<sub>2</sub>e/tonne)

*Equation 8.4* The OC approach for calculating supplier specific emission factors associated with the treatment of waste.

A supplier can calculate the Carbon footprint arising from treating a unit of waste by providing the following inputs:

$$
\frac{\left(\text{Electricity} \times \text{ElectricityFac} \right) + \left(\text{GasOil} \times \text{GasOilFac} \right)  + \left(\text{Water} \times \text{WaterFac} \right) }
{X Tonnes of Waste Stream Proccessed} = \text{kgCO}_2/ tonne waste\text [OC]{e}
$$

Where:
* Electricity = The total electricity consumption used to treat X tonnes of waste by supplier (kWh)
* ElectricityFac = The value assigned to the Carbon footprint per unit of electricity from the BEIS dataset (kgCO<sub>2</sub>/kWh)
* GasOil = The total Gas Oil consumption used to treat X tonnes of waste by supplier (L)
* GasOilFac = The value assigned to the Carbon footprint per unit of Gas Oil from the BEIS dataset (kgCO<sub>2</sub>/L)
* Water = The total water supply and treatment used to treat X tonnes of waste by supplier (m3)
* WaterFac = The value assigned to the Carbon footprint per unit of water supply and treatment from the BEIS dataset (kgCO<sub>2</sub>/m3)
* X Tonnes of Waste Stream Proccessed= The volume of a given waste stream treated correlating to the Inputs measured


*Equation 8.5* The OC approach for calculating supplier specific emission factors associated with the transportation of waste.
TBC



## Examples

Benny wants to calculate the emissions arising from waste produced at Strawberry Hospital using the standard calculation. He has the data for the annual volume of waste produced by each waste stream, and has confirmed that the waste supplier will be treating the waste according to the methods outlined below:


| Waste Stream  | Annual Volume (tonnes)  | Confirmed waste process |
| -----|:---:| :---:|
| Offensive | 120 | Low temperature incineration with EfW |
| Infectious | 40 | Autoclave decontamination followed by  Low temperature incineration with EfW  |
| Anatomical Waste, Cytotoxic Waste, Clinical Waste | 40 | High temperature incineration | 

EfW= energy from waste

Benny will then multiply the weight of each waste type by the waste disposal factor from the relevant dataset: see below from Rizan article

| Waste Stream  |  Waste process | Carbon footprint (kgCO2e/t waste) |
| -----|:---:| :---:|
| Non-infectious offensive waste | Low temperature incineration with EfW | 249 |
| Infectious waste | Autoclave decontamination followed by  Low temperature incineration with EfW | 569  |
| Clinical waste, medicinal contaminated sharps, anatomical waste, medicinal waste | High temperature incineration | 1074 | 


$$
\frac{\left(\text{100} \times \text{249} \right) + \left(\text{40} \times \text{569} \right) + \left(\text{40} \times \text{1074} \right) }
{1000} = \text{90.62 tCO<sub>2</sub>}
$$

