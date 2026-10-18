# Third-party materials

## SAP sample content

Source: [SAP-samples/datasphere-content](https://github.com/SAP-samples/datasphere-content), specifically [SAP_Sample_Content](https://github.com/SAP-samples/datasphere-content/tree/main/SAP_Sample_Content).

The upstream sample README states:

> Copyright © 2023 SAP SE or an SAP affiliate company. All rights reserved.

The upstream `.reuse/dep5` identifies files under `*` as:

> Copyright: 2019-2023 SAP SE or an SAP affiliate company and data-warehouse-cloud-content
> License: Apache-2.0

An unchanged copy of the upstream root license is included in [LICENSES/Apache-2.0.txt](LICENSES/Apache-2.0.txt). Local CSV paths and upstream hashes are recorded in [docs/source-provenance.json](docs/source-provenance.json).

The original 38 local CSVs were compared with that repository on 16 October 2026. On 18 October, unused inputs were removed; the portfolio now includes 10 CSVs (four HR, three Finance, three Sales). Their text contents match after encoding and line-ending normalization, including trailing line endings. The retained files were not modified. Provenance lists only retained inputs; the two retained files needing additional whitespace comparisons are recorded in [docs/source-differences.json](docs/source-differences.json).

The `HR/`, `FI/`, and `Sales/` directories contain SAP sample inputs. Model exports are outputs from the project tenant; the Sales model extends tutorial content. Project changes and validations are described in README.md. This project does not claim authorship of the SAP sample data or the original tutorial model.

The upstream notice distinguishes API calls to external products from the repository's open-source license. Access to SAP or third-party products remains subject to the provider's applicable agreements; a copy of sample content does not grant access to a SAP tenant.

SAP names and marks belong to their respective owners. This is an independent learning portfolio, not an official SAP product. No blanket license is assigned here to newly authored portfolio material.

