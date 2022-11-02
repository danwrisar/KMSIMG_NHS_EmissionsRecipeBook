# 06 Energy (well-to-tank)

## Introduction

### Dependencies

* [Department for Business, Energy and Industrial Strategy (BEIS) conversion factors for company reporting](https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting) (Accessed 22 July 2022)
* [Department for Levelling Up, Housing and Communities (DLUHC) energy certificate repository](https://www.gov.uk/find-energy-certificate) (Accessed 02 November 2022)

### Acknowledgements

Dan Wright<sup>1</sup>

1. Kent Community Health NHS Foundation Trust

## Methodology

### Definition

Emissions associated with the supply of natural gas, the transmission and distribution of electricity, and the supply of fuel for use by NHS Fleet, business-use only leased vehicles and business travel vehicles. 

> NOTE: The transmission and distribution of electricity is included here to mitigate potential 'scoping-out' of associated emissions while retaining accuracy of the methodologies outlined in [05 Electricity](/Chapters/005_kmsimg_electricity.md).

### Calculations: Natural gas (well-to-tank)

#### Data map

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Modelled energy consumption | X |  |  |
| Monitored annual consumption, ≥11% estimated (kWh) |  | X |  |
| Monitored annual consumption, ≤10% estimated (kWh) |  |  | X |

##### Reduced calculation: Natural gas (well-to-tank)

*Equation 6.1* The RC approach for calculating well-to-tank emissions associated with the supply of natural gas.

$$ 
\frac{\left( \text{ModCon} \times \text{A} \right) \times \text{WTTFac}}
{1000} = \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* ModCon = Value of modelled annual energy use (kWh/m<sup>2</sup>) from the relevant Display Energy Certificate.
* A = Value of total useful floor area (m<sup>2</sup>) from the relevant Display Energy Certificate.
* WTTFac = Carbon factor assigned to well-to-tank supply of the fuel by the relevant BEIS carbon factor database publication.

##### Standard calculation: Natural gas (well-to-tank)

*Equation 6.2* The SC approach for calculating well-to-tank emissions associated with the supply of natural gas.

$$ 
\frac{\text{EstMonCon} \times \text{WTTFac}}
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* EstMonCon = Value of monitored annual energy use (kWh) where ≥11% of data are estimated.
* WTTFac = Carbon factor assigned to well-to-tank supply of the fuel by the relevant BEIS carbon factor database publication.  

##### Optimal calculation: Natural gas (well-to-tank)

*Equation 6.3* The OC approach for calculating well-to-tank emissions associated with the supply of natural gas.

$$ 
\frac{\text{MonCon} \times \text{WTTFac}}
{1000} = \text{tCO}_2\text{e} \text{ [OC]}
$$

Where:
* MonCon = Value of monitored annual energy use (kWh) where ≤10% of data are estimated.
* WTTFac = Carbon factor assigned to to well-to-tank supply of the fuel by the relevant BEIS carbon factor database publication. 

### Calculations: Electricity (transmission and distribution)

#### Data map

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Modelled electricity consumption | X |  |  |
| Monitored annual consumption, $\geq$ 11% estimated (kWh) |  | X |  |
| Monitored annual consumption, $\leq$ 10% estimated (kWh) |  |  | X |

##### Reduced calculation: Electricity (transmission and distribution)

*Equation 6.4* The RC approach for calculating transmission and distribution emissions associated with the supply of electricity.

$$ 
\frac{\left( \left( \text{ModCon} \times \text{A} \right) \times \text{TDFac}\right)}
{1000} 
= \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* ModCon = Value of modelled annual electricity use (kWh/m<sup>2</sup>) from the relevant Display Energy Certificate.
* A = Value of total useful floor area (m<sup>2</sup>) from the relevant Display Energy Certificate.
* TDFac = Carbon factor assigned to transmission and distribution of grid electricity by the relevant BEIS carbon factor database publication.  

##### Standard calculation: Electricity (transmission and distribution)

*Equation 6.5* The SC approach for calculating transmission and distribution emissions associated with the supply of electricity.

$$ 
\frac{\text{EstMonCon} \times \text{TDFac}}
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* EstMonCon = Value of monitored annual electricity use (kWh) where ≥11% of data are estimated.
* TDFac = Carbon factor assigned to transmission and distribution of grid electricity by the relevant BEIS carbon factor database publication.  

##### Optimal calculation: Electricity (transmission and distribution)

*Equation 6.6* *Equation 6.6* The OC approach for calculating transmission and distribution emissions associated with the supply of electricity.

$$ 
\frac{\text{MonCon} \times \text{TDFac}}
{1000} = \text{tCO}_2\text{e} \text{ [OC]}
$$

Where:
* MonCon = Value of monitored annual electricty use (kWh) where ≤10% of data are estimated.
* TDFac = Carbon factor assigned to transmission and distribution of grid electricity by the relevant BEIS carbon factor database publication.

### Calculations: NHS Fleet and leased vehicles (well-to-tank)

#### Data map

**Standard calculation: NHS Fleet and leased vehicles**

*Equation 6.8* The SC approach for XXXXXX.

$$ 
\frac{\left( \text{ModCon} \times \text{A} \right) \times \text{Fac}}
{1000} = \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* XXX = XXX

## Examples

**Standard calculation: Natural gas**

Stu sources the Display Energy Certification (DEC) for the building he is interested in. Using information from the Building Energy Use figure (Figure 1.1), Stu multiplies the annual energy use of other fuels (328) by the total useful floor area for the building (2778.54). The calculated annual total consumption (911,361.12) is presented in kWh. 

By using the BEIS Carbon Factors  for the year he is interested in (2019), Stu was able to source a value for emissions per kWh of natural gas use assuming gross calorific value (0.18385kgCO<sub>2</sub>e/kWh). Stu wanted to report in tonnes, therefore divided the sum by 1,000. This value was then rounded to 2 decimal places. 
Along with adding their units (tCO<sub>2</sub>e), Stu added the [RC] tag to support transparency around how this figure was calculated using a reduced data calculation method. The final value added to Stu’s report on emissions associated with natural gas consumption was 167.55tCO<sub>2</sub>e [RC].

*Equation X.4* A worked example of emissions associated with XXXXXXXX using an RC method.

$$ 
\frac{\left( 328 \times 2778.54 \right) \times 0.18385}
{1000} = 167.55\text{tCO}_2\text{e} \text{ [RC]}
$$

**Standard Calculation**

*Equation X.5* A worked example of emissions associated with XXXXXXXX using an SC method.

**Optimal Calculation**

*Equation X.6* A worked example of emissions associated with XXXXXXXX using an OC method.
