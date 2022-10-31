# 05 NHS Fleet & Leased Vehicles

[Kent and Medway Sustainability: NHS Emissions Cookbook]

**Authors**:
  Dan Wright<sup>1</sup>, James Bate <sup>2</sup>, Vicky Cooper<sup>3</sup>, Paul Davis<sup>4</sup>, Julia Hart<sup>3</sup>, Stu Meades<sup>5</sup> & Alison Watson<sup>6</sup>.

1. Kent Community Health NHS Foundation Trust
2. Greener NHS
3. Kent and Medway NHS and Social Care Mental Health Trust 
4. Maidstone and Tunbridge Wells NHS Trust
5. Greener Edge Ltd.
6. Kent and Medway Integrated Care Board

## Introduction

### Dependencies

* [RAC Fuel Watch](https://www.rac.co.uk/drive/advice/fuel-watch/) (Accessed 30 September 2022)
* [Department for Business, Energy and Industrial Strategy (BEIS) conversion factors for company reporting](https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting) (Accessed 22 July 2022)

### Acknowledgements

### To do list

* NHS Fleeet & Leased Vehicles: OC
* NHS Fleet & Leased Vehicles: OC example

### Definition
Emissions associated with any travel completed by business-only vehicles owned and/or operated by the trust.

### Data map

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Fuel card expenses (£) | X |  |  |
| Fuel card consumption (litres) |  | X |  |
|  |  |  |  |

### Methodology

**Reduced calculation**

*Equation 5.1* The RC approach for calculating emissions from NHS Fleet & Leased Vehicles.

$$ 
\frac{\left( \frac{\text{F1Cost}}{\text{F1Price}} \times \text{F1Fac} \right) + \left( \frac{\text{F2Cost}}{\text{F2Price}} \times \text{F2Fac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* F*n*Cost = The total annual cost of the distinct fuel type (£) the first fuel type being denoted 'F1'.
* F*n*Price = The cost per litre of the distinct fuel type (£/litre), the first fuel type being denoted 'F1' .
* F*n*Fac = The carbon factor assigned to the distinct fuel by the relevant BEIS carbon factor database publication (CO<sub>2</sub>e/litre), the first fuel type being denoted 'F1'.

**Standard calculation**

*Equation 5.2* The SC approach for natural gas consumption.

$$ 
\frac{\left(\text{F1Litres} \times \text{F1Fac} \right) + \left( \text{F2Litres} \times \text{F2Fac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* F*n*Litres = The annual quantity of the distinct fuel type consumed (litre), the first fuel type being denoted 'F1' .
* F*n*Fac = The carbon factor assigned to the distinct fuel by the relevant BEIS carbon factor database publication (CO<sub>2</sub>e/litre), the first fuel type being denoted 'F1'.

### Examples

**Reduced Data Calculation**

Raul is able to source total cost of fuel for the year he is interested in from the relevant department. Crucially, he knows how much was spent per individual fuel, with £10,000 spent on unleaded fuel and £20,000 spent on diesel fuel. Raul uses a recognised source, such as the [RAC Fuel Watch database](https://www.rac.co.uk/drive/advice/fuel-watch/), to establish a cost per unit to enable him to extract the litres of fuel that correspond to the aforementioned total cost per fuel. In 2019, the cost of unleaded fuel was £1.2578 per litre while the cost of diesel fuel was £1.3117 per litre. 

By using the BEIS Carbon Factors for the year he is interested in (2019), Raul was able to source a value for emissions per litre of unleaded fuel with an average biofuel blend (2.19585kgCO<sub>2</sub>e/litre) and per litre of diesel fuel with an average biofuel blend (2.59411kgCO<sub>2</sub>e/litre). Raul wanted to report in tonnes, therefore divided the sum by 1,000. This value was then rounded to 2 decimal places. Along with adding their units (tCO<sub>2</sub>e), Raul added the [RC] tag to support transparency around how this figure was calculated using a reduced data calculation method. The final value added to Raul’s report on emissions associated with NHS Fleet & Leased Vehicles was 57.01tCO<sub>2</sub>e [RC].

*Equation 5.4* A worked example of emissions associated with NHS Fleet & Leased Vehicles using an RC method.

$$ 
\frac{\left( \frac{\text{10000}}{\text{1.2578}} \times \text{2.19585} \right) + \left( \frac{\text{20000}}{\text{1.3117}} \times \text{2.59411} \right) ... }
{1000} = 57.01\text{tCO}_2\text{e} \text{ [RC]}
$$

**Standard Calculation**

Maxine has access to fuel cards records which state total quantities of distinct fuels purchased over the course of the year she is interested in. She knows that 20,000 litres of unleaded fuel were purchased and 10,000litres od diesel fuel were purchased. By using the BEIS Carbon Factors for the year she is interested in (2019), Maxine was able to source a value for emissions per litre of unleaded fuel with an average biofuel blend (2.19585kgCO<sub>2</sub>e/litre) and per litre of diesel fuel with an average biofuel blend (2.59411kgCO<sub>2</sub>e/litre). 

Maxine wanted to report in tonnes, therefore divided the sum by 1,000. This value was then rounded to 2 decimal places. Along with adding her units (tCO<sub>2</sub>e), Maxine added the [SC] tag to support transparency around how this figure was calculated using a standard data calculation method. The final value added to Maxine's report on emissions associated with NHS Fleet & Leased Vehicles was 30.33tCO<sub>2</sub>e [SC].

*Equation 5.5* A worked example of emissions associated with NHS Fleet & Leased Vehicles using an SC method.

$$ 
\frac{\left(\text{20000} \times \text{2.19585} \right) + \left( \text{10000} \times \text{2.59411} \right) ... }
{1000} = 30.33\text{tCO}_2\text{e} \text{ [SC]}
$$

