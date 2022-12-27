# 06 Energy (well-to-tank)

<p align="center">
  <a href="#dependencies">Depedencies</a> •
  <a href="#definition">Definition</a> •
  <a href="#methodology">Methodology</a> •
  <a href="#examples">Examples</a>
</p>

## Dependencies

* [Department for Business, Energy and Industrial Strategy (BEIS) conversion factors for company reporting](https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting) (Accessed: 22 July 2022)
* [Department for Levelling Up, Housing and Communities (DLUHC) energy certificate repository](https://www.gov.uk/find-energy-certificate) (Accessed: 02 November 2022)

## Definition

Emissions associated with the supply of natural gas, the transmission and distribution of electricity, and the supply of fuel for use by NHS Fleet, business-use only leased vehicles and business travel vehicles. 

> NOTE: The transmission and distribution of electricity is included here to mitigate potential 'scoping-out' of associated emissions while retaining accuracy of the methodologies outlined in [05 Electricity](/Chapters/005_kmsimg_electricity.md).

## Methodology

### Calculations: Natural gas (well-to-tank)

**Data map: Natural gas (well-to-tank)**

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal calculation [OC] |
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

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal calculation [OC] |
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

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal calculation [OC] |
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

## Examples