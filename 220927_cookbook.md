# Kent & Medway Sustainability: NHS Emissions Cookbook 

**Authors**:
  Dan Wright<sup>1</sup>, James Bate <sup>2</sup>, Sirina Blankson<sup>3</sup>, Emma Clarke<sup>4</sup>, Vicky Cooper<sup>3</sup>, Stu Meades<sup>5</sup>, John Mills<sup>6</sup>, Finn Nightingale<sup>1</sup> & Alison Watson<sup>7</sup>.

1. Kent Community Health NHS Foundation Trust
2. Greener NHS
3. Kent and Medway NHS and Social Care Mental Health Trust 
4. Kent County Council
5. Greener Edge Ltd.
6. 2gether Support Solutions
7. Kent and Medway Integrated Care Board

[Intro]

Dependencies

* [Department for Business, Energy and Industrial Strategy (BEIS) conversion factors for company reporting](https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting) (Accessed: 22 July 2022)

Acknowledgements

Approach inspired by the Domestic Operation Rating (Lomas et al., 2020)

Equations Karl Landers and Raul Jimenez van Hoorn

## Fossil fuels

### Definition
Emissions associated with combustion of any gaseous, liquid, and solid fossil fuels and owned sites and tenanted sites where billing responsibility to the energy supplier is held.

### Data map

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Modelled energy consumption | X |  |  |
| Monitored annual consumption, ≥11% estimated (kWh) |  | X |  |
| Monitored annual consumption, ≤10% estimated (kWh) |  |  | X |

### Calculations: Natural gas

**Reduced calculation**

$$ 
\frac{\left( \text{ModCon} \times \text{A} \right) \times \text{Fac}}
{1000} = \text{tCO}_2\text{e}_\text{ [RC]}
$$

Where:
* ModCon = Value of modelled annual energy use (kWh/m<sup>2</sup>) from the relevant Display Energy Certificate.
* A = Value of total useful floor area (m<sup>2</sup>) from the relevant Display Energy Certificate.
* Fac = Carbon factor assigned to the fuel by the relevant BEIS carbon factor database publication.  

**Standard calculation**

$$ 
\frac{\text{EstMonCon} \times \text{Fac}}
{1000} = \text{tCO}_2\text{e}_\text{ [SC]}
$$

Where:
* EstMonCon = Value of monitored annual energy use (kWh) where ≥11% of data are estimated.
* Fac = Carbon factor assigned to the fuel by the relevant BEIS carbon factor database publication.  

**Optimal calculation**

$$ 
\frac{\text{MonCon} \times \text{Fac}}
{1000} = \text{tCO}_2\text{e}_\text{ [OC]}
$$

Where:
* MonCon = Value of monitored annual energy use (kWh) where ≤10% of data are estimated.
* Fac = Carbon factor assigned to the fuel by the relevant DEFRA or BEIS carbon factor database publication.  

### Examples

**Reduced Data Calculation**

Stu sources the Display Energy Certification (DEC) for the building he is interested in. Using information from the Building Energy Use figure (Figure 1), Stu multiplies the annual energy use of other fuels (328) by the total useful floor area for the building (2778.54). The calculated annual total consumption (911,361.12) is presented in kWh. 

By using the BEIS Carbon Factors  for the year he is interested in (2019), Stu was able to source a value for emissions per kWh of natural gas use assuming gross calorific value (0.18385kgCO<sub>2</sub>e/kWh). Stu wanted to report in tonnes, therefore divided the sum by 1,000. This value was then rounded to 2 decimal places. 
Along with adding their units (tCO<sub>2</sub>e), Stu added the <sup>RC</sup> tag to support transparency around how this figure was calculated using a reduced data calculation method. The final value added to Stu’s report on emissions associated with natural gas consumption was 167.55tCO<sub>2</sub>e<sup>RC</sup>.

![Example of a Display Energy Certificate](Images/DECExample.png)
Figure 1. Example of a 