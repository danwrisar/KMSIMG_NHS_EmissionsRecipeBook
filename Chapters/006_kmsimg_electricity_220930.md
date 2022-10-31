# 06 Electricity

[Kent and Medway Sustainability: NHS Emissions Cookbook]

**Authors**:
  Dan Wright<sup>1</sup>, James Bate <sup>2</sup>, Vicky Cooper<sup>3</sup>, Emma Lee-Jarman<sup>1</sup>, Stu Meades<sup>5</sup>, Finn Nightingale<sup>1</sup> & Alison Watson<sup>6</sup>.

1. Kent Community Health NHS Foundation Trust
2. Greener NHS
3. Kent and Medway NHS and Social Care Mental Health Trust 
4. Kent County Council
5. Greener Edge Ltd.
6. Kent and Medway Integrated Care Board

## Introduction

### Dependencies

### Acknowledgements

### To do list

### Notes

The transmission and distribution of energy is considered to be a scope three emissions. As such, it is not included within the scope of the Greener NHS request for emissions from scope two electricity consumption.

## Methodology

### Definition

Emissions associated with the generation of electricity consumed at owned sites and tenanted sites where billing responsibility to the energy supplier is held.

### Data map

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Modelled electricity consumption | X |  |  |
| Monitored annual consumption, $\geq$ 11% estimated (kWh) |  | X |  |
| Monitored annual consumption, $\leq$ 10% estimated (kWh) |  |  | X |

### Calculations

**Reduced calculation**

*Equation 6.1* The RC approach for electricity consumption.

$$ 
\frac{\left( \left( \text{ModCon} \times \text{A} \right) \times \text{GenFac}\right)}

{1000} 

= \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* ModCon = Value of modelled annual electricity use (kWh/m<sup>2</sup>) from the relevant Display Energy Certificate.
* A = Value of total useful floor area (m<sup>2</sup>) from the relevant Display Energy Certificate.
* GenFac = Carbon factor assigned to the generation of electricity by the relevant BEIS carbon factor database publication.

**Standard calculation**

*Equation 6.2* The SC approach for electricity consumption.

$$ 
\frac{\text{EstMonCon} \times \text{GenFac}}
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* EstMonCon = Value of monitored annual electricity use (kWh) where ≥11% of data are estimated.
* GenFac = Carbon factor assigned to the fuel by the relevant BEIS carbon factor database publication.

**Optimal calculation**

*Equation 6.3* The OC approach for electricity consumption.

$$ 
\frac{\text{MonCon} \times \text{GenFac}}
{1000} = \text{tCO}_2\text{e} \text{ [OC]}
$$

Where:
* MonCon = Value of monitored annual electricty use (kWh) where ≤10% of data are estimated.
* GenFac = Carbon factor assigned to the fuel by the relevant DEFRA or BEIS carbon factor database publication.  

### Examples

**Reduced Data Calculation**

Emma sourced the Display Energy Certification (DEC) for the building she was interested in. Using information from the Building Energy Use figure (Figure 6.1), Emma multiplied the annual energy use of electricity (107) by the total useful floor area for the building (2778.54). The calculated annual total consumption (297,303.78) was presented in kWh. 

By using the [BEIS Conversion Factors dataset for the year she is interested in (2019)](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2019), Emma was able to source a value for emissions associated with generating electricity (0.2556kgCO<sub>2</sub>e/kWh). Emma wanted to report in tonnes, therefore divided the sum by 1,000. This value was then rounded to 2 decimal places. Along with adding their units (tCO<sub>2</sub>e), Emma added the [RC] tag to support transparency around how this figure was calculated using a reduced data calculation method. The final value added to Emma’s report on emissions associated with electricity consumption was 75.99tCO<sub>2</sub>e [RC].

*Equation 6.4* A worked example of emissions associated with electricity consumption using an RC method.

$$ 
\frac{\left( 107 \times 2778.54 \right) \times 0.2556}
{1000} = 75.99\text{tCO}_2\text{e} \text{ [RC]}
$$

![Example of a Display Energy Certificate](Images/DECExample.png)

*Figure 6.1* Example of data sourced from a Display Energy Certificate.

**Standard Calculation**

Andy received confirmation from their energy supplier that the site they were interested in used 50,000kWh of electricity over the course of a year. The supplier also indicated that two months preceding the end of the period being assessed were estimated meter reads alongside two months mide year (Figure 6.2). Therefore, it was suggested that 33% of the data underlying the period total consumption were estimated, and it was therefore necessary to use the Standard Calculation methodology.

By using the [BEIS Conversion Factors dataset for the year he was interested in (2019) Andy was able to source a value for emissions associated with generating electricty (0.2556kgCO<sub>2</sub>e/kWh). Andy wanted to report in tonnes, therefore divided the sum by 1,000. This value was then rounded to 2 decimal places. Along with adding their units (tCO<sub>2</sub>e), Andy made sure to add the [SC] tag to support transparency around how this figure was calculated. The final value added to Andy’s annual report was 12.78tCO<sub>2</sub>e [SC].

*Equation 6.5* A worked example of emissions associated with electricity consumption using an SC method.

$$ 
\frac{12780 \times 0.2556}
{1000} = 12.78\text{tCO}_2\text{e} \text{ [SC]}
$$

![Visualisation of estimated compared to actual consumption](Images/EstimatedMeterReads_Elec.png)

*Figure 6.2* A visualisation of actual and estimated electricity consumption data.

**Optimal Calculation**

Irem received confirmation from their energy supplier that the site they were interested in used 18,000kWh of electricity over the course of a year. The supplier provided access to data from an installed Automated Meter Reader (AMR) and Irem was able to spot four weeks where no gas was being consumed unexpectedly. As such, data were missing for four weeks of a total 48 (for sake of this example), equalling 8.33% of estimated or missing data and 91.67% of verified or intact data. It was therefore possible to use the Optimal Calculation methodology.

By using the BEIS Conversion Factors dataset for the year she is interested in (2019), Irem was able to source a value for emissions per kWh of natural gas use, assuming gross calorific value (0.2556kgCO<sub>2</sub>e/kWh). Irem wanted to report in tonnes, therefore divided the sum by 1,000. This value was then rounded to 2 decimal places. Along with adding their units (tCO<sub>2</sub>e), Irem made sure to add the [OC] tag to support transparency around how this figure was calculated. The final value added to Irem’s annual report was 4.60tCO<sub>2</sub>e [OC].

*Equation 6.6* A worked example of emissions associated with electricity consumption using an OC method.

$$ 
\frac{18000 \times 0.2556}
{1000} = 4.60\text{tCO}_2\text{e} \text{ [SC]}
$$

![Visualisation of estimated compared to actual consumption](Images/AMRMeterReads_Elec.png)

*Figure 6.3* A visualisation of actual and estimated gas consumption split per week (simplified to 48 weeks across 12 months for demonstration purposes).
