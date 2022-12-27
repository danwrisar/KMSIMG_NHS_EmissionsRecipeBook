# 03 Anaesthetics

<p align="center">
  <a href="#dependencies">Depedencies</a> •
  <a href="#definition">Definition</a> •
  <a href="#methodology">Methodology</a> •
  <a href="#examples">Examples</a>
</p>

## Dependencies
* [Association of Anaesthetists: The Real-Time Anaesthetic Gasses Calculator (Pierce, 2022)](https://anaesthetists.org/Home/Resources-publications/Environment/Guide-to-green-anaesthesia/Anaesthetic-gases-calculator) (Accessed: 27 December 2022)

## Definition
Emissions associated with the consumption of bottled and piped anaesthetic gasses including halothane, nitrous oxide, isoflurane, sevoflurane, and desflurane.

## Methodology

### Calculations: Anaesthetic gasses per cylinder

**Data map**

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
|  | |  |  |
| Purchasing logs (litres) |  | X |  |
|  |  |  |  |

**Standard calculation: Bottled anaesthetic gasses**

*Equation 3.2* The SC approach for emissions associated with anaesthetic gasses per cylinder.

$$ 
\frac{\text{GasNomCap} \times \text{GasDen} \times \text{GloWarm}}{1000}
=  \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* GasNomCap = Total nominal capacity of the gas containers (litres).
* GasDen = Density of the gas (kg/litre).
* GloWarm = Global warming potential of the gas.

## Calculations: Anaesthetic gasses by flow

### Data map

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Estimated use (hours) | X |  |  |
| Logged use (hours |  | X |  |
|  |  |  |  |

**Reduced calculation: Anaesthetic gasses by flow**

*Equation 3.4* The RC approach for emissions associated with anaesthetic gasses measured by flow.

$$ 
\frac{\text{EstHours} \times \text{RTImpact}}{1000}
=  \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* EstHours = Estimated duration of gas flow over period (hours).
* RTImpact = Relevant emissions per hour approximated by the *Real-Time Anaesthetic Gasses Calculator* (kgCO<sub>2</sub>e/hr).

**Standard calculation: Anaesthetic gasses by flow**

*Equation 3.5* The SC approach for emissions associated with anaesthetic gasses per cylinder.

$$ 
\frac{\text{LoggedHours} \times \text{RTImpact}}{1000}
=  \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* LoggedHours = Recorded duration of gas flow over period (hours).
* RTImpact = Relevant emissions per hour approximated by the *Real-Time Anaesthetic Gasses Calculator* (kgCO<sub>2</sub>e/hr).

## Examples

**Standard Calculation: Anaesthetic gasses per cyclinder**

Karl sources purchase logs from his procurement contact for bottled nitrous oxide gas. From this data he is able to identify the capacity of the bottles purchased and the number of bottles purchased. He finds that 25 bottles of nitrous oxide gas had been purchased, each with a nominal capacity of 1,800 litres (45,000 litres of capacity in total across the 25 bottles). Karl obtains a value for density of nitrous oxide from a reputable source, such as the [CRC Handbook of Chemistry and Physics](https://hbcp.chemnetbase.com/faces/contents/ContentsSearch.xhtml) which states the density of nitrous oxide as 0.0018kg/l.

Karl refers to a verified source, such as [The Association of Anaesthetists](https://anaesthetists.org/Home/Resources-publications/Environment/Guide-to-green-anaesthesia/Anaesthetic-gases-calculator) website, for a global warming potential figure for nitrous oxide (310). He wants to report in tonnes, therefore divides the sum by 1,000 and rounds to two decimal places. 

Along with adding his units (tCO<sub>2</sub>e), Karl adds the [SC] tag to support transparency around how this figure was calculated using a reduced data calculation method. The final value added to Karl’s report on emissions associated with natural gas consumption was 167.55tCO<sub>2</sub>e [SC].

*Equation 3.9* A worked example of an SC calculation of emissions associated with natural gas consumption.

$$ 
\frac{\left( 45000 \times 0.0018 \times 310 \right)}{1000}
=  25.11 \text{tCO}_2\text{e} \text{ [SC]}
$$
