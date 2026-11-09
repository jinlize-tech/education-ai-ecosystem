# Jinlize Education AI

Jinlize Education AI is an independent education-sector AI product system for training and education organizations, principals, teachers, course consultants, academic operations staff, HR staff, finance staff, and multi-campus managers.

The ecosystem contains **100 planned products**: **80 Skills** and **20 Agents**, each managed in an independent repository. All 101 education repositories, including this hub, use **Apache-2.0**.

## Current status

- Product planning: frozen at `EDUCATION_BASELINE_V1.0.0`
- Product planning documents: 100 independent `PRODUCT_SPEC.md` files
- Initial implementation: **100/100 PACKAGE_READY**
- Local package/contract tests: **100/100 PASS**
- WorkBuddy platform validation: **0/100, NOT_VERIFIED**
- Release-ready: **0/100**

The repositories contain installable WorkBuddy-oriented package candidates. Local tests prove package structure, contracts, deterministic calculator behavior where applicable, and safety checks. They do not prove WorkBuddy parsing, installation, model behavior, review, or publication.

## Development

- [Development status](DEVELOPMENT_STATUS.md)
- [Release matrix](RELEASE_MATRIX.csv)
- [Final acceptance report](docs/EDUCATION_100_PRODUCTS_FINAL_ACCEPTANCE_REPORT.md)
- [Stage acceptance reports](docs/stages)

## Planning documents

- [100-product catalog](CATALOG.md)
- [Master plan](docs/EDUCATION_PRODUCT_MASTER_PLAN.md)
- [Product specification matrix](docs/EDUCATION_PRODUCT_SPEC_MATRIX.csv)
- [Product specification index](docs/PRODUCT_SPEC_INDEX.md)
- [Four-stage roadmap](docs/EDUCATION_PRODUCT_ROADMAP.md)
- [WorkBuddy standard](docs/EDUCATION_WORKBUDDY_STANDARD.md)
- [Deduplication review](docs/EDUCATION_PRODUCT_DEDUPLICATION_REVIEW.md)
- [Project isolation policy](docs/PROJECT_ISOLATION_POLICY.md)

## Architecture

| Code | Section | Products |
|---|---|---:|
| 01 | 招生营销中心 | 15 |
| 02 | 销售转化中心 | 12 |
| 03 | 教学教研中心 | 18 |
| 04 | 教务运营中心 | 12 |
| 05 | 家校服务中心 | 10 |
| 06 | 人力组织中心 | 10 |
| 07 | 财务运营中心 | 10 |
| 08 | 校区标准化与多校区管理中心 | 13 |
|  | **合计** | **100** |

## License

License: Apache-2.0.

This repository and the 100 independent education product repositories are free and open. Anyone may use, modify, and distribute the material under Apache License 2.0. The complete legal terms are in [LICENSE](LICENSE).

The project does not sell official paid SKUs for these 100 products. This commercial policy does not limit any right granted by Apache-2.0, including third-party commercial use or redistribution.

## Organization

- [jinlize-tech](https://github.com/jinlize-tech)
- [education-ai-ecosystem](https://github.com/jinlize-tech/education-ai-ecosystem)

## Frozen baseline

- Baseline version: `EDUCATION_BASELINE_V1.0.0`
- Baseline tag: `education-baseline-v1.0.0`
- [Baseline manifest](BASELINE_MANIFEST.json)
- [Baseline version](BASELINE_VERSION.md)
- [Independent baseline audit](docs/EDUCATION_BASELINE_AUDIT.md)

Product implementation work proceeds on development branches after this frozen planning baseline. Specification changes require a new version and audit.

## Current implementation status

- Current product package version: 1.1.0
- Deep upgrade: 100/100
- Contract and scenario tested: 100/100
- Runtime: MODEL_RUNTIME_NOT_VERIFIED
- WorkBuddy validation: WORKBUDDY_VALIDATION_NOT_IN_SCOPE
- Acceptance: [EDUCATION_UPGRADE_FINAL](EDUCATION_UPGRADE_FINAL/FINAL_ACCEPTANCE_REPORT.md)

