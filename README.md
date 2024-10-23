# Pitavastatin-Model
Whole-body PBPK model of pitavastatin.

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c8/Pitavastatin.svg/2560px-Pitavastatin.svg.png" alt="File:Pitavastatin.svg" style="zoom:50%;" />

This pitavastatin model is intended to be used as a victim drug in OATP1B1-mediated drug-drug interactions (DDI).

This whole-body PBPK model of pitavastatin has been developed using published pharmacokinetic clinical data by Mori 2020 [[1](#references)], Takehara 2018 [[2](#references)], Lou 2015 [[3](#references)], Kimoto 2022 [[4](#references)], Chen 2013 [[5](#references)] and Prueksaritanont 2014 [[6](#references)]. 
The model has then been evaluated by simulating clinical studies and comparing with respective observed data. 

The presented model includes the following features:

- metabolism by unspecified UGT enzym present in the liver,
- transport by OATP1B1/B3,
- transport by BCRP
- no renal clearance by glomerular filtration,
- oral absorption with dissolution rate assigned to the Lint80 function.



## Repository files
This repository contains:

- a [PK-Sim snapshot (*.json) file](https://docs.open-systems-pharmacology.org/working-with-pk-sim/pk-sim-documentation/importing-exporting-project-data-models#exporting-project-to-snapshot-loading-project-from-snapshot) of the current PBPK model
- static content (e.g. text blocks, *.md files) as inputs for an evaluation plan
- an evaluation plan (evaluation-plan.json) to create an evaluation report using the snapshot and static text blocks to display the performance of the model

**The latest release of the snapshot of the model, the evaluation plan and the static content can be found [here](../../releases/latest).**

**The latest release of the PK-Sim project model file and the respective evaluation report can be found [here](https://github.com/Open-Systems-Pharmacology/OSP-PBPK-Model-Library/releases/latest).**

## Code of conduct
Everyone interacting in the Open Systems Pharmacology community (codebases, issue trackers, chat rooms, mailing lists etc...) is expected to follow the Open Systems Pharmacology [code of conduct](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODE_OF_CONDUCT.md#contributor-covenant-code-of-conduct).

## Contribution
We encourage contribution to the Open Systems Pharmacology community. Before getting started please read the [contribution guidelines](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CONTRIBUTING.md#ways-to-contribute). If you are contributing code, please be familiar with the [coding standard](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODING_STANDARDS.md#visual-studio-settings).

## License
The model code is distributed under the [GPLv2 License](https://github.com/Open-Systems-Pharmacology/Suite/blob/develop/LICENSE).

## References
[1] [D Mori, E Kimoto, B Rago, Y Kondo, A King‐Ahmad, R Ramanathan, LS Wood, JG Johnson, VH Le, M Vourvahis, A David Rodrigues. Dose‐dependent inhibition of OATP1B by rifampicin in healthy volunteers: comprehensive evaluation of candidate biomarkers and OATP1B probe drugs. Clinical Pharmacology & Therapeutics, Apr;107(4):1004-13, 2020.](https://pubmed.ncbi.nlm.nih.gov/31628668/)

[2] [I Takehara, T Yoshikado, K Ishigame, D Mori, KI Furihata, N Watanabe, O Ando, K Maeda, Y Sugiyama, H Kusuhara. Comparative study of the dose-dependence of OATP1B inhibition by rifampicin using probe drugs and endogenous substrates in healthy volunteers. Pharmaceutical research, Jul;35:1-3, 2018.](https://pubmed.ncbi.nlm.nih.gov/29748935/)

[3]  [Z Luo, Y Zhang, J Gu, P Feng, Y Wang. Pharmacokinetic Properties of Single- and Multiple-Dose Pitavastatin Calcium Tablets in Healthy Chinese Volunteers. Curr Ther Res Clin Exp, Mar 3;77:52-7, 2015.](https://pubmed.ncbi.nlm.nih.gov/26082816/)

[4] [E Kimoto, C Costales, MA West, YA Bi, M Vourvahis, A David Rodrigues, MVS Varma. Biomarker-Informed Model-Based Risk Assessment of Organic Anion Transporting Polypeptide 1B Mediated Drug-Drug Interactions. Clin Pharmacol Ther, Feb;111(2):404-415, 2022.](https://pubmed.ncbi.nlm.nih.gov/34605015/)

[5] [Y Chen, W Zhang, WH Huang, ZR Tan, YC Wang, X Huang, HH Zhou. Effect of a single-dose rifampin on the pharmacokinetics of pitavastatin in healthy volunteers. Eur J Clin Pharmacol., Nov;69(11):1933-8, 2013. ](https://pubmed.ncbi.nlm.nih.gov/23831870/)

[6] [T Prueksaritanont, X Chu, R Evers, SO Klopfer, L Caro, PA Kothare, C Dempsey, S Rasmussen, R Houle, G Chan, X Cai, R Valesky, IP Fraser, SA Stoch. Pitavastatin is a more sensitive and selective organic anion-transporting polypeptide 1B clinical probe than rosuvastatin. Br J Clin Pharmacol., Sep;78(3):587-98, 2014.](https://pubmed.ncbi.nlm.nih.gov/24617605/)
