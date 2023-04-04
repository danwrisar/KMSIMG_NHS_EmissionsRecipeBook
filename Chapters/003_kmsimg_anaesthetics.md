# 03 Anaesthetics

<p align="center">
  <a href="#dependencies">Dependencies</a> •
  <a href="#definition">Definition</a> •
  <a href="#methodology">Methodology</a> •
  <a href="#examples">Examples</a>
</p>

## Dependencies
* [Association of Anaesthetists: The Real-Time Anaesthetic Gasses Calculator (Pierce, 2022)](https://anaesthetists.org/Home/Resources-publications/Environment/Guide-to-green-anaesthesia/Anaesthetic-gases-calculator) (Accessed: 27 December 2022)

## Definition
Emissions associated with the consumption of cylinder and piped anaesthetic gasses including halothane, nitrous oxide, mixed nitrous oxide, isoflurane, sevoflurane, and desflurane.

## Methodology

### Calculations: Anaesthetic gasses per cylinder

**Data map**

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Greener NHS Dashboard | X |  |  |
| Cylinder purchasing logs  |  | X |  |
| Number of expired cylinders returned to supplier |  |  | X |
| Number of cylinders stolen/lost |  |  | X |

**Reduced calculation: Anaesthetic gasses (by cylinder)**

See the <a href="#examples">example</a> for reduced calculation of emissions associated with purchase of anaesthetic gasses through use of the Greener NHS Dashboard.

**Standard calculation: Anaesthetic gasses (by cylinder)**

*Equation 3.2* The SC approach for calcualting emissions associated with anaesthetic gasses per cylinder.

$$ 
\frac{\text{GasNomCap} \times \text{GasDen} \times \text{GloWarm}}{1000}
=  \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* GasNomCap = Total nominal capacity of the gas containers (litres).
* GasDen = Density of the gas (kg/litre).
* GloWarm = Global warming potential of the gas.

**Optimal calculation: Anaesthetic gasses (by cylinder)**

*Equation 3.3* The OC approach for calculating emissions associated with anaesthetic gasses per cylinder.

$$ 
\frac{\left(\text{GasNomCap - ExpiredNomCap - LostNomCap} \right) \times \text{GasDen} \times \text{GloWarm}}{1000}
=  \text{tCO}_2\text{e} \text{ [OC]}
$$

Where:
* GasNomCap = Total nominal capacity of the gas containers (litres).
* ExpiredNomCap = Total nominal capacity of the expired gas containers expired that were returned to the supplier (litres).
* LostNomCap = Total nominal capacity of the gas containers that were stolen or lost (litres).
* GasDen = Density of the gas (kg/litre).
* GloWarm = Global warming potential of the gas.

## Examples

**Reduced calculation: Anaesthetic gasses (per cylinder)**

Jerome is intersted in understanding sevoflurane emissions associated with the provider trust he works for. As an NHS colleague, Jerome is able to register for access to the Greener NHS Knowledge Hub available on the [NHS Futures](https://future.nhs.uk/system/home?done=) platform. Jerome navigates to the 'Resources and Tools' section of the [Greener NHS Knowledge Hub](https://future.nhs.uk/sustainabilitynetwork/groupHome), clicks through to the 'Data and Analytics' page and registers to use the Greener NHS Dashboard. 

This dashboard features a record of 'volatile anaesthetic gasses' per region and per trust. Jerome selects his trust and filters by an annual view to source a figure for the rolling average emissions associated with sevoflurane use in the financial year he is interested in, for example, from April 2022 to March 2023. Jerome sources a figure of 92.08 for carbon equivalent emissions associated with use of sevoflurane. In addition to adding his units (tCO<sub>2</sub>e), Jerome adds the [RC] tag to support transparency around how this figure was calculated using a reduced data calculation method. The final value added to Jerome’s report on emissions associated with sevoflurane use is 92.08tCO<sub>2</sub>e [RC].

**Standard calculation: Anaesthetic gasses (per cylinder)**

Karl sources purchase logs from his procurement contact for cylinderd nitrous oxide gas. From this data he is able to identify the capacity of the cylinders purchased and the number of cylinders purchased. He finds that 25 cylinders of nitrous oxide gas had been purchased, each with a nominal capacity of 1,800 litres (45,000 litres of capacity in total across the 25 cylinders). Karl obtains a value for density of nitrous oxide from a reputable source, such as the [CRC Handbook of Chemistry and Physics](https://hbcp.chemnetbase.com/faces/contents/ContentsSearch.xhtml) which states the density of nitrous oxide as 0.0018kg/l.

Karl refers to a verified source, such as [The Association of Anaesthetists](https://anaesthetists.org/Home/Resources-publications/Environment/Guide-to-green-anaesthesia/Anaesthetic-gases-calculator) website, for a global warming potential figure for nitrous oxide (310). He wants to report in tonnes, therefore divides the sum by 1,000 and rounds to two decimal places. Along with adding his units (tCO<sub>2</sub>e), Karl adds the [SC] tag to support transparency around how this figure was calculated using a standard data calculation method. The final value added to Karl’s report on emissions associated with nitrous oxide consumption is 25.11tCO<sub>2</sub>e [SC].

*Equation 3.5* A worked example of an SC approach for calculating emissions associated with anaesthetic gasses per cylinder.

$$ 
\frac{\left( 45000 \times 0.0018 \times 310 \right)}{1000}
=  25.11 \text{tCO}_2\text{e} \text{ [SC]}
$$

**Optimal calculation: Anaesthetic gasses (per cylinder)**

Juliana wants to better understand emissions associated with mixed nitrous oxide (also known as Entonox) and requests procurement information for cylinder mixed nitrous oxide gas, registers logging any returned expired cylinders and any recorded thefts over the period of interest. From this data she is able to identify the capacity of the cylinders purchased, the number of cylinders purchased, the number of expired cylinders that were returned without being used and the number of cylinders that were lost or stolen. She finds that 50 cylinders of mixed nitrous oxide gas had been purchased, each with a nominal capacity of 1,800 litres (90,000 litres of capacity in total across the 50 cylinders). Juliana also receives the information that two cylinders were returned to the supplier as they expired while in storage (3,600 litres of capacity from two cylinders) and that three cylinders were noted as being unaccounted for, potentially due to theft (5,400 litres of capacity from three cylinders). Juliana obtains a value for density of nitrous oxide from a reputable source, such as the [CRC Handbook of Chemistry and Physics](https://hbcp.chemnetbase.com/faces/contents/ContentsSearch.xhtml) which states the density of nitrous oxide as 0.0018kg/l.

Juliana refers to a verified source, such as [The Association of Anaesthetists](https://anaesthetists.org/Home/Resources-publications/Environment/Guide-to-green-anaesthesia/Anaesthetic-gases-calculator) website, for a global warming potential figure for nitrous oxide (310). She wants to report in tonnes, therefore divides the sum by 1,000 and rounds to two decimal places. 

Along with adding her units (tCO<sub>2</sub>e), Juliana adds the [OC] tag to support transparency around how this figure was calculated using an optimal data calculation method. The final value added to Juliana’s report on emissions associated with mixed nitrous oxide consumption is 45.20tCO<sub>2</sub>e [SC].

*Equation 3.6* A worked example of an OC approach for calculating emissions associated with anaesthetic gasses per cylinder.

$$ 
\frac{\left(\text{90,000 - 3,600 - 5,400} \right) \times \text{0.0018} \times \text{310}}{1000}
=  \text{tCO}_2\text{e} \text{ [OC]}
$$