# Jinlize Education AI

Jinlize Education AI is an independent education-sector AI product system for training and education organizations, principals and institution leaders, frontline teachers, course consultants, academic operations staff, and education-business managers.

This repository is the management and index hub for a planned **1 hub repository + 100 independent product repositories** structure. It records project positioning, product categories, repository indexes, version-management rules, open-source licensing status, contribution rules, and development status.

## Current status

- Planned product repositories: **100**
- Planned Skills: **80**
- Planned Agents: **20**
- Current product implementation status: **Planned / 待研发**
- Available Skill or Agent implementations in this ecosystem: **none yet**

This repository is a planning and repository-management container. Public repository creation does not mean that a Skill or Agent has been implemented, tested, approved, or published on WorkBuddy or any other platform.

## Architecture

The hub repository does not contain product implementations. Each product has an independent repository under the `jinlize-tech` organization. Product repositories currently contain only a minimal placeholder README.

Business sections:

| Code | Section | Planned repositories |
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

## Product index

- [Human-readable catalog](CATALOG.md)
- [CSV repository index](REPOSITORY_INDEX.csv)
- [JSON repository index](REPOSITORY_INDEX.json)
- [Contribution framework](CONTRIBUTING.md)
- [Changelog](CHANGELOG.md)
- [License status](LICENSE_STATUS.md)

## Repository and version rules

1. The hub repository stores indexes, categories, status records, and governance documents only.
2. Each product remains independently installable and usable when later implemented; the hub must not become a hidden runtime dependency.
3. Repository names in this batch are planning identifiers and do not assert that the corresponding function has been delivered.
4. A product moves out of `Planned / 待研发` only after its own requirements, implementation, tests, audit evidence, and release decision are recorded in that product repository.
5. Product releases may use semantic versioning after implementation begins, while the hub records the status and links to the product repository; no release is implied at initialization.
6. No source code, prompt, knowledge base, product archive, or client data is stored in this hub.

## Licensing

Apache-2.0 has been proposed but is not yet approved for adoption. No `LICENSE` file is included in this initialization batch. See [LICENSE_STATUS.md](LICENSE_STATUS.md) for the current boundary.

## Organization

- GitHub organization: [jinlize-tech](https://github.com/jinlize-tech)
- Hub repository: [education-ai-ecosystem](https://github.com/jinlize-tech/education-ai-ecosystem)
