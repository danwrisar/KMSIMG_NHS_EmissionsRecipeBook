# 09 Water

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

Emissions associated with the supply and treatment of water at owned sites and tenanted sites where the reporter holds billing responsibility to the water supplier.

### Calculations

#### Data map

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Water supply and treatment billing (£) | X |  |  |
| Water supply and treatment logging (m^3^) |  | X |  |
| |  |  |  |

#### Reduced calculation

*Equation 9.1* The RC approach for calculating emissions associated with the disposal of waste.

$$
\frac{\left(\text{WatSuppCost} \times \text{WatSICFac} \right) + \left(\text{WatTreat} \times \text{WatSICFac} \right)}
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* WatSuppCost = The cost of water supply (£).
* WatTreatCost = The cost of water treatment (£).
* WatSICFac = The value assigned to "natural water; water treatment and supply services" from a date relevant dataset (kgCO~2~e/£).

#### Standard calculation

*Equation 8.2* The SC approach for calculating emissions associated with the disposal of waste.

$$
\frac{\left(\text{WatSuppVol} \times \text{WatSuppFac} \right) + \left(\text{WatTreatVol} \times \text{WatTreatFac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* WatSuppVol = The volume of water supplied (m^3^).
* WatSuppFac = The value assigned to emissions associted with supply of water from a date relevant dataset (kgCO~2~e/m^3^).
* WatTreatVol = The volume of water treated (m^3^).
* WatTreatFac = The value assigned to emissions associted with treatment of water from a date relevant dataset (kgCO~2~e/m^3^).