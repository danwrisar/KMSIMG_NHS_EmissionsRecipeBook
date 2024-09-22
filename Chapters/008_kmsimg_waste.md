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
* Rizan, Bhutta, Reed & Lillywhite (2021) The carbon footprint of waste streams in a UK hospital, Journal of Cleaner Production, 286. https://doi.org/10.1016/j.jclepro.2020.125446 (Accessed: 15 June 2023)

## Definition

Emissions associated with the transport, treatment and end-of-life disposal of materials at any sites where the reporter holds billing responsibility.

## Methodology

**Data map**

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Waste management billing (£) | X |  |  |
| Waste disposal quantities by waste stream (tonnes) |  | X | X |
| Supplier treatment emission factors by waste stream (kgCO<sub>2</sub>e/tonne) |  |  | X |
| Supplier transport emission by waste stream (kgCO<sub>2</sub>e/ tonne) |  |  | X |

<!-- 230803 DW demoted the DEFRA SICs approach following conversation with GW 
**Reduced calculation: Waste**

*Equation 8.1* The RC approach for calculating emissions associated with the disposal of waste.

$$
\frac{\left(\text{Wa1Cost} \times \text{WaSICFac} \right) + \left(\text{Wa2Cost} \times \text{WaSICFac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* Wa*n*Cost = The cost of disposal of the waste type, with the first waste type being denoted 'Wa1' (£).
* WaSICFac = The value assigned to "waste collection, treatment and disposal services; materials recovery services" from a date relevant dataset (kgCO<sub>2</sub>e/£).
-->

**Reduced calculation: Waste**

*Equation 8.1* The RC approach for calculating emissions associated with the disposal of waste.

$$
\frac{\left(\text{Wa1Wei} \times \text{Wa1Fac} \right) + \left(\text{Wa2Wei} \times \text{Wa2Fac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* Wa*n*Wei = The weight of the waste type disposed of, with the first waste type being denoted 'Wa1' (tonnes).
* WaType*n*Fac = The value assigned to the disposal of the waste type by means of disposal from the relevant BEIS carbon factor database publication (kgCO<sub>2</sub>e/tonne).

**Standard calculation: Waste**

*Equation 8.2* The SC approach for calculating emissions associated with the disposal of waste.

$$
\frac{\left(\text{Wa1Wei} \times \text{Wa1Fac} \right) + \left(\text{Wa2Wei} \times \text{Wa2Fac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* Wa*n*Wei = The weight of the waste type disposed of, with the first waste type being denoted 'Wa1' (tonnes).
* WaPro*n*Fac = The value assigned to the process for disposal of the waste type confirmed by the treatment provider from [Rizan et al. (p.7, 2021)](https://doi.org/10.1016/j.jclepro.2020.125446) (kgCO<sub>2</sub>e/tonne).

**Optimal calculation: Waste**

*Equation 8.3* The OC approach for calculating emissions associated with the disposal of waste including emissions associated with the supplier treatment and transport of waste.

$$
\frac{\left(\text{Wa1Wei} \times \text{Wa1Treat}) + (\text{Wa1Wei} \times \text{Wa1Tran}) + (\text{Wa2Wei} \times \text{Wa2Treat}) + (\text{Wa2Wei} \times \text{Wa2Tran} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [OC]}
$$

Where:
* Wa*n*Wei = The weight of the waste type disposed of, with the first waste type being denoted 'Wa1' (tonnes).
* Wa*n*Treat = The value assigned to the treatment of the waste type, specific to the supplier's treatment process, calculated using **=** (kgCO<sub>2</sub>e/tonne)
* Wa*n*Tran = The value assigned to the transport of the waste type, specific to the supplier's distance and vehicle type , calculated using Equation 8.5(kgCO<sub>2</sub>e/tonne)
* WaProcessed = Quantity of waste stream processed (tonnes)

*Equation 8.4* The approach to calculating supplier specific emission factors associated with the treatment of a type of waste.

$$
\frac{\left(\text{ElMon} \times \text{ElFac} \right) + \left(\text{GOMon} \times \text{GOFac} \right) + \left(\text{WatMon} \times \text{WatFac} \right) }
{\text{WaPro}} = \text{kgCO}_2\text{e/tonne}
$$

Where:
* ElMonCon = The total monitored electricity used to treat waste by supplier (kWh)
* ElFac = The carbon factor assigned to the generation of electricity by the relevant BEIS carbon factor database publication (kgCO<sub>2</sub>e/kWh).
* GOMon = The total monitored gas oil consumption used to treat waste by supplier (l).
* GOFac = The carbon factor assigned to the combustion of gas oil by the relevant BEIS carbon factor database publication (kgCO<sub>2</sub>e/l).
* Wat = The total water used to treat waste by supplier (m<sup>3</sup>).
* WatFac = The carbon factor assigned to the supply and treatment of water by the relevant BEIS carbon factor database publication (kgCO<sub>2</sub>e/m<sup>3</sup>).
* WaPro = The quantity of waste treated over the relevant period (tonnes).

*Equation 8.5* The approach to calculating supplier specific emission factors associated with the transport of a type of waste.

$$ 
\frac{\left(\text{F1Litres} \times \text{F1Fac} \right) + \left( \text{F2Litres} \times \text{F2Fac} \right) ... }
{\text{WaPro}} = \text{kgCO}_2\text{e/tonne}
$$

Where:
* F*n*Litres = The annual quantity of the distinct fuel type consumed by vehicles transporting waste in the processing process (l), the first fuel type being denoted 'F1' .
* F*n*Fac = The carbon factor assigned to the distinct fuel by the relevant BEIS carbon factor database publication (CO<sub>2</sub>e/litre), the first fuel type being denoted 'F1'.
* WaPro = The quantity of waste treated over the relevant period (tonnes).


## Examples

**Standard calculation: Waste**

Benny wants to calculate the emissions arising from waste produced at Strawberry Hospital over the course of a year using the standard calculation. He has the data for the annual volume of waste produced by each waste stream, and has confirmed the waste supplier's approach to treating each waste stream (Table 8.1).

*Table 8.1* A summary of total waste created per stream and the processes utilised to treat the waste.

| Waste stream  | Annual volume (tonnes)  | Confirmed waste process |
| -----|:---:| :---|
| Offensive | 120 | Low temperature incineration with energy from waste (EfW) |
| Infectious | 40 | Autoclave decontamination followed by low temperature incineration with EfW  |
| Anatomical Waste, Cytotoxic Waste, Clinical Waste | 40 | High temperature incineration | 

Benny sources the emission factor value associated with the process of waste disposal sourced from the most up-to-date appropriate publication, such as the factors proposed by  [Rizan et al. (p.7, 2021)](https://doi.org/10.1016/j.jclepro.2020.125446) featured in Table 8.2.

*Table 8.2* Carbon emission factors associated with disposing of waste per process as per [Rizan et al., (2021)](https://doi.org/10.1016/j.jclepro.2020.125446).

| Waste Stream  |  Waste process | Waste process (kgCO<sub>2</sub>e/t) | Transport (kgCO<sub>2</sub>e/t) | Total (kgCO<sub>2</sub>e/t) |
| ---|:---| :---:| :---:| :---:|
| Recycling reusable surgical instruments | Recycling scrap metal | 21 | 0* | 21 |
| Recycling reusable surgical linens | Recycling clothing | 21 | 0* | 21 |
| Recycling batteries | Recycling batteries | 65 | 0* | 65 |
| Dry mixed recyclable waste | Low temperature incineration with EfW | 167 | 5 | 172 |
| Domestic waste | Low temperature incineration with EfW | 167 | 5 | 172 |
| Non-infectious offensive waste | Low temperature incineration with EfW | 167 | 82 | 249 |
| Infectious waste | Autoclave decontamination followed by low temperature incineration with EfW | 338 | 64 | 569 |
| Clinical waste, medicinal contaminated sharps, anatomical waste, medicinal waste | High temperature incineration | 949 | 125 | 1074 |

\* Emissions associated with transportation included within the processing emissions.

Benny wants to report in tonnes, therefore divides the sum by 1,000 and rounds to two decimal places. Along with adding his units (tCO<sub>2</sub>e), Benny adds the [SC] tag to support transparency around how this figure was calculated. The final value added to Benny’s annual report is 90.62tCO<sub>2</sub>e [SC].

$$
\frac{\left(\text{100} \times \text{249} \right) + \left(\text{40} \times \text{569} \right) + \left(\text{40} \times \text{1074} \right) }
{1000} = \text{90.62} \text{tCO}_2\text{e [SC]}
$$

