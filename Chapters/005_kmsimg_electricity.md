# 05 Electricity

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

Emissions associated with the generation of electricity consumed at owned sites and tenanted sites where the reporter holds billing responsibility to the energy supplier.

> NOTE: The transmission and distribution of energy is considered to be a *scope three* emission. As such, it is not included within the the Greener NHS request for *scope two* emissions from electricity consumption and is instead included in [06 Energy (well-to-tank)](/Chapters/006_kmsimg_welltotank.md).

## Methodology

### Calculations: Electricity

**Data map**

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Modelled electricity consumption | X |  |  |
| Monitored annual consumption, &gt; 10% estimated (kWh) |  | X |  |
| Monitored annual consumption, $\leq$ 10% estimated (kWh) |  |  | X |

**Reduced calculation: Electricity**

*Equation 5.1* The RC approach for electricity consumption.

$$ 
\frac{\left( \left( \text{ModCon} \times \text{A} \right) \times \text{GenFac}\right)}
{1000} 
= \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* ModCon = Value of modelled annual electricity use (kWh/m<sup>2</sup>) from the relevant Display Energy Certificate.
* A = Value of total useful floor area (m<sup>2</sup>) from the relevant Display Energy Certificate.
* GenFac = Carbon factor assigned to the generation of electricity by the relevant BEIS carbon factor database publication.

**Standard calculation: Electricity**

*Equation 5.2* The SC approach for electricity consumption.

$$ 
\frac{\text{EstMonCon} \times \text{GenFac}}
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* EstMonCon = Value of monitored annual electricity use (kWh) where >10% of data are estimated.
* GenFac = Carbon factor assigned to the fuel by the relevant BEIS carbon factor database publication.

**Optimal calculation: Electricity**

*Equation 5.3* The OC approach for electricity consumption.

$$ 
\frac{\text{MonCon} \times \text{GenFac}}
{1000} = \text{tCO}_2\text{e} \text{ [OC]}
$$

Where:
* MonCon = Value of monitored annual electricty use (kWh) where ≤10% of data are estimated.
* GenFac = Carbon factor assigned to the fuel by the relevant BEIS carbon factor database publication.  

## Examples

**Reduced calculation: Electricity**

Emma sources the Display Energy Certification (DEC) for the building she was interested in using the [energy certificate repository](https://www.gov.uk/find-energy-certificate). Using information from the Building Energy Use figure (Figure 5.1), Emma multiplied the annual energy use of electricity (107) by the total useful floor area for the building (2778.54). The calculated annual total consumption (297,303.78) was presented in kWh. 

By using the [BEIS Conversion Factors dataset for the year she is interested in (2019)](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2019), Emma was able to source a value for emissions associated with generating electricity (0.2556kgCO<sub>2</sub>e/kWh). Emma wanted to report in tonnes, therefore divided the sum by 1,000. This value was then rounded to 2 decimal places. Along with adding their units (tCO<sub>2</sub>e), Emma added the [RC] tag to support transparency around how this figure was calculated using a reduced data calculation method. The final value added to Emma’s report on emissions associated with electricity consumption was 75.99tCO<sub>2</sub>e [RC].

*Equation 5.4* A worked example of emissions associated with electricity consumption using an RC method.

$$ 
\frac{\left( 107 \times 2778.54 \right) \times 0.2556}
{1000} = 75.99\text{tCO}_2\text{e} \text{ [RC]}
$$

![Example of a Display Energy Certificate](Images/DECExample.png)

*Figure 5.1* Example of data sourced from a Display Energy Certificate.

**Standard calculation: Electricity**

Andy receives confirmation from his energy supplier that the site he is interested in used 50,000kWh of electricity over the course of a year. The supplier also indicates that four months were estimated usage, including two months at the end of the year (Figure 5.2). Therefore, it can be suggested that 33% of the data underlying the period total consumption were estimated, and it is necessary to use the Standard Calculation methodology.

By using the [BEIS Conversion Factors dataset for the year he is interested in (2019)](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2019), Andy is able to source a value for emissions associated with generating electricty (0.2556kgCO<sub>2</sub>e/kWh). Andy wants to report in tonnes, therefore divides the sum by 1,000 and rounds to two decimal places. Along with adding his units (tCO<sub>2</sub>e), Andy adds the [SC] tag to support transparency around how this figure was calculated. The final value added to Andy’s annual report is 12.78tCO<sub>2</sub>e [SC].

*Equation 5.5* A worked example of emissions associated with electricity consumption using an SC method.

$$ 
\frac{12780 \times 0.2556}
{1000} = 12.78\text{tCO}_2\text{e} \text{ [SC]}
$$

![Visualisation of estimated compared to actual consumption](Images/EstimatedMeterReads_Elec.png)

*Figure 5.2* A visualisation of actual and estimated electricity consumption data.

**Optimal calculation: Electricity**

Irem receives confirmation from her energy supplier that the site they are interested in used 18,000kWh of electricity over the course of a year. The supplier provides access to data from an installed Automated Meter Reader (AMR) and Irem is able to spot four weeks where no electricity was being consumed unexpectedly (Figure 5.3). As such, data were missing for four weeks of a total 48 (for the sake of this example), equalling 8.33% of estimated or missing data and 91.67% of verified or intact data. It is possible to use the Optimal Calculation methodology.

By using the [BEIS Conversion Factors dataset for the year she is interested in (2019)](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2019), Irem was able to source a value for emissions per kWh of natural gas use, assuming gross calorific value (0.2556kgCO<sub>2</sub>e/kWh). Irem wants to report in tonnes, therefore divides the sum by 1,000 and rounds to two decimal places. Along with adding her units (tCO<sub>2</sub>e), Irem adds the [OC] tag to support transparency around how this figure was calculated. The final value added to Irem’s annual report is 4.60tCO<sub>2</sub>e [OC].

*Equation 5.6* A worked example of emissions associated with electricity consumption using an OC method.

$$ 
\frac{18000 \times 0.2556}
{1000} = 4.60\text{tCO}_2\text{e} \text{ [OC]}
$$

![Visualisation of estimated compared to actual consumption](Images/AMRMeterReads_Elec.png)

*Figure 5.3* A visualisation of actual and estimated electricity consumption split per week (simplified to 48 weeks across 12 months for demonstration purposes).
