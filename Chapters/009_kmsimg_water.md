# 09 Water

<p align="center">
  <a href="#dependencies">Dependencies</a> •
  <a href="#definition">Definition</a> •
  <a href="#methodology">Methodology</a> •
  <a href="#examples">Examples</a>
</p>

## Dependencies

* [The Department for Environment, Food and Rural Affairs (DEFRA) UK and England's carbon footprint to 2019: UK Full dataset 1990 - 2019, including conversion factors by SIC code](https://www.gov.uk/government/statistics/uks-carbon-footprint) (Accessed: 03 November 2022)
* [Department for Business, Energy and Industrial Strategy (BEIS) conversion factors for company reporting](https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting) (Accessed: 22 July 2022)

## Definition

Emissions associated with the supply and treatment of water at owned sites and tenanted sites where the reporter holds billing responsibility to the water supplier.

## Methodology

**Data map**

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Water supply and treatment billing (£) | X |  |  |
| Monitored annual consumption, ≥11% estimated (m<sup>3</sup>) |  | X |  |
| Monitored annual consumption, ≤10% estimated (m<sup>3</sup>) |  |  | X |

**Reduced calculation: Water**

*Equation 9.1* The RC approach for calculating emissions associated with the use of water.

$$
\frac{\left(\text{WatSuppCost} \times \text{WatSICFac} \right) + \left(\text{WatTreat} \times \text{WatSICFac} \right)}
{1000} = \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* WatSuppCost = The cost of water supply (£).
* WatTreatCost = The cost of water treatment (£).
* WatSICFac = The value assigned to "natural water; water treatment and supply services" from a date relevant dataset (kgCO<sub>2</sub>e/£).

**Standard calculation: Water**

*Equation 9.2* The SC approach for calculating emissions associated with the use of water.

$$
\frac{\left(\text{WatSuppVol} \times \text{WatSuppFac} \right) + \left(\text{WatTreatVol} \times \text{WatTreatFac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* WatSuppVol = The volume of water supplied (m<sup>3</sup>) where ≥11% estimated.
* WatSuppFac = The value assigned to emissions associted with supply of water from a date relevant dataset (kgCO<sub>2</sub>e/m<sup>3</sup>).
* WatTreatVol = The volume of water treated (m<sup>3</sup>).
* WatTreatFac = The value assigned to emissions associted with treatment of water from a date relevant dataset (kgCO<sub>2</sub>e/m<sup>3</sup>).

**Optimal calculation: Water**

*Equation 9.3* The OC approach for calculating emissions associated with the use of water.

$$
\frac{\left(\text{WatSuppVol} \times \text{WatSuppFac} \right) + \left(\text{WatTreatVol} \times \text{WatTreatFac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [OC]}
$$

Where:
* WatSuppVol = The volume of water supplied (m<sup>3</sup>) where ≤10% estimated.
* WatSuppFac = The value assigned to emissions associted with supply of water from a date relevant dataset (kgCO<sub>2</sub>e/m<sup>3</sup>).
* WatTreatVol = The volume of water treated (m<sup>3</sup>).
* WatTreatFac = The value assigned to emissions associted with treatment of water from a date relevant dataset (kgCO<sub>2</sub>e/m<sup>3</sup>).

## Examples

**Reduced calculation: Water**

Jeremy sources the[Department for Environment, Food and Rural Affairs (DEFRA) UK and England's carbon footprint to 2019: UK Full dataset 1990 - 2019, including conversion factors by SIC code](https://www.gov.uk/government/statistics/uks-carbon-footprint) dataset. Using the information most relevant to the period being assessed, Jeremy makes a note of the *GHG (kgCO2e per £)* value for 'Natural water; water treatment and supply services'.

Jeremy then multiplies the costs for supply (£400) and treatment (£600) by the intensity metric sourced from DEFRA (0.215kgCO<sub>2</sub>e/£). Jeremy wants to report in tonnes, therefore divides the sum by 1,000 and then rounds to two decimal places. Along with adding their units (tCO<sub>2</sub>e), Jeremy adds the [RC] tag to support transparency around how this figure was calculated. The final value added to Jeremey’s report on emissions associated with water supply and treatment is 0.22tCO<sub>2</sub>e [RC].

*Equation 9.4* A worked example of an RC calculation of emissions associated with supply and treatment of water.

$$
\frac{\left(400 \times 0.215 \right) + \left(600 \times 0.215 \right)}
{1000} = 0.22\text{tCO}_2\text{e} \text{ [RC]}
$$

**Standard calculation: Water**

For more information on ascertaining whether the standard calculation (e.g. where more than, or equal to, 11% of consumption data has been estimated) can be used and a transferable method for using, please see <a href="001_kmsimg_fossilfuels">Fossil Fuels</a>.

**Optimal calculation: Water** 

For more information on ascertaining whether the optimal calculation (e.g. where less than, or equal to, 10% of consumption data has been estimated) can be used and a transferable method for using, please see <a href="001_kmsimg_fossilfuels">Fossil Fuels</a>.