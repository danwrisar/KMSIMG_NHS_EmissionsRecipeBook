# 08 Waste

<p align="center">
  <a href="#introduction">Introduction</a> •
  <a href="#methodology">Methodology</a> •
  <a href="#examples">Examples</a>
</p>

## Introduction

### Dependencies

* [The Department for Environment, Food and Rural Affairs (DEFRA) UK and England's carbon footprint to 2019: UK Full dataset 1990 - 2019, including conversion factors by SIC code](https://www.gov.uk/government/statistics/uks-carbon-footprint) (Accessed: 03 November 2022)
* [Department for Business, Energy and Industrial Strategy (BEIS) conversion factors for company reporting](https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting) (Accessed: 22 July 2022)

### Acknowledgements

Dan Wright<sup>1</sup>, James Bate <sup>2</sup>, Vicky Cooper<sup>3</sup>, Emma Lee-Jarman<sup>1</sup>, Stu Meades<sup>5</sup>, Finn Nightingale<sup>1</sup> & Alison Watson<sup>6</sup>.

1. Kent Community Health NHS Foundation Trust
2. Greener NHS
3. Kent and Medway NHS and Social Care Mental Health Trust 
4. Kent County Council
5. Greener Edge Ltd.
6. Kent and Medway Integrated Care Board

## Methodology

### Definition

Emissions associated with the transport, treatment and end-of-life disposal of materials at any sites where the reporter holds billing responsibility.

### Calculations

#### Data map

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Waste management billing (£) | X |  |  |
| Waste disposal quantities (tonnes) |  | X |  |
| |  |  |  |

#### Reduced calculation

*Equation 8.1* The RC approach for calculating emissions associated with the disposal of waste.

$$
\frac{\left(\text{Waste1Cost} \times \text{WasteSICFac} \right) + \left(\text{Waste2Cost} \times \text{WasteSICFac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* Waste*n*Cost = The cost of disposal of the waste type, with the first waste type being denoted 'Waste1' (£).
* WasteSICFac = The value assigned to "waste collection, treatment and disposal services; materials recovery services" from a date relevant dataset (kgCO<sub>2</sub>e/£).

#### Standard calculation

*Equation 8.2* The SC approach for calculating emissions associated with the disposal of waste.

$$
\frac{\left(\text{Waste1Weight} \times \text{Waste1Fac} \right) + \left(\text{Waste2Cost} \times \text{Waste2Fac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* Waste*n*Weight = The weight of the waste type disposed of, with the first waste type being denoted 'Waste1' (tonnes).
* Waste*n*Fac = The value assigned to the disposal of the waste type by means of disposal from a date relevant dataset (kgCO<sub>2</sub>e/tonne).