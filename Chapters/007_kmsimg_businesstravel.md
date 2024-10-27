# 07 Business travel (public transport, greyfleet etc.)

<p align="center">
  <a href="#dependencies">Dependencies</a> •
  <a href="#definition">Definition</a> •
  <a href="#methodology">Methodology</a> •
  <a href="#examples">Examples</a>
</p>

## Dependencies

* [Department for Business, Energy and Industrial Strategy (BEIS) conversion factors for company reporting](https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting) (Accessed: 22 July 2022)
* [The Context of Vehicle Emissions (COVE) Tool](https://danwrisar.github.io/COVE-Tool/) (Accessed: 03 November 2022)
* [Department for Transport (DfT) Vehicle Lookup Service](https://vehicleenquiry.service.gov.uk/) (Accessed: 03 November 2022)
* [Department for Transport (DfT) Vehicle licensing statistics data tables: VEH0156](https://www.gov.uk/government/statistical-data-sets/vehicle-licensing-statistics-data-tables#all-vehicles) (Accessed: 03 November 2022)
* Department for Energy Security & Net Zero (DESNZ) Methodology Paper for Conversion Factors Final Report 2024 https://assets.publishing.service.gov.uk/media/66a9fe4ca3c2a28abb50da4a/2024-greenhouse-gas-conversion-factors-methodology.pdf (Accessed: 27 October 2024)

## Definition

Emissions associated with any vehicles formally claiming mileage expenses and/or any travel completed where the reporting organisation has directly paid, or reimbursed the cost, including, but not limited to, travel by air, water, rail, bus and taxi.

> NOTE: Paul Chandler, Deputy Director of Net Zero Travel and Transports for Greener NHS, confirmed that reporting through business travel theme is to be restricted to vehicular transport and not include hotel stays etc. associted with business travel (27 October 2022).

## Methodology

### Calculations: Greyfleet

**Data map**

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| |  |  |  |
| Total mileage (claim data) |  | X |  |
| Mileage per journey (claim data) |  |  | X |

**Standard calculation: Greyfleet**

*Equation 7.2* The SC approach for calculating emissions associated with greyfleet travel.

$$
\frac{\left( \text{TotMil} \times \text{kmConv} \right)\times \text{AvgFac}}
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* TotMil = The total mileage completed by greyfleet over the period of interest.
* AvgFac = The total average emissions (gCO<sub>2</sub>) per kilometre for vehicles first registered in the United Kingdom five years prior to the period of interest.
* kmConv = 1.609344

**Optimal calculation: Greyfleet**

*Equation 7.3* The OC approach for calculating emissions associated with greyfleet.

$$
\frac{\left( \left(\left(\text{V1Mil} \times \text{kmConv} \right) \times \text{V1Fac} \right) \times RWuplift \right) + \left(\left(\left(\text{V2Mil} \times \text{kmConv} \right) \times \text{V2Fac} \right) \times RWuplift \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [OC]}
$$

Where: 

* V*n*Mil = The mileage completed by a unique vehicle over the period of interest (miles), the first unique vehicle being denoted 'V1' .
* V*n*Fac = The registered emissions (gCO<sub>2</sub>) per kilometre for the unique vehicle denoted 'V1'.
* RWuplift = Real World Uplift, an average value used to upscale the registered NEDC or WLTP gCO<sub>2</sub>/km emissions figure to reflect real world driving. See DESNZ Methodology Paper for Conversion factors, Chapter 5 - Passenger Land Transport Emission Factors, for more information and the values used for each year.
* kmConv = The value used to upscale miles to kilometers (1.609344).
