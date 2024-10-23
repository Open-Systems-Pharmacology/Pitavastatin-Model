### 2.3.1 Absorption

The parameter value for  `Specific intestinal permeability`  was optimized based on clinical oral data, see results of optimization in [Section 2.3.4](#234-automated-parameter-identification). The solubility was obtianed from DrugBank (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data))

The dissolution of tablets was implemented via empirical Lint80 dissolution, according to Cho 2023 ([Cho 2024](#5-references)). 

### 2.3.2 Distribution

Pitavastatin is highly bound to plasma proteins (>99 %) (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)). A value of 0.52% was used in this PBPK model for `Fraction unbound (plasma, reference value)`. The major binding partner was set to albumin (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)).

An important parameter influencing the resulting volume of distribution is lipophilicity. The reported experimental logP values are in the range of 1.92-2.91 (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)) which served as a starting value. Finally, the model parameters `Lipophilicity` was optimized to match clinical data (see also [Section 2.3.4](#234-automated-parameter-identification)).

After testing the available organ-plasma partition coefficient and cell permeability calculation methods built in PK-Sim, observed clinical data was best described by choosing the partition coefficient calculation by `Rodgers and Rowland` and cellular permeability calculation by `Charge dependent Schmitt`.

### 2.3.3 Metabolism and Elimination

One metabolic pathway was implement into the model a first order process 

* Unspecific UGT
Metabolic enzyme activity is described as first order process

The unspecific UGT was set to only be expressed in the liver. Metabolic enzyme activity was set to be described as first order process, were the `CLspec/[Enzyme]` was optimized based on clinical data (see [Section 2.3.4](#234-automated-parameter-identification)).

And two transport protein was implemented into the model via Michaelis-Menten kinetics 

* OATP1B1

The OATP1B1 expression profiles is based on high-sensitive real-time RT-PCR ([Nishimura 2003](#5-references)). The reference concentration for OATP1B1 was measured by liquid chromatography tandem mass spectroscopy ([Prasad 2014](#5-references)). Transporter activity was described as saturable process following Michaelis-Menten kinetics, were the `Km` was taken from literature and the `kcat` was optimized based on clinical data (see [Section 2.3.4](#234-automated-parameter-identification)).

* BCRP

The BCRP expression profiles is based on Microarray expression data from ArrayExpress. The reference concentration for OATP1B1 was measured by liquid chromatography tandem mass spectroscopy ([Prasad 2013](#5-references)). Transporter activity was described as saturable process following Michaelis-Menten kinetics, were the `Km` was taken from literature and the `kcat` was optimized based on clinical data (see [Section 2.3.4](#234-automated-parameter-identification)).

Additionally, renal clearance was set to 0 according to literature (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)).


### 2.3.4 Automated Parameter Identification

The following parameters were optimized by fitting the model to the data:

| Model Parameter                |
| ------------------------------ | 
| `Lipophilicity`                | 
| `kcat` (OATP1B1)               |
| `CLspec/[Enzyme]` (OAT3)       |
| `kcat` (BCRP)                  |
| `Specific intestinal permeability`| 


 
