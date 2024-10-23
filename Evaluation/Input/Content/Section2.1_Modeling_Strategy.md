The general concept of building a PBPK model has previously been described by Kuepfer et al. ([Kuepfer 2016](#5-references)). Relevant information on anthropometric (height, weight) and physiological parameters (e.g. blood flows, organ volumes, binding protein concentrations, hematocrit, cardiac output) in adults was gathered from the literature and has been previously published ([Willmann 2007](#5-references)). The information was incorporated into PK-Sim® and was used as default values for the simulations in adults.

The applied activity and variability of plasma proteins and active processes that are integrated into PK-Sim® are described in the publicly available PK-Sim® Ontogeny Database Version 7.3 ([PK-Sim Ontogeny Database Version 7.3](#5-references)) or otherwise referenced for the specific process.

A mean model was built based on clinical data from studies with intravenous and oral administration of pitavastatin by Mori 2020 ([Mori 2020](#5-references)), Takehara 2018 ([Takehara 2018](#5-references)), Lou 2015 ([Lou 2015](#5-references)), Kimoto 2022 ([Kimoto 2022](#5-references)), Chen 2013 ([Chen 2013](#5-references)) and Prueksaritanont 2014 ([Prueksaritanont 2014](#5-references)). The studies reported mean plasma concentrations of pitavastatin. The mean PBPK model was developed using a mean individual based on the demographic data for each study and if no demographic data were provided the following values were used; male, European, 30 years of age, 73 kg body weight and 176 cm body height. The relative tissue-specific expressions of the enzyme and transporter predominantly being involved in the metabolism/transport of pitavastatin (OATP1B1 and BCRP) were considered ([Meyer 2012](#5-references)). A Lint80 function with 80% of tablet dissolved in 30 minutes were applied according to Cho 2024 ([Cho 2024](#5-references)). 

Due to the large inter-study variability of pitavastatin plasma concentration, a large part of the available clinical data was used for model building.

A specific set of parameters (see below) was optimized to describe the disposition of pitavastatin using the Parameter Identification module provided in PK-Sim®. Structural model selection was mainly guided by visual inspection and total error of the resulting description of data, 95% confidence interval of the identified parameter values and biological plausibility.

The model was then verified by simulating further clinical studies reporting pharmacokinetic concentration-time profiles after oral administration of pitavastatin in individuals with different SLCO1B1 genotypes.

Details about input data (physicochemical, *in vitro* and clinical) can be found in [Section 2.2](#22-data-used).

Details about the structural model and its parameters can be found in [Section 2.3](#23-model-parameters-and-assumptions).




