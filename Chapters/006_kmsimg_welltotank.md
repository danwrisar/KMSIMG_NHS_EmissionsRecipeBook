# 06 Energy (well-to-tank)

<p align="center">
  <a href="#dependencies">Dependencies</a> •
  <a href="#definition">Definition</a> •
  <a href="#methodology">Methodology</a> •
  <a href="#examples">Examples</a>
</p>

## Dependencies

* [Department for Business, Energy and Industrial Strategy (BEIS) conversion factors for company reporting (full set)](https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting) (Accessed: 22 July 2022)
* [Department for Levelling Up, Housing and Communities (DLUHC) energy certificate repository](https://www.gov.uk/find-energy-certificate) (Accessed: 02 November 2022)

## Definition

Emissions associated with the supply of natural gas, the transmission and distribution of electricity, and the supply of fuel for use by NHS Fleet, business-use only leased vehicles and business travel vehicles. 

> NOTE: The transmission and distribution of electricity is included here to mitigate potential 'scoping-out' of associated emissions while retaining accuracy of the methodologies outlined in [05 Electricity](/Chapters/005_kmsimg_electricity.md).

## Methodology

### Calculations: Natural gas (well-to-tank)

**Data map: Natural gas (well-to-tank)**

| Description of data available  | Reduced calculation [RC] | Standard calculation [SC] | Optimal calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Modelled energy consumption | X |  |  |
| Monitored annual consumption, ≥11% estimated (kWh) |  | X |  |
| Monitored annual consumption, ≤10% estimated (kWh) |  |  | X |

**Reduced calculation: Natural gas (well-to-tank)**

*Equation 6.1* The RC approach for calculating well-to-tank emissions associated with the supply of natural gas.

$$ 
\frac{\left( \text{ModCon} \times \text{A} \right) \times \text{WTTFac}}
{1000} = \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* ModCon = Value of modelled annual energy use (kWh/m<sup>2</sup>) from the relevant Display Energy Certificate.
* A = Value of total useful floor area (m<sup>2</sup>) from the relevant Display Energy Certificate.
* WTTFac = Carbon factor assigned to well-to-tank supply of the fuel by the relevant BEIS carbon factor database publication.

**Standard calculation: Natural gas (well-to-tank)**

*Equation 6.2* The SC approach for calculating well-to-tank emissions associated with the supply of natural gas.

$$ 
\frac{\text{EstMonCon} \times \text{WTTFac}}
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* EstMonCon = Value of monitored annual energy use (kWh) where ≥11% of data are estimated.
* WTTFac = Carbon factor assigned to well-to-tank supply of the fuel by the relevant BEIS carbon factor database publication.  

**Optimal calculation: Natural gas (well-to-tank)**

*Equation 6.3* The OC approach for calculating well-to-tank emissions associated with the supply of natural gas.

$$ 
\frac{\text{MonCon} \times \text{WTTFac}}
{1000} = \text{tCO}_2\text{e} \text{ [OC]}
$$

Where:
* MonCon = Value of monitored annual energy use (kWh) where ≤10% of data are estimated.
* WTTFac = Carbon factor assigned to to well-to-tank supply of the fuel by the relevant BEIS carbon factor database publication. 

## Calculations: Electricity (transmission and distribution)

**Data map: Electricity (transmission and distribution)**

| Description of data available  | Reduced calculation [RC] | Standard calculation [SC] | Optimal calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Modelled electricity consumption | X |  |  |
| Monitored annual consumption, $\geq$ 11% estimated (kWh) |  | X |  |
| Monitored annual consumption, $\leq$ 10% estimated (kWh) |  |  | X |

**Reduced calculation: Electricity (transmission and distribution)**

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

**Standard calculation: Electricity (transmission and distribution)**

*Equation 6.5* The SC approach for calculating transmission and distribution emissions associated with the supply of electricity.

$$ 
\frac{\text{EstMonCon} \times \text{TDFac}}
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* EstMonCon = Value of monitored annual electricity use (kWh) where ≥11% of data are estimated.
* TDFac = Carbon factor assigned to transmission and distribution of grid electricity by the relevant BEIS carbon factor database publication.  

**Optimal calculation: Electricity (transmission and distribution)**

*Equation 6.6* *Equation 6.6* The OC approach for calculating transmission and distribution emissions associated with the supply of electricity.

$$ 
\frac{\text{MonCon} \times \text{TDFac}}
{1000} = \text{tCO}_2\text{e} \text{ [OC]}
$$

Where:
* MonCon = Value of monitored annual electricty use (kWh) where ≤10% of data are estimated.
* TDFac = Carbon factor assigned to transmission and distribution of grid electricity by the relevant BEIS carbon factor database publication.

## Calculations: NHS Fleet and leased vehicles (well-to-tank)

**Data map: NHS Fleet and leased vehicles (well-to-tank)**

| Description of data available  | Reduced calculation [RC] | Standard calculation [SC] | Optimal calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Fuel card expenses (£) | X |  |  |
| Fuel card consumption (litres) |  | X |  |
|  |  |  |  |

**Reduced calculation: NHS Fleet and leased vehicles (well-to-tank)**

*Equation 6.7* The RC approach for calculating emissions from NHS Fleet and leased vehicles.

$$ 
\frac{\left( \frac{\text{F1Cost}}{\text{F1Price}} \times \text{F1WTTFac} \right) + \left( \frac{\text{F2Cost}}{\text{F2Price}} \times \text{F2WTTFac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* F*n*Cost = The total annual cost of the distinct fuel type (£) the first fuel type being denoted 'F1'.
* F*n*Price = The cost per litre of the distinct fuel type (£/litre), the first fuel type being denoted 'F1'.
* F*n*WTTFac = Carbon factor assigned to well-to-tank supply of the fuel by the relevant BEIS carbon factor database publication.

**Standard calculation: NHS Fleet and leased vehicles (well-to-tank)**

*Equation 6.8* The SC approach for calculating emissions from NHS Fleet and leased vehicles.

$$ 
\frac{\left(\text{F1Litres} \times \text{F1WTTFac} \right) + \left( \text{F2Litres} \times \text{F2WTTFac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* F*n*Litres = The annual quantity of the distinct fuel type consumed (litre), the first fuel type being denoted 'F1' .
* F*n*WTTFac = Carbon factor assigned to well-to-tank supply of the fuel by the relevant BEIS carbon factor database publication.

**Optimal calculation: NHS Fleet and leased vehicles (well-to-tank)**

> We're looking for contributors to this open, shared resource! Please check the [issues ticket](https://github.com/danwrisar/KMSIMG_NHS_EmissionsRecipeBook/issues/6) for this theme to get involved. 

## Examples

**Reduced calculation: Natural gas (well-to-tank)**

Alice sources the Display Energy Certification (DEC) for the building she is interested in using the [energy certificate repository](https://www.gov.uk/find-energy-certificate). Using information from the Building Energy Use figure (Fig 6.1), Alice multiplies the annual energy use of *other fuels* (328) by the *total useful floor area* for the building (2778.54). The calculated annual total consumption (911,361.12) is presented in kWh. 

By using the [BEIS Conversion Factors *full* dataset for the year she is interested in (2019)](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2019), Alice is able to source a value for well-to-tank emissions kWh of natural gas use assuming gross calorific value (0.02391kgCO<sub>2</sub>e/kWh). Alice wants to report in tonnes, therefore divides the sum by 1,000 and then rounds to two decimal places. Along with adding her units (tCO<sub>2</sub>e), Alice adds the [RC] tag to support transparency around how this figure was calculated. The final value added to Alice’s report on well-to-tank emissions associated with natural gas consumption is 21.79tCO<sub>2</sub>e [RC].

*Equation 6.10* A worked example of an RC calculation of well-to-tank emissions associated with natural gas consumption.

$$ 
\frac{\left( 328 \times 2,778.54 \right) \times 0.02391}
{1,000} = 21.79\text{tCO}_2\text{e} \text{ [RC]}
$$

![Example of a Display Energy Certificate](Images/DECExample.png)

*Figure 6.1* Example of data sourced from a Display Energy Certificate.

**Standard calculation: Natural gas (well-to-tank)**

Jordan receives confirmation from their energy supplier that the site she is interested in used 100,000kWh of natural gas over the course of the year they are interested in. The supplier also indicates that the four months at the end of the period being assessed were estimated meter reads (Figure 6.2). Therefore, it can be suggested that 33% of the data underlying the period total consumption were estimated, and it is therefore necessary to use the Standard Calculation (SC) methodology.

By using the [BEIS Conversion Factors *full* dataset for the year they are interested in (2019)](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2019), Jordan is able to source a value for well-to-tank emissions kWh of natural gas use assuming gross calorific value (0.02391kgCO<sub>2</sub>e/kWh). Alice wants to report in tonnes, therefore divides the sum by 1,000 and then rounds to two decimal places. Along with adding her units (tCO<sub>2</sub>e), Alice adds the [SC] tag to support transparency around how this figure was calculated. The final value added to Alice’s report on well-to-tank emissions associated with natural gas consumption is 2.39tCO<sub>2</sub>e [SC].

*Equation 6.11* A worked example of an SC calculation of well-to-tank emissions associated with natural gas consumption.

$$ 
\frac{\text{100,000} \times \text{0.02391}}
{1,000} = 2.39 \text{tCO}_2\text{e} \text{ [SC]}
$$  

![Visualisation of estimated compared to actual consumption](Images/EstimatedMeterReads_Gas.png)

*Figure 6.2* A visualisation of actual and estimated gas consumption.  

**Optimal calculation: Natural gas (well-to-tank)**

Boris receives confirmation from his energy supplier that the site he is interested in used 200,000kWh of natural gas over the course of the year he is interested in. The supplier provides access to data from an installed Automated Meter Reader (AMR) and Boris is able to spot four weeks where no gas was being consumed unexpectedly (Figure 6.3). As such, data were considered missing for four weeks of a total 48 (for sake of this example), equalling 8.33% of estimated or missing data and 91.67% of verified or intact data. It is therefore possible to use the Optimal Calculation methodology.

By using the [BEIS Conversion Factors *full* dataset for the year he is interested in (2019)](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2019), Boris is able to source a value for well-to-tank emissions kWh of natural gas use assuming gross calorific value (0.02391kgCO<sub>2</sub>e/kWh). Boris wants to report in tonnes, therefore divides the sum by 1,000 and then rounds to two decimal places. Along with adding his units (tCO<sub>2</sub>e), Boris adds the [OC] tag to support transparency around how this figure was calculated. The final value added to Boris’ report on well-to-tank emissions associated with natural gas consumption is 4.78tCO<sub>2</sub>e [OC].

*Equation 6.12* A worked example of an OC calculation of well-to-tank emissions associated with natural gas consumption.

$$ 
\frac{200000 \times 0.02391}
{1000} = 4.78\text{tCO}_2\text{e} \text{ [OC]}
$$

![Visualisation of estimated compared to actual consumption](Images/AMRMeterReads_Gas.png)