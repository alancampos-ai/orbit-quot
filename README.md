# Orbit quotients

#### Article: <small><strong>Exact Orbit Quotients for Allocation</strong> <a href=""><img src="https://cdn.simpleicons.org/doi/2dd4bf" alt="DOI" height="14" align="absmiddle"></a> <a href=""><img src="https://cdn.simpleicons.org/zenodo/2dd4bf" alt="Zenodo" height="14" align="absmiddle"></a> <a href="https://drive.google.com/drive/folders/1l_O2fPVqgi_ExNcjWi0Rm2CghuVsLLO6?usp=drive_link"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/google/google-original.svg" alt="Google Drive" height="14" align="absmiddle"></a></small>

We establish an exact orbit quotient for weighted many-to-one allocation with lower quotas, post-local conflicts, and lexicographic max-excess fairness. Under post-fixing symmetries with uniform adjacency, weights, and complete-or-empty conflict blocks, integer orbit counts admit constructive lifts preserving loads and weights. The quotient preserves every capped optimum and the orbit image of the feasible integer hull. Validation covers 220 instances, 660 formulation runs, 1098 capacity checks, and 120 quotient checks. At multiplicity 32, median reductions relative to Compact are 94.41% in variables, 99.57% in rows, 92.15% in runtime, and 99.39% in sparse-model memory. At multiplicity eight, nine paired Wilcoxon runtime comparisons are significant after Holm correction ($p=1.91\times10^{-5}$). A HEC92-derived timetable yields singleton applicant orbits: all eleven methods return weight 7912 and fairness one, while the quotient adds variables.

#### Dependencies

The experiments used Ubuntu 24.04.4 LTS and CPython 3.12.7. MILPs were solved with HiGHS through `scipy.optimize.milp`, using the following dependencies:

* NumPy 2.3.5
* SciPy 1.17.0
* NetworkX 3.7
* Matplotlib 3.10.8
* psutil 7.2.2
* PyYAML 6.0.3

#### Installation

```bash
docker build --pull -f docker/Dockerfile -t orbit-quot:latest .
docker run --rm orbit-quot:latest
```

#### License (MIT)

* Copyright (c) alancampos-ai
* Code released under the MIT License.
