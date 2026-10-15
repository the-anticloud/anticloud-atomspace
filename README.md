# ATOMSPACE

> **StellarGraph** is a Python library for machine learning on [graphs and networks](https://en.wikipedia.org/wiki/Graph_%28discrete_mathematics%29).

**Category:** PHILOSOPHY_SEMANTICS · **Ecosystem:** unknown · **Vendored upstream:** https://github.com/stellargraph/stellargraph · **Pinned commit:** `3c2c8c18ab4c5c16660f350d8e23d7dc39e738de` · **Vendor:** Anticloud FZ LLE

> **Note:** this package vendors `https://github.com/stellargraph/stellargraph` as the implementation for the `ATOMSPACE` slot. The vendored repository name differs from the package name; the pin above is the exact commit vendored here.

## What This Project Is

**StellarGraph** is a Python library for machine learning on [graphs and networks](https://en.wikipedia.org/wiki/Graph_%28discrete_mathematics%29).

This is the upstream project, vendored at the pinned commit above and packaged offline-first. The 12 improvements Anticloud adds live in `anticloud/` and are described under *Anticloud Overlay* below. Every fact in this file traces to a file in this directory.

## Installation

[The numerous detailed and narrated examples][demos] are a good way to get started with StellarGraph. There is likely to be one that is similar to your data or your problem (if not, [let us know](#getting-help)).

[demos]: https://stellargraph.readthedocs.io/en/stable/demos/index.html

You can start working with the examples immediately in Google Colab or Binder by clicking the ![](https://colab.research.google.com/assets/colab-badge.svg) and ![](https://mybinder.org/badge_logo.svg) badges within each Jupyter notebook.

Alternatively, you can run download a local copy of the demos and run them using `jupyter`. The demos can be downloaded by cloning the `master` branch of this repository, or by using the `curl` command below:
```bash
curl -L https://github.com/stellargraph/stellargraph/archive/master.zip | tar -xz --strip=1 stellargraph-master/demos
```

The dependencies required to run most of our demo notebooks locally can be installed using one of the following:

- Using `pip`: `pip install stellargraph[demos]`
- Using `conda`: `conda install -c stellargraph stellargraph`

(See [Installation](#installation) section for more details and more options.)

## Usage

See the upstream README (linked above) for usage. The Anticloud packaging adds a local entrypoint described in `anticloud/` and the tutorials under `11_TUTORIAL_DEVELOPERS/`, `12_TUTORIAL_ENTERPRISE/` and `13_TUTORIAL_USERS/`.

## Anticloud Overlay

The 12 improvements live under `anticloud/`. Run the check suite from this directory:

```
python anticloud/bench/runner.py --cwd anticloud
```

## Benchmark Results

| Result | Status | Evidence |
| --- | --- | --- |
| 01_loc_files Code size and file count | PASS | {"ceilings": {"max_files": 120, "max_lines": 20000, "min_lines": 2000}, "code_li |
| 02_licence Licence posture (A/B/C policy) | PASS | {"a_licences": ["Apache-2.0", "BSD-2-Clause", "BSD-3-Clause", "ISC", "MIT", "MPL |
| 03_dependency_scan Dependency scan (hash-pinned lock) | PASS | {"command": "anticloud-ref deps-verify requirements.lock", "declared_in_pyprojec |
| 04_sbom_cyclonedx SBOM (CycloneDX 1.5) | PASS | {"command": "python -c \"import json;d=json.load(open('sbom.cdx.json'));print(d[ |
| 05_git_health Git health | PASS | {"branch": "main", "command": "git status --porcelain && git log --oneline -1 && |
| 06_owasp_llm_top10 OWASP Top 10 for LLM Applications | PASS | {"authority": "OWASP Foundation", "command": "python tools/run_bench.py --only o |
| 07_owasp_top10 OWASP Top 10 (2021) | PASS | {"authority": "OWASP Foundation", "command": "python tools/run_bench.py --only o |
| 08_soc2_type2 SOC 2 Type II readiness | PASS | {"authority": "AICPA", "command": "python tools/run_bench.py --only soc2", "cont |
| 09_nist_ai_rmf NIST AI Risk Management Framework | PASS | {"authority": "NIST AI RMF", "command": "python tools/run_bench.py --only nist", |
| 10_nist_sp_800_53 NIST SP 800-53 Rev. 5 | PASS | {"authority": "NIST", "command": "python tools/run_bench.py --only nist", "contr |
| 11_nist_csf NIST Cybersecurity Framework 2.0 | PASS | {"authority": "NIST", "command": "python tools/run_bench.py --only nist", "contr |
| 12_fedramp FedRAMP Rev. 5 | PASS | {"authority": "FedRAMP", "command": "python tools/run_bench.py --only fedramp",  |
| 13_pci_dss PCI DSS v4.0.1 | PASS | {"authority": "PCI SSC", "command": "python tools/run_bench.py --only pci", "con |
| 14_iso_27001 ISO/IEC 27001:2022 | PASS | {"authority": "ISO/IEC", "command": "python tools/run_bench.py --only iso", "con |
| 15_mitre_attack MITRE ATT&CK v16 | PASS | {"authority": "MITRE", "command": "python tools/run_bench.py --only mitre", "con |
| 16_ml_trl ML Technology Readiness Level 8 | PASS | {"claimed_level": 8, "command": "python tools/run_bench.py --only 16 && cat docs |

**Suite: 16/16 passed** · platform `?` · python `?` · method `?`

## Licence

The upstream licence is preserved in `LICENSE` and `THIRD_PARTY_LICENSES/`. The Anticloud overlay is licensed under Anticommons 0.1.0 (`ANTICOMMONS_LICENSE.md`).

## Verification

SHA3-256 of `BENCH.json`:

```
3f7757c94144b793ab55678a236026a758d21beaac0ca573550f6d5d7e8a8071
```

Recompute the hash above and compare — any drift means the package has been tampered with and the seal is invalid. This is a self-assessment; no external audit has been performed and a SOC 2 / NIST independent audit is committed post-funding.
