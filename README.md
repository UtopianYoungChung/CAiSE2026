# Supplementary Materials - Identity-Sensitive Requirements in Human-AI Collaboration

Paper: Modeling and Analyzing Identity-Sensitive Requirements in Human-AI Collaboration  
Venue: CAiSE 2026 (38th International Conference on Advanced Information Systems Engineering)  
Authors: Young Jo(seph) Chung, Kun Eun (Karen) Bae, Eric Yu  
Affiliation: Faculty of Information and Department of Computer Science, University of Toronto

## Overview

This repository contains supplementary materials for the CAiSE 2026 paper on identity-sensitive requirements in human-AI collaboration.

The Santander case is presented in full in the paper. This repository provides **three additional illustrative case packages** under `examples/`, with model artifacts provided as PDF files (Strategic Dependency and Strategic Rationale diagrams, plus compiled case narratives where noted).

## Repository structure

```text
CAiSE2026/
|- .gitignore
|- LICENSE
|- README.md
`- examples/
   |- CleverLoan/
   |  |- CleverLoan Indentity Sensitive Model Examples.pdf
   |  |- CleverLoan LC-1.pdf
   |  |- CleverLoan LC-2_ SR 'AS-IS'.pdf
   |  |- CleverLoan LC-3 SD 'To-Be'.pdf
   |  `- CleverLoan LC-4 SR 'To-Be'.pdf
   |- NeuroYou/
   |  |- NeuroYou Identity Sensitive Model Examples.pdf
   |  |- NY-1 Functional SR Model.pdf
   |  |- NY-2 SR 'AS-IS'.pdf
   |  |- NY-3 SD 'To-Be'.pdf
   |  `- NY-4 SR 'To-Be'.pdf
   `- CustomerSupport/
      |- CustomerSupport Identity Sensitive Model Examples.pdf
      |- CS-1 As-Is SD.pdf
      `- CS-2 To-Be SR.pdf
```

## CleverLoan case materials

The `examples/CleverLoan/` folder contains:

- `CleverLoan Indentity Sensitive Model Examples.pdf`
- `CleverLoan LC-1.pdf`
- `CleverLoan LC-2_ SR 'AS-IS'.pdf`
- `CleverLoan LC-3 SD 'To-Be'.pdf`
- `CleverLoan LC-4 SR 'To-Be'.pdf`

These files illustrate the identity-sensitive requirements analysis approach using Strich et al.'s loan-consulting setting.

## NeuroYou case materials

The `examples/NeuroYou/` folder contains:

- `NeuroYou Identity Sensitive Model Examples.pdf` — compiled narrative and discussion for this case (functional SR, identity-sensitive As-Is SR, To-Be SD with alternatives, To-Be SR with Alternative 2)
- `NY-1 Functional SR Model.pdf` — functional as-is Strategic Rationale (no person-based identities)
- `NY-2 SR 'AS-IS'.pdf` — identity-sensitive as-is Strategic Rationale
- `NY-3 SD 'To-Be'.pdf` — to-be Strategic Dependency (Alternative 1 and Alternative 2)
- `NY-4 SR 'To-Be'.pdf` — to-be Strategic Rationale with Alternative 2 (hybrid practice)

These files illustrate identity-sensitive models for van den Broek et al.'s hiring-system setting.

## CustomerSupport case materials

The `examples/CustomerSupport/` folder contains:

- `CustomerSupport Identity Sensitive Model Examples.pdf` — supplementary write-up (case introduction, As-Is and To-Be narrative, typal dependency registry **D1–D18**, concrete dependency matrix **CD1–CD15**, and references); consult this PDF together with the diagram files below
- `CS-1 As-Is SD.pdf` — As-Is Strategic Dependency model (Brynjolfsson-style augmentative deployment)
- `CS-2 To-Be SR.pdf` — To-Be Strategic Rationale model (identity-sensitive redesign with means–ends alternatives, contribution links, and relational closure on the typal layer)

These materials relate to Brynjolfsson et al.’s generative-AI-at-work customer-support setting.

## References

- Strich, F., Mayer, A.-S., Fiedler, M.: What Do I Do in a World of Artificial Intelligence? Investigating the Impact of Substitutive Decision-Making AI Systems on Employees' Professional Role Identity. Journal of the Association for Information Systems 22(2), 304-324 (2021)
- van den Broek, E., Sergeeva, A., Huysman, M.: When the Machine Meets the Expert: An Ethnography of Developing AI for Hiring. MIS Quarterly 45(3), 1557-1580 (2021)
- Brynjolfsson, E., Li, D., Raymond, L.R.: Generative AI at Work. National Bureau of Economic Research Working Paper 31161, Cambridge, MA (2023). https://doi.org/10.3386/w31161
- Simon, C., Revilla, E., Saenz, M.J.: Integrating AI in Organizations for Value Creation through Human-AI Teaming: A Dynamic-Capabilities Approach. Journal of Business Research 182, 114783 (2024)
- Yu, E., Giorgini, P., Maiden, N.A., Mylopoulos, J.: Social Modeling for Requirements Engineering. MIT Press, Cambridge, MA (2011)

## Citation

If you use these materials, please cite:

```bibtex
@inproceedings{chung2026identity,
  title={Modeling and Analyzing Identity-Sensitive Requirements in Human-AI Collaboration},
  author={Chung, Young Jo(seph) and Bae, Kun Eun (Karen) and Yu, Eric},
  booktitle={Proceedings of the 38th International Conference on Advanced Information Systems Engineering (CAiSE 2026)},
  year={2026},
  publisher={Springer},
  series={Lecture Notes in Computer Science}
}
```

## License

This work is licensed under the Creative Commons Attribution 4.0 International License. See `LICENSE`.
