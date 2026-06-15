### 2.3.1 Absorption

The parameter value for  `Specific intestinal permeability`  was optimized based on clinical oral data, see results of optimization in [Section 2.3.4](#234-automated-parameter-identification). The solubility was obtained from DrugBank (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data))

The dissolution of tablets was implemented via empirical Lint80 dissolution, according to Cho 2024 ([Cho 2024](#5-references)). 

### 2.3.2 Distribution

Pitavastatin is highly bound to plasma proteins (>99 %) (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)). A value of 0.52% was used in this PBPK model for `Fraction unbound (plasma, reference value)`. The major binding partner was set to albumin (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)).

An important parameter influencing the resulting volume of distribution is lipophilicity. The reported experimental logP values are in the range of 1.92-2.91 (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)) which served as a starting value. Finally, the model parameter `Lipophilicity` was optimized to match clinical data (see also [Section 2.3.4](#234-automated-parameter-identification)).

After testing the available organ-plasma partition coefficient and cell permeability calculation methods built in PK-Sim, observed clinical data was best described by choosing the partition coefficient calculation by `Rodgers and Rowland` and cellular permeability calculation by `Charge dependent Schmitt`.

### 2.3.3 Metabolism and Elimination

One metabolic pathway was implemented into the model as a first order process:

* **Unspecified UGT**: The unspecified UGT was set to only be expressed in the liver. Metabolic enzyme activity was described as a first order process, where the `CLspec/[Enzyme]` was optimized based on clinical data (see [Section 2.3.4](#234-automated-parameter-identification)).

Two transport proteins were implemented into the model via Michaelis-Menten kinetics:

* **OATP1B1/1B3**: The OATP1B1 expression profiles are based on high-sensitivity real-time RT-PCR ([Nishimura 2003](#5-references)). The reference concentration for OATP1B1 was measured by liquid chromatography tandem mass spectroscopy ([Prasad 2014](#5-references)), i.e. not according to the default implementation in PK-Sim. Transporter activity was described as a saturable process following Michaelis-Menten kinetics, where the `Km` was taken from literature and the `kcat` was optimized based on clinical data (see [Section 2.3.4](#234-automated-parameter-identification)).

* **BCRP**: The BCRP expression profiles are based on Microarray expression data from ArrayExpress. The reference concentration for BCRP was measured by liquid chromatography tandem mass spectroscopy ([Prasad 2013](#5-references)), i.e. not according to the default implementation in PK-Sim. Transporter activity was described as a saturable process following Michaelis-Menten kinetics, where the `Km` was taken from literature and the `kcat` was optimized based on clinical data (see [Section 2.3.4](#234-automated-parameter-identification)).

Additionally, renal clearance was set to 0 according to literature (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)).


### 2.3.4 Automated Parameter Identification

The following parameters were optimized by fitting the model to the data:

| Model Parameter                |
| ------------------------------ | 
| `Lipophilicity`                | 
| `kcat` (OATP1B1)               |
| `CLspec/[Enzyme]` (UGT)        |
| `kcat` (BCRP)                  |
| `Specific intestinal permeability`| 


 
