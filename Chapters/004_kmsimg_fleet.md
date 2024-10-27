# 04 NHS Fleet & Leased Vehicles

<p align="center">
  <a href="#dependencies">Dependencies</a> •
  <a href="#definition">Definition</a> •
  <a href="#methodology">Methodology</a> •
  <a href="#examples">Examples</a>
</p>

## Dependencies

* [RAC Fuel Watch](https://www.rac.co.uk/drive/advice/fuel-watch/) (Accessed: 30 September 2022)
* [Department for Business, Energy and Industrial Strategy (BEIS) conversion factors for company reporting](https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting) (Accessed: 22 July 2022)

## Definition
Emissions associated with any travel completed by business-only vehicles owned or leased by the reporting organisation.

## Methodology

### Calculations: NHS Fleet & Leased vehicles

**Data map**

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Fuel card expenses (£) | X |  |  |
| Fuel card consumption (litres) |  | X |  |
|  |  |  |  |

**Reduced calculation: NHS Fleet & Leased vehicles**

*Equation 4.1* The RC approach for calculating emissions from NHS Fleet & Leased vehicles.

$$ 
\frac{\left( \frac{\text{F1Cost}}{\text{F1Price}} \times \text{F1Fac} \right) + \left( \frac{\text{F2Cost}}{\text{F2Price}} \times \text{F2Fac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* F*n*Cost = The total annual cost of the distinct fuel type (£) the first fuel type being denoted 'F1'.
* F*n*Price = The cost per litre of the distinct fuel type (£/litre), the first fuel type being denoted 'F1' .
* F*n*Fac = The carbon factor assigned to the distinct fuel by the relevant BEIS carbon factor database publication (CO<sub>2</sub>e/litre), the first fuel type being denoted 'F1'.

**Standard calculation: NHS Fleet & Leased vehicles**

*Equation 4.2* The SC approach for calculating emissions from NHS Fleet & Leased vehicles.

$$ 
\frac{\left(\text{F1Litres} \times \text{F1Fac} \right) + \left( \text{F2Litres} \times \text{F2Fac} \right) ... }
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* F*n*Litres = The annual quantity of the distinct fuel type consumed (litre), the first fuel type being denoted 'F1' .
* F*n*Fac = The carbon factor assigned to the distinct fuel by the relevant BEIS carbon factor database publication (CO<sub>2</sub>e/litre), the first fuel type being denoted 'F1'.

**Optimal calculation: NHS Fleet & Leased Vehicles**

> We're looking for contributors to this open, shared resource! Please check the [issues ticket](https://github.com/danwrisar/KMSIMG_NHS_EmissionsRecipeBook/issues/5) for this theme to get involved. 

## Examples

**Reduced calculation: NHS Fleet & Leased Vehicles**

Raul is able to source total cost of fuel for the year he is interested in from the relevant internal department. Crucially, he knows how much was spent per individual fuel, with £10,000 spent on unleaded fuel and £20,000 spent on diesel fuel. Raul uses a recognised source, such as the [RAC Fuel Watch database](https://www.rac.co.uk/drive/advice/fuel-watch/), to establish a cost per unit to enable him to extract the litres of fuel that correspond to the aforementioned total cost per fuel. In 2019, the cost of unleaded fuel was £1.2578 per litre while the cost of diesel fuel was £1.3117 per litre. 

By using the [BEIS Conversion Factors dataset for the year he is interested in (2019)](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2019), Raul is able to source a value for emissions per litre of unleaded fuel with an average biofuel blend (2.20904kgCO<sub>2</sub>e/litre) and per litre of diesel fuel with an average biofuel blend (2.59411kgCO<sub>2</sub>e/litre). Raul wants to report in tonnes, therefore divides the sum by 1,000 and rounds to two decimal places. Along with adding his units (tCO<sub>2</sub>e), Raul adds the [RC] tag to support transparency around how this figure was calculated. The final value added to Raul’s report on emissions associated with NHS Fleet & Leased Vehicles is 57.01tCO<sub>2</sub>e [RC].

*Equation 4.4* A worked example of emissions associated with NHS Fleet & Leased vehicles using an RC method.

$$ 
\frac{\left( \frac{\text{10000}}{\text{1.2578}} \times \text{2.19585} \right) + \left( \frac{\text{20000}}{\text{1.3117}} \times \text{2.59411} \right) ... }
{1000} = 57.01\text{tCO}_2\text{e} \text{ [RC]}
$$

**Standard calculation: NHS Fleet & Leased Vehicles**

Maxine has access to fuel cards records which state total quantities of distinct fuels purchased over the course of the year she is interested in. She knows that 20,000 litres of unleaded fuel were purchased and 10,000 litres of diesel fuel were purchased. By using the [BEIS Conversion Factors dataset for the year she is interested in (2019)](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2019), Maxine is able to source a value for emissions per litre of unleaded fuel with an average biofuel blend (2.19585kgCO<sub>2</sub>e/litre) and per litre of diesel fuel with an average biofuel blend (2.59411kgCO<sub>2</sub>e/litre). 

Maxine wants to report in tonnes, therefore divides the sum by 1,000 and rounds to two decimal places. Along with adding her units (tCO<sub>2</sub>e), Maxine adds the [SC] tag to support transparency around how this figure was calculated. The final value added to Maxine's report on emissions associated with NHS Fleet & Leased Vehicles is 69.86tCO<sub>2</sub>e [SC].

*Equation 4.5* A worked example of emissions associated with NHS Fleet & Leased vehicles using an SC method.

$$ 
\frac{\left(\text{20000} \times \text{2.19585} \right) + \left( \text{10000} \times \text{2.59411} \right) ... }
{1000} = 69.86\text{tCO}_2\text{e} \text{ [SC]}
$$

**Optimal calculation: NHS Fleet & Leased vehicles**

> We're looking for contributors to this open, shared resource! Please check the [issues ticket](https://github.com/danwrisar/KMSIMG_NHS_EmissionsRecipeBook/issues/5) for this theme to get involved. 
