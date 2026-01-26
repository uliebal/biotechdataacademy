---
title: "Flux Simulations with Genome Scale Models"
date: 2025-01-19
draft: false

---
{{<toc>}}
<!-- 
####################################################
Introduction
####################################################
 -->
## Introduction

Cells grow because the metabolic network converts substrates into energy and buildings blocks for new cells. The conversions takes place via stepwise modifications of the metabolites by the activity of enzymes. Graphically, metabolites are shown as vertices and reactions as connecting arrows. Subdivisions of the metabolic network yield metabolic pathways, which serve certain physiological requirements, like energy production via oxidative phosphorylation, carbon fixation or fatty acid synthesis (see figure below). Eventually, all components necessary for life, and not available from the environment, are synthesized in an organisms metabolic network.

<!-- Figure Growth and Substrate Rates -->
{{< figure src="/images/Tutorials/GSMMSims/Metabolic_Metro_Map.svg" caption="Visualization of metabolic pathways forming a metabolic network ([Chakazul, Wikimedia Commons](https://en.wikipedia.org/wiki/File:Metabolic_Metro_Map.svg))." numbered="true" width="800" position="center" command="fill" option="q100" class="img-fluid" webp="false" >}}

Metabolic networks differ between organisms based on their environment. Organisms adapted to a resource rich and stable environments, like *Mycoplasma genitalium* adapted to human niches, have few enzymes and a small metabolic network because required compounds are derived externaly [Wikipedia](https://en.wikipedia.org/wiki/Mycoplasma_genitalium). Organisms in poor and changing environments have larger metabolic capacities [Reference needed]. 


<a class="btn btn-primary" href="/Example_GrowthExp.xlsx" download>
  Download Excel: Growth data
</a>

<!-- 
####################################################
Computational
####################################################
 -->

## Computational preparations

### Python packages

The data analysis is based on widely available Python packages. It also requires a package called iambcodes, which can be downloaded by PyPi and provides customized nonlinear fit functions.

{{< accordion "Python Code" >}}
```python
```
{{< /accordion >}}

### Filesystem & parameters

The following code cell defines data file for analysis and sets the paths and figure file type of the results. Some general parameters for the conversion of mole to gramm are provided and the visualization of the "\(\pm\)" sign.

{{< accordion "Python Code" >}}
```python
```
{{< /accordion >}}

### Data import
In the example file above, the sheet '10mM' contains measurements for additional metabolites 

<!-- Figure Excel Standard Single-->
{{< figure src="/images/Tutorials/CarbonBalance/ExcelStandardFormat.svg" caption="Standard format for data table sheet as xlsx-file type." numbered="true" width="1200">}}

{{< accordion "Python Code" >}}
```python
```
{{< /accordion >}}

### Data selection
Using the Excel Worksheet names, we select the data that we want to analyze with the variable 
{{< accordion "Python Code" >}}
```python
```
{{< /accordion >}}



## Summary
Overall, the actual rates from the original simulation could be well estimated. The constant RQ shows that the metabolism is constant throughout the simulation and its lower value indicates the existence of organic acid byproducts. The carbon and electron balances calculation result in 7% imbalances that occur in data even when experimental noise is deactivated. The reason is that the growth rate is slightly overestimated, probably because the biomass estimation on the basis of the logistic growth equation with a maximum biomass capacity in the model does not optimally capture the decrease of growth rate due to substrate depletion.