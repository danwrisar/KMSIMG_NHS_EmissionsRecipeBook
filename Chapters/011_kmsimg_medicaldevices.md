# 11 Medical devices

<p align="center">
  <a href="#dependencies">Dependencies</a> •
  <a href="#definition">Definition</a> •
  <a href="#methodology">Methodology</a> •
  <a href="#examples">Examples</a>
</p>

## Dependencies

* [Official statistics: UK and England's carbon footprint to 2019 - UK full dataset 1990 - 2019, including conversion factors by SIC code (Department for Environment, Food and Rural Affairs, 2022)](https://www.gov.uk/government/statistics/uks-carbon-footprint) (Accessed 27 December 2022)

## Definition

Emissions associated with the manufacture, operation and disposal of medical devices integral to the diagnosis, treatment, support and care of patients.

## Methodology

**Data map**

| Description of data available  | Reduced calculation [RC]  | Standard calculation [SC] | Optimal Calculation [OC] |
| ------------------------------ |:---:| :---:| :---:|
| Per category purchasing (£) | X |  |  |
| Per supplier purchasing (£) |  | X |  |
| Supplier verification |  |  | X |

**Reduced calculation: Medical devices**

*Equation 11.1* The RC approach for calculating emissions associated with procurement of medical devices.

$$\frac{\left( \text{MedDev1Spend} \times \text{MedDev1Factor} \right) + \left( \text{MedDev2Spend} \times \text{MedDev2Factor} \right) ...}
{1000} = \text{tCO}_2\text{e} \text{ [RC]}$$

Where:
* MedDev*n*Spend = The spend on an element (e.g. x-ray machine purchase) mapped to the theme of medical devices (£).
* MedDev*n*Factor = The weighting assigned to the element through the Standard Industrial Code (SIC) multipliers tab in the relevant [DEFRA emissions dataset](https://www.gov.uk/government/statistics/uks-carbon-footprint) mapped to the theme of medical devices (kgCO<sub>2</sub>e/£). 

**Standard calculation: Medical devices**

*Equation 11.2* The SC approach for calculating emissions associated with procurement of medical devices.

$$ 
\frac{\left( \text{MedDev2Spend} \times \text{MedDev1Factor} \right) + \left( \text{MedDev2Spend} \times \text{MedDev2Factor} \right) ...}
{1000} = \text{tCO}_2\text{e} \text{ [RC]}
$$

Where:
* MedDevSupplier*n*Spend = The spend per supplier with an assigned Standard Industrial Code (SIC) mapped to the theme of medical devices (£).
* MedDevSupplier*n*Factor = The weighting assigned to the element through the Standard Industrial Code (SIC) multipliers tab in the relevant [DEFRA emissions dataset](https://www.gov.uk/government/statistics/uks-carbon-footprint) mapped to the theme of medical devices (kgCO<sub>2</sub>e/£). 

**Optimal calculation: Medical devices**

See the <a href="#examples">example</a> for optimal calculation of emissions associated with procurement of medical devices in collaboration with suppliers.

## Examples

**Reduced calculation: Medical devices**

*Equation X.1* The RC approach for XXXXXX.

$$\frac{\left( \text{ModCon} \times \text{A} \right) \times \text{Fac}}
{1000} = \text{tCO}_2\text{e} \text{ [RC]}$$

Where:
* XXX = XXX

**Standard calculation: Medical devices**

**Optimal calculation: Medical devices**

> To achieve a denotation an optimal calculation of emissions associated with the procurement of medical devices, it is necessary to obtain verified impacts from suppliers. The estimated value(s) acquired through the standard calculation approach offers a valuable means to initiate and progress conversations with suppliers with the objective of obtaining a more accurate footprint associated with purchasing from a supplier. Should a supplier be unable to verify, this offers opportunities for introduction of specific key performance indicators in future contract negotations or re-tenders for services and/or products.

Sandra follows the standard calculation approach to acquire a value for emissions associated with spend on medical devices at a supplier called *Mick's Dental Bazaar* (10.2tCO<sub>2</sub>e). Sandra works with her procurement colleagues to understand the nature of the purchase, such as whether there is a contract in place, and if so, if there may be any pertinent key performance indicators and if the contract may be upcoming for renewal.

With support as necessary from her procurement colleagues, Sandra contacts the account manager, or relevant contact, at *Mick's Dental Bazaar* to share the findings of her emission estimation with the objective of obtain verification for tje

Can *Mick's Dental Bazaar* verify that 10.2tCO<sub>2</sub>e is a reasonable estimation for emissions associated with the spend?

If YES:

IF NO:

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

```flow
st=>start: Start
op=>operation: Your Operation
cond=>condition: Yes or No?
e=>end

st->op->cond
cond(yes)->e
cond(no)->op
```

* Can *Mick's Dental Bazaar* provide a more accurate estimation of estimation for emissions associated with the spend?

If the estimation value is agreed...


If the estimation value is not agreed...
