# 07 Business travel (public transport, greyfleet etc.)

## Introduction

### Dependencies

* [Department for Business, Energy and Industrial Strategy (BEIS) conversion factors for company reporting](https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting) (Accessed: 22 July 2022)
* [The Context of Vehicle Emissions (COVE) Tool](https://danwrisar.github.io/COVE-Tool/) (Accessed: 03 November 2022)
* [Department for Transport (DfT) Vehicle Lookup Service](https://vehicleenquiry.service.gov.uk/) (Accessed: 03 November 2022)
* [Department for Transport (DfT) Vehicle licensing statistics data tables: VEH0156](https://www.gov.uk/government/statistical-data-sets/vehicle-licensing-statistics-data-tables#all-vehicles) (Accessed: 03 November 2022)

### Acknowledgements

Dan Wright<sup>1</sup>, James Bate <sup>2</sup>, Vicky Cooper<sup>3</sup>, Paul Davis<sup>4</sup>, Julia Hart<sup>3</sup>, Stu Meades<sup>5</sup> & Alison Watson<sup>6</sup>.

1. Kent Community Health NHS Foundation Trust
2. Greener NHS
3. Kent and Medway NHS and Social Care Mental Health Trust 
4. Maidstone and Tunbridge Wells NHS Trust
5. Greener Edge Ltd.
6. Kent and Medway Integrated Care Board

## Methodology

### Definition

Emissions associated with any vehicles formally claiming mileage expenses and/or any travel completed where the reporting organisation has directly paid, or reimbursed the cost, including, but not limited to, travel by air, water, rail, bus and taxi.

> NOTE: Paul Chandler, Deputy Director of Net Zero Travel and Transports for Greener NHS, confirmed that reporting through business travel theme is to be restricted to vehicular transport and not include hotel stays etc. associted with business travel (27 October 2022).

### Calculations: Greyfleet

#### Data map

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| |  |  |  |
| Total mileage (claim data) |  | X |  |
| Mileage per journey (claim data) |  |  | X |

#### Standard calculation: Greyfleet

*Equation 7.2* The SC approach for calculating emissions associated with greyfleet travel.

$$
\frac{\left( \text{TotMil} \times \text{kmConv} \right)\times \text{AvgFac}}
{1000} = \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* TotMil = The total mileage completed by greyfleet over the period of interest.
* AvgFac = The total average emissions (gCO2) per kilometre for vehicles first registered in the United Kingdom five years prior to the period of interest.
* kmConv = 1.609344

#### Optimal calculation: Greyfleet

*Equation 7.3* The OC approach for calculating emissions associated with greyfleet.

$$
\frac{\left(\left(\text{V1Mil} \times \text{kmConv} \right) \times \text{V1Fac} \right) + \left(\left(\text{V2Mil} \times \text{kmConv} \right) \times \text{V2Fac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where: 

* V*n*Mil = The mileage completed by a unique vehicle over the period of interest (miles), the first unique vehicle being denoted 'V1' .
* V*n*Fac = The registered emissions (gCO2) per kilometre for the unique vehicle denoted 'V1'.
* kmConv = 1.609344