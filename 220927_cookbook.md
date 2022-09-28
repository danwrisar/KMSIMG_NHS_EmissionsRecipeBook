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

To do list

* (1) Fossils fuels: Liquid fuels RC, SC and OC
* (1) Fossil fuels: Solid fuels RC, SC and OC
* (2) NHS Facilities RC, SC and OC
* (3) Anaesthetics: Bottled gas RC and OC
* (3) Anaesthetics: Piped gas RC, SC and OC

## 1. Fossil fuels

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

*Equation 1.1* The RC approach for natural gas consumption.

$$ 
\frac{\left( \text{ModCon} \times \text{A} \right) \times \text{Fac}}
{1000} = \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* ModCon = Value of modelled annual energy use (kWh/m<sup>2</sup>) from the relevant Display Energy Certificate.
* A = Value of total useful floor area (m<sup>2</sup>) from the relevant Display Energy Certificate.
* Fac = Carbon factor assigned to the fuel by the relevant BEIS carbon factor database publication.

**Standard calculation**

*Equation 1.2* The SC approach for natural gas consumption.

$$ 
\frac{\text{EstMonCon} \times \text{Fac}}
{1000} = \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* EstMonCon = Value of monitored annual energy use (kWh) where ≥11% of data are estimated.
* Fac = Carbon factor assigned to the fuel by the relevant BEIS carbon factor database publication.  

**Optimal calculation**

*Equation 1.3* The OC approach for natural gas consumption.

$$ 
\frac{\text{MonCon} \times \text{Fac}}
{1000} = \text{tCO}_2\text{e} \text{ [OC]}
$$

Where:
* MonCon = Value of monitored annual energy use (kWh) where ≤10% of data are estimated.
* Fac = Carbon factor assigned to the fuel by the relevant DEFRA or BEIS carbon factor database publication.  

### Examples

**Reduced Data Calculation**

Stu sources the Display Energy Certification (DEC) for the building he is interested in. Using information from the Building Energy Use figure (Figure 1.1), Stu multiplies the annual energy use of other fuels (328) by the total useful floor area for the building (2778.54). The calculated annual total consumption (911,361.12) is presented in kWh. 

By using the BEIS Carbon Factors  for the year he is interested in (2019), Stu was able to source a value for emissions per kWh of natural gas use assuming gross calorific value (0.18385kgCO<sub>2</sub>e/kWh). Stu wanted to report in tonnes, therefore divided the sum by 1,000. This value was then rounded to 2 decimal places. 
Along with adding their units (tCO<sub>2</sub>e), Stu added the [RC] tag to support transparency around how this figure was calculated using a reduced data calculation method. The final value added to Stu’s report on emissions associated with natural gas consumption was 167.55tCO<sub>2</sub>e [RC].

E*quation 1.4* A worked example of an RDC calculation of emissions associated with natural gas consumption.

$$ 
\frac{\left( 328 \times 2778.54 \right) \times 0.18385}
{1000} = 167.55\text{tCO}_2\text{e} \text{ [RC]}
$$

![Example of a Display Energy Certificate](Images/DECExample.png)

*Figure 1.1* Example of data sourced from a Display Energy Certificate.

**Standard Calculation**

Julia receives confirmation from their energy supplier that the site they are interested in used 100,000kWh of natural gas. The supplier also indicated that for the four months preceding the end of the period being assessed were estimated meter reads (Figure 1.2). Therefore, it is suggested that 33% of the data underlying the period total consumption were estimated, and therefore necessary to use the Standard Calculation methodology.

Using the BEIS Carbon Factors  for the year they are interested in (2019), Julia was able to source a value for emissions per kWh of natural gas use, assuming gross calorific value (0.18385kgCO<sub>2</sub>e/kWh). Julia wanted to report in tonnes, therefore divided the sum by 1,000. This value was then rounded to 2 decimal places.  Along with adding their units (tCO<sub>2</sub>e), Julia made sure to add the [SC] tag to support transparency around how this figure was calculated. The final value added to Julia’s annual report was 18.39tCO<sub>2</sub>e [SC].

E*quation 1.5* A worked example of an RDC calculation of emissions associated with natural gas consumption.

$$ 
\frac{100000 \times 0.18385}
{1000} = 18.39\text{tCO}_2\text{e} \text{ [SC]}
$$

![Visualisation of estimated compared to actual consumption](Images/EstimatedMeterReads.png)

*Figure 1.2* A visualisation of actual and estimated electrical consumption.

**Optimal Calculation**

