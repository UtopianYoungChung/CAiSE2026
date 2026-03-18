# Supplementary Materials — Identity-Sensitive Requirements in Human-AI Collaboration

**Paper:** Modeling and Analyzing Identity-Sensitive Requirements in Human-AI Collaboration
**Venue:** CAiSE 2026 (38th International Conference on Advanced Information Systems Engineering)
**Authors:** Young Jo(seph) Chung, Kun Eun (Karen) Bae, Eric Yu
**Affiliation:** Faculty of Information & Department of Computer Science, University of Toronto

---

## Overview

This repository contains supplementary illustrative examples for the paper *Modeling and Analyzing Identity-Sensitive Requirements in Human-AI Collaboration*. The paper introduces an approach for representing and analyzing professional identity concerns in requirements engineering when AI systems are viewed as having agency within organizations. It maps identity dimensions (person-based, role-based, relational) from organizational identity theory to *i** constructs (agents, roles, dependencies) and demonstrates this mapping through a retrospective analysis of a bank's AI talent acquisition system (Santander case, presented in the paper).

Due to space constraints, the Santander case is presented in full in the paper. This repository provides additional illustrative examples that further demonstrate the approach's applicability across organizational contexts.

## Repository Structure

```
CAiSE2026/
├── README.md
├── LICENSE
├── examples/
│   └── CleverLoan/
│       ├── CleverLoan_narration.md          # Detailed case narration and analysis
│       ├── CleverLoan LC-1.pdf              # LC-1: Functional SR model
│       ├── CleverLoan LC-2_ SR 'AS-IS'.pdf  # LC-2: As-Is SR model with person-based identities
│       ├── CleverLoan LC-3 SD 'To-Be'.pdf   # LC-3: To-Be SD model
│       ├── CleverLoan LC-4 SR 'To-Be'.pdf   # LC-4: To-Be SR model
│       └── ...
```

## Illustrative Examples

### CleverLoan — AI Loan Decision System

Drawn from Strich et al. (2021), this case analyzes an AI-assisted loan consulting system at a European retail bank. Unlike the Santander case (where the manager championed human-AI collaboration), CleverLoan's management prioritized efficiency over preserving consultants' professional identities — producing contrasting outcomes.

**Key contributions beyond the Santander case:**

- **Divergent identities within a single role:** Two agents (Max, experienced; Anna, junior) instantiate the same *Loan Consultant* role but respond to AI in opposite ways — threat vs. empowerment
- **AI-enabled role creation:** The To-Be model introduces an entirely new *AI-Supported Consultant* role with no As-Is precedent
- **Failure mode analysis:** Models what happens when identity concerns are *not* addressed in system design, including organizationally destructive behaviors (data manipulation)
- **Diagnostic capability:** Surfaces the same requirement categories (transparency, authority preservation) as the Santander case but as *unmet* requirements, demonstrating the framework's diagnostic value

The four *i** models (LC-1 through LC-4) progressively introduce identity-sensitive constructs, paralleling the paper's Figures 3-6 for the Santander case.

See [`examples/CleverLoan/CleverLoan_narration.md`](examples/CleverLoan/CleverLoan_narration.md) for the full case narration and analysis.

## References

- Strich, F., Mayer, A.-S., Fiedler, M.: What Do I Do in a World of Artificial Intelligence? Investigating the Impact of Substitutive Decision-Making AI Systems on Employees' Professional Role Identity. *Journal of the Association for Information Systems* **22**(2), 304-324 (2021)
- Simon, C., Revilla, E., Saenz, M.J.: Integrating AI in Organizations for Value Creation through Human-AI Teaming: A Dynamic-Capabilities Approach. *Journal of Business Research* **182**, 114783 (2024)

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

This work is licensed under the [Creative Commons Attribution 4.0 International License](LICENSE).
