# WorkBuddy统一研发与适配标准

## 1. 当前核验状态

- 核验日期：2026-11-06（Asia/Shanghai）
- 目标平台：WorkBuddy开放平台
- 当前产品状态：`PLANNED_FOR_WORKBUDDY`
- 当前未完成：真实上传、ZIP解析、安装、调用、文件权限、审核和上架测试

## 2. 官方公开资料

| 资料 | URL | 状态 | 适用结论 |
|---|---|---|---|
| Skill开发文档 | https://open.workbuddy.cn/docs/skill | 已核实（A，公开页面） | Skill市场安装、ZIP解析、基础结构与SKILL.md frontmatter字段 |
| 专家开发文档 | https://open.workbuddy.cn/docs/expert | 已核实（A，公开页面） | 专家市场、plugin.json、agents定义、头像规范与Education分类 |
| 开放平台概述 | https://open.workbuddy.cn/docs | 已核实（A，公开页面） | 平台文档入口与产品范围 |
| 收入变现 | https://open.workbuddy.cn/docs/monetization | 已核实（A，公开页面） | 平台当前存在付费能力；本项目不设置官方付费SKU |

## 3. 平台强制要求与内部标准

| 项目 | 平台公开资料状态 | 本项目内部标准 |
|---|---|---|
| Skill目录和必需文件 | 已核实：公开文档展示 `SKILL.md` 必需 | 研发阶段按上传时最新官方结构生成，本阶段不创建实际文件 |
| Skill frontmatter | 已核实：公开文档列出 name、display_name、description、version、author等字段 | 所有展示名称、描述和示例均需中英文一致性检查 |
| 专家目录 | 已核实：公开文档展示 `.codebuddy-plugin/plugin.json`、`avatars/`、`agents/`、`README.md` | 研发阶段单独核验，不沿用Skill目录 |
| 专家展示字段 | 已核实：公开文档列出displayName、profession、displayDescription、categoryId、tags、quickPrompts等 | 中英文一致；描述和标签不得夸大能力 |
| 平台类目 | 已核实：公开文档列出 `15-Education` | 作为候选类目，上传时以后台当前选项为准 |
| 文件大小、数量、审核周期等 | 待核实 | 不在本阶段推测；上传前重新读取官方文档和后台 |
| 工具权限与数据留存 | 待核实到具体账号和场景 | 研发前逐项核验，不默认拥有文件、网络或MCP权限 |

## 4. Skill标准

1. 单一职责、明确触发条件、固定输入输出和异常处理。
2. 独立安装后能够完成承诺的核心任务，不依赖同组Agent或兄弟Skill。
3. 默认不调用收费外部API，不产生未披露费用。
4. 用户输入和输出不得包含公司Logo、宣传语、内部提示词或研发目录。
5. 研发阶段再生成实际 `SKILL.md`；当前只保留 `PRODUCT_SPEC.md`。

## 5. Agent标准

1. 具备专业角色、信息收集、诊断、任务规划、阶段性成果、人工确认、异常恢复和最终复盘。
2. Agent不是「更长提示词」或Skill集合包装，必须提供跨步骤综合判断和交付编排价值。
3. 研发阶段按WorkBuddy专家格式生成独立Agent定义文件，不使用用户禁止的 `AGENT.md` 作为产品实现。
4. 不得自行声明未获系统分配的tools；外部MCP或连接器依赖必须另行走必要性、费用、数据和权限审批。

## 6. 测试与发布门槛

- 标准输入、缺字段、冲突输入、超范围、隐私、长文件、格式异常和工具失败必须覆盖。
- Agent增加中断恢复、人工确认和多阶段交付测试。
- 测试必须在目标提交和目标WorkBuddy版本上执行并可追溯。
- ZIP解析、平台预览、正式审核、正式上架分别记录，不以任一前置状态替代后续状态。
- 未完成平台实测和独立审计前，不得描述为「可上架」或「已发布」。

## 7. 数据与客户可见信息

- 数据最小化，不主动索取与任务无关的个人信息。
- 不将客户输入用于训练、营销或无关用途。
- 客户成果不显示公司品牌、水印或广告式自我介绍。
- 平台强制开发者元数据与客户交付内容严格区分。
