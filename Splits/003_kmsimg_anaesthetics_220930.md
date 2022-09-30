# 03 Anaesthetics

[Kent and Medway Sustainability: NHS Emissions Cookbook]

**Authors**:
  Dan Wright<sup>1</sup>

1. Kent Community Health NHS Foundation Trust

## Introduction

### Dependencies

### Acknowledgements

### To do list

* Anaesthetics: Bottled gas RC and OC
* Anaesthetics: Piped gas RC, SC and OC

## Methodology

### Definition
Emissions associated with the consumption of bottled and piped anaesthetic gasses including halothane, nitrous oxide, isoflurane, sevoflurane, and desflurane.

### Data map

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
|  |  |  |  |
| Consumption logs  |  | X |  |
|  |  |  |  |

### Calculations: Bottled anaesthetic gasses

**Standard calculation**

*Equation 3.2* The SC approach for bottled anaesthetic gasses.

$$ 
\frac{\left( \text{GasNomCap} \times \text{GasDen} \times \text{GloWarm} \right)}{1000}
=  \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* GasNomCap = Total nominal capacity of the gas containers (litres).
* GasDen = Density of the gas (kg/litre).
* GloWarm = Global warming potential of the gas.

#### Examples: Bottled anaesthetic gasses

**Standard Calculation**

Karl sources purchase logs for bottled nitrous oxide gas. From this data he is able to identify the capacity of the bottles purchased and the number of bottles purchased. He found that 25 bottles of nitrous oxide gas had been purchased, each with a nominal capacity of 1,800 litres. Therefore, total liquid capacity of the containers was 45,000 litres. Karl obtains a value for density of nitrous oxide from a reputable source, such as the CRC Handbook of Chemistry and Physics by Haynes et al. (2011) which states the density of nitrous oxide as 0.0018kg/l.

Karl refers to a verified source, such as [The Association of Anaesthetists](https://anaesthetists.org/Home/Resources-publications/Environment/Guide-to-green-anaesthesia/Anaesthetic-gases-calculator) website, for a global warming potential figure for nitrous oxide (310). He wants to report in tonnes, therefore divides the sum by 1,000. This value was then rounded to 2 decimal places. 
Along with adding his units (tCO<sub>2</sub>e), Karl added the [SC] tag to support transparency around how this figure was calculated using a reduced data calculation method. The final value added to Stu’s report on emissions associated with natural gas consumption was 167.55tCO<sub>2</sub>e [RC].

Equation 3.5* A worked example of an RDC calculation of emissions associated with natural gas consumption.

$$ 
\frac{\left( 45000 \times 0.0018 \times 310 \right)}{1000}
=  25.11 \text{tCO}_2\text{e} \text{ [SC]}
$$