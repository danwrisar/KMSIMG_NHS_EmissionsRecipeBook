# 01 Fossil Fuels

<p align="center">
  <a href="#dependencies">Dependencies</a> •
  <a href="#definition">Definition</a> •
  <a href="#methodology">Methodology</a> •
  <a href="#examples">Examples</a>
</p>

## Dependencies

* [Department for Business, Energy and Industrial Strategy (BEIS) conversion factors for company reporting](https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting) (Accessed: 22 July 2022)
* [Department for Levelling Up, Housing and Communities (DLUHC) energy certificate repository](https://www.gov.uk/find-energy-certificate) (Accessed: 02 November 2022)

## Definition
Emissions associated with the combustion of any gaseous, liquid, and solid fossil fuels at owned sites and tenanted sites where the reporter holds billing responsibility to the energy supplier.

## Methodology

### Calculations: Natural gas

**Data map**

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Modelled energy consumption | X |  |  |
| Monitored annual consumption, ≥11% estimated (kWh) |  | X |  |
| Monitored annual consumption, ≤10% estimated (kWh) |  |  | X |

**Reduced calculation: Natural gas**

*Equation 1.1* The RC approach for natural gas consumption.

$$ 
\frac{\left( \text{ModCon} \times \text{A} \right) \times \text{FuelFac}}
{1000} = \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* ModCon = Value of modelled annual energy use (kWh/m<sup>2</sup>) from the relevant Display Energy Certificate.
* A = Value of total useful floor area (m<sup>2</sup>) from the relevant Display Energy Certificate.
* FuelFac = Carbon factor assigned to the fuel by the relevant BEIS carbon factor database publication.

**Standard calculation: Natural gas**

*Equation 1.2* The SC approach for natural gas consumption.

$$ 
\frac{\text{EstMonCon} \times \text{FuelFac}}
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* EstMonCon = Value of monitored annual energy use (kWh) where ≥11% of data are estimated.
* FuelFac = Carbon factor assigned to the fuel by the relevant BEIS carbon factor database publication.  

**Optimal calculation: Natural gas**

*Equation 1.3* The OC approach for natural gas consumption.

$$ 
\frac{\text{MonCon} \times \text{FuelFac}}
{1000} = \text{tCO}_2\text{e} \text{ [OC]}
$$

Where:
* MonCon = Value of monitored annual energy use (kWh) where ≤10% of data are estimated.
* FuelFac = Carbon factor assigned to the fuel by the relevant BEIS carbon factor database publication.  

## Examples

**Reduced calculation: Natural gas**

Stu sources the Display Energy Certification (DEC) for the building they are interested in using the [energy certificate repository](https://www.gov.uk/find-energy-certificate). Using information from the Building Energy Use figure, Stu multiplies the annual energy use of *other fuels* (328) by the *total useful floor area* for the building (2778.54). The calculated annual total consumption (911,361.12) is presented in kWh. 

By using the [BEIS Conversion Factors dataset for the year they are interested in (2019)](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2019), Stu is able to source a value for emissions per kWh of natural gas use assuming gross calorific value (0.18385kgCO<sub>2</sub>e/kWh). Stu wants to report in tonnes, therefore divides the sum by 1,000 and then rounds to two decimal places. Along with adding their units (tCO<sub>2</sub>e), Stu adds the [RC] tag to support transparency around how this figure was calculated. The final value added to Stu’s report on emissions associated with natural gas consumption is 167.55tCO<sub>2</sub>e [RC].

*Equation 1.4* A worked example of an RC calculation of emissions associated with natural gas consumption.

$$ 
\frac{\left( 328 \times 2778.54 \right) \times 0.18385}
{1000} = 167.55\text{tCO}_2\text{e} \text{ [RC]}
$$

![Example of a Display Energy Certificate](Images/DECExample.png)

*Figure 1.1* Example of data sourced from a Display Energy Certificate.

**Standard calculation: Natural gas**

Julia receives confirmation from her energy supplier that the site she is interested in used 100,000kWh of natural gas over the course of a year she is interested in. The supplier also indicates that the four months at the end of the period being assessed were estimated meter reads (Figure 1.2). Therefore, it can be suggested that 33% of the data underlying the period total consumption were estimated, and it is therefore necessary to use the Standard Calculation (SC) methodology.

By using the [BEIS Conversion Factors dataset for the year she is interested in (2019)](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2019), Julia is able to source a value for emissions per kWh of natural gas use, assuming gross calorific value (0.18385kgCO<sub>2</sub>e/kWh). Julia wants to report in tonnes, therefore divides the sum by 1,000 and then rounds the value to two decimal places. Along with adding her units (tCO<sub>2</sub>e), Julia added the [SC] tag to support transparency around how this value was calculated. The final value added to Julia’s annual report is 18.39tCO<sub>2</sub>e [SC].

*Equation 1.5* A worked example of an SC calculation of emissions associated with natural gas consumption.

$$ 
\frac{100000 \times 0.18385}
{1000} = 18.39\text{tCO}_2\text{e} \text{ [SC]}
$$

![Visualisation of estimated compared to actual consumption](Images/EstimatedMeterReads_Gas.png)

*Figure 1.2* A visualisation of actual and estimated gas consumption.

**Optimal calculation: Natural gas**

Jo receives confirmation from her energy supplier that the site she is interested in used 200,000kWh of natural gas over the course of the year she is interested in. The supplier provides access to data from an installed Automated Meter Reader (AMR) and Jo is able to spot four weeks where no gas was being consumed unexpectedly. As such, data were considered missing for four weeks of a total 48 (for sake of this example), equalling 8.33% of estimated or missing data and 91.67% of verified or intact data. It is therefore possible to use the Optimal Calculation methodology.

By using the [BEIS Conversion Factors dataset for the year she is interested in (2019)](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2019), Jo is able to source a value for emissions per kWh of natural gas use, assuming gross calorific value (0.18385kgCO<sub>2</sub>e/kWh). Jo wants to report in tonnes, therefore divides the sum by 1,000 and then rounds to two decimal places. Along with adding their units (tCO<sub>2</sub>e), Jo adds the [OC] tag to support transparency around how this figure was calculated. The final value added to Jo’s annual report is 36.77tCO<sub>2</sub>e [OC].

*Equation 1.6* A worked example of an OC calculation of emissions associated with natural gas consumption.

$$ 
\frac{200000 \times 0.18385}
{1000} = 36.77\text{tCO}_2\text{e} \text{ [OC]}
$$

![Visualisation of estimated compared to actual consumption](Images/AMRMeterReads_Gas.png)

*Figure 1.3* A visualisation of actual and estimated gas consumption split per week (simplified to 48 weeks across 12 months for demonstration purposes).

