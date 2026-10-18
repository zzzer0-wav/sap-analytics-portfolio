# Publication review

Checked on 16 October 2026. Scope: the local portfolio files; no upload or remote repository was created.

## Completed checks

- All seven SAP model/Preview JSON files parse. The Sales export contains both new KPIs and the country-comparison Preview settings.
- All local README links resolve. Eight screenshots are included: two HR, two Finance, and four Sales.
- All 38 CSVs match the corresponding public SAP sample file contents after accounting for encoding, CRLF/LF, and trailing line endings. The raw byte hashes differ; files have not been rewritten to force a match.
- [Source provenance](source-provenance.json) records the upstream Git tree and per-file Git blob hashes. Thirty-one files match after UTF-8/LF normalization. [Additional comparisons](source-differences.json) show that the remaining seven have the same lines and differ only in trailing whitespace after normalization.
- An unchanged upstream Apache-2.0 license and third-party attribution are included. No separate root NOTICE was present in the inspected upstream tree.
- A targeted scan of model JSON found no matches for password, secret, bearer, access-token, or private-key-header patterns. This is a limited pattern check, not a guarantee that every possible secret format has been excluded.
- A local Git repository on branch `main` and a `.gitignore` have been created. No commit, remote, or push was performed in this review.

## Information retained in exports and screenshots

Model and Preview exports contain SAP schema identifiers, object names, dependency names, and source-system metadata. Screenshots include the training space code and SAP UI. These are not passwords; the original exports are retained to avoid silently breaking model references. They should be considered visible to readers of a public repository.

The CSVs include employee names/demographic fields and business partner contact fields. Their content was compared with the public SAP sample files as described above; they are not presented as the user's own employee/customer data.

## Reproduction limits

- HR and Finance figures were checked against local sample data; Sales screenshot arithmetic and exported formulas were checked, but Sales totals were not independently reconciled to the local CSVs.
- Import into a fresh tenant and cross-tenant Preview restoration have not been tested. Sales relies on remote sources, time objects, and additional tutorial dependencies.
- 2023 Sales is incomplete in the observed model (latest displayed date: 15 May). The main annual comparison uses 2021 and 2022.
- Only one Preview settings file per Finance/Sales model is included. Other layouts are documented through screenshots and instructions.

## Next publication step

Update on 17 October 2026: two SAC screenshots were added, bringing the screenshot count to ten. Both were visually reviewed; the overview shows the 2022 KPIs and the detail image shows all eight country rows with complete values. README now features the SAC overview, and Sales documentation records the user-confirmed Year-filter checks. No SAC transport package is included. The overview filename's duplicated `.png` extension was corrected.

Choose the destination GitHub account and repository name, then review the first commit before pushing. No repository URL has been configured. The upstream sample license is included; licensing of newly authored portfolio material has not been assigned.

## CSV cleanup — 18 October 2026

Removed 28 unused HR/Finance sample CSVs. Retained the four documented HR inputs, three Finance inputs, and three Sales sample inputs. Source provenance and additional comparisons now list only retained files. The 38-file checks above describe the original audit. Sales still requires the remote/tutorial dependencies documented in sales.md; removed FI product samples were not the Sales remote sources. The Finance SAC screenshot brings the current screenshot count to eleven.