Jo receives confirmation from their energy supplier that the site they are interested in used 200,000kWh of natural gas. The supplier provides access to data from an installed Automated Meter Reader (AMR) and the assessor was able to spot three weeks where no gas was being consumed unexpectedly. As such, data were missing for four weeks of a total 48 (for sake of demonstration), equalling 8.33% of estimated or missing data and 91.67% of verified or intact data. It was therefore possible to use the Optimal Calculation methodology.

Using the BEIS Carbon Factors  for the year they are interested in (2019), Jo was able to source a value for emissions per kWh of natural gas use, assuming gross calorific value (0.18385kgCO<sub>2</sub>e/kWh). Jo wanted to report in tonnes, therefore divided the sum by 1,000. This value was then rounded to 2 decimal places. Along with adding their units (tCO<sub>2</sub>e), Julia made sure to add the [OC] tag to support transparency around how this figure was calculated. The final value added to Julia’s annual report was 36.77tCO<sub>2</sub>e [OC].

*Equation 1.6* A worked example of an RDC calculation of emissions associated with natural gas consumption.

$$ 
\frac{200000 \times 0.18385}
{1000} = 36.77\text{tCO}_2\text{e} \text{ [OC]}
$$

![Visualisation of estimated compared to actual consumption](Images/AMRMeterReads.png)

*Figure 1.3* A visualisation of actual and estimated electrical consumption split per week (simplified to 48 weeks across 12 months for demonstration purposes).

## 2. Anaesthetics

### Definition
Emissions associated with the consumption of bottled and piped anaesthetic gasses including halothane, nitrous oxide, isoflurane, sevoflurane, and desflurane.

### Data map

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
|  |  |  |  |
| Consumption logs  |  | X |  |
|  |  |  |  |

### Calculations: Bottled anaesthetic gasses

**Reduced calculation**

*Equation 2.1* The RC approach for bottled anaesthetic gasses.

[To complete]

**Standard calculation**

*Equation 2.2* The SC approach for bottled anaesthetic gasses.

$$ 
\frac{\left( \text{GasNomCap} \times \text{GasDen} \times \text{GloWarm} \right)}{1000}
=  \text{tCO}_2\text{e} \text{ [SC]}
$$

Where:
* GasNomCap = Total nominal capacity of the gas containers (litres).
* GasDen = Density of the gas (kg/litre).
* GloWarm = Global warming potential of the gas.

**Optimal calculation**

*Equation 2.3* The OC approach for bottled anaesthetic gasses.

[To complete]

#### Examples: Bottled anaesthetic gasses

**Reduced Data Calculation**

[To complete]

**Standard Calculation**

Karl sources purchase logs for bottled nitrous oxide gas. From this data he is able to identify the capacity of the bottles purchased and the number of bottles purchased. He found that 250 bottles of nitrous oxide gas had been purchased, each with a liquid capacity of 20 litres. Therefore, total liquid capacity of the containers was 5,000 litres.

Karl refers to the  for a value for global warming potential of nitrous oxide

By using the BEIS Carbon Factors  for the year he is interested in (2019), Stu was able to source a value for emissions per kWh of natural gas use assuming gross calorific value (0.18385kgCO<sub>2</sub>e/kWh). Stu wanted to report in tonnes, therefore divided the sum by 1,000. This value was then rounded to 2 decimal places. 
Along with adding their units (tCO<sub>2</sub>e), Stu added the [RC] tag to support transparency around how this figure was calculated using a reduced data calculation method. The final value added to Stu’s report on emissions associated with natural gas consumption was 167.55tCO<sub>2</sub>e<sub> [RC]</sub>.

E*quation 1.4* A worked example of an RDC calculation of emissions associated with natural gas consumption.

$$ 
\frac{\left( 328 \times 2778.54 \right) \times 0.18385}
{1000} = 167.55\text{tCO}_2\text{e}_\text{ [RC]}
$$

*Equation 3.5* A worked example of an RDC calculation of emissions associated with natural gas consumption.

$$ 
\frac{100000 \times 0.18385}
{1000} = 18.39\text{tCO}_2\text{e}_\text{ [SC]}
$$

**Optimal Calculation**

[To complete]

### Calculations: Piped anaesthetic gas

**Reduced calculation**

*Equation 3.7* The RC approach for piped anaesthetic gasses.

[To complete]

**Standard calculation**

*Equation 3.8* The SC approach for piped anaesthetic gasses.

[To complete]

**Optimal calculation**

*Equation 3.9* The OC approach for piped anaesthetic gasses.

[To complete]