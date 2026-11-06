# 教培产品基线独立审计报告（整改后重建审计）

- 审计方式：从 GitHub API 重新读取远程仓库、提交、文件树和文件正文
- 不采用上一轮执行报告的 PASS 结论作为证据
- 审计时间：11/06/2026 20:54:21
- 审计结论：**通过**

## 1. 仓库审计

| 指标 | 结果 |
|---|---:|
| 审计仓库 | 101（1个总仓库＋100个产品仓库） |
| 产品仓库通过 | 100 |
| 产品仓库失败 | 0 |
| Skill | 80 |
| Agent | 20 |
| 唯一产品编号 | 100 |
| 唯一仓库名称 | 100 |
| 敏感信息命中产品 | 0 |

总仓库远程HEAD：`29dea85b20a3ebbd62077baa746cbf3d7df9969d`；公开状态：public；LICENSE SHA-256：`CFC7749B96F63BD31C3C42B5C471BF756814053E847C10F3EB003417BC523D30`。

所有产品仓库均检查了：存在性、组织归属、公开状态、默认分支、远程文件树、README、PRODUCT_SPEC.md、LICENSE、远程HEAD、敏感信息和索引一致性。

## 2. 审计发现

- 未发现审计问题。

- 开放P0：0
- 开放P1：0
- 开放P2：0

## 3. 100份规格书逐项审计

| 产品编号 | 产品 | 类型 | 12章节 | 案例 | 测试 | 身份/矩阵一致 | 敏感命中 | 模板共享比例 | 结论 |
|---|---|---|---:|---:|---:|---|---:|---:|---|
| `JLZ-EDU-SK-001` | 本地教培市场调研 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-002` | 招生营销活动策划 | Skill | 12 | 3 | 6 | True | 0 | 0.541 | PASS |
| `JLZ-EDU-SK-003` | 年度招生规划 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-SK-004` | 小红书招生文案 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-005` | 朋友圈招生文案 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-SK-006` | 教培短视频脚本 | Skill | 12 | 3 | 6 | True | 0 | 0.55 | PASS |
| `JLZ-EDU-SK-007` | 招生直播脚本 | Skill | 12 | 3 | 6 | True | 0 | 0.55 | PASS |
| `JLZ-EDU-SK-008` | 招生海报文案 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-009` | 老带新活动策划 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-010` | 异业合作方案 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-011` | 招生线索表单设计 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-012` | 招生预算测算 | Skill | 12 | 3 | 6 | True | 0 | 0.55 | PASS |
| `JLZ-EDU-AG-001` | 校区招生增长诊断 | Agent | 12 | 3 | 7 | True | 0 | 0.5161 | PASS |
| `JLZ-EDU-AG-002` | 内容营销运营 | Agent | 12 | 3 | 7 | True | 0 | 0.5039 | PASS |
| `JLZ-EDU-AG-003` | 社区招生渠道拓展 | Agent | 12 | 3 | 7 | True | 0 | 0.5161 | PASS |
| `JLZ-EDU-SK-013` | 招生线索分层 | Skill | 12 | 3 | 6 | True | 0 | 0.5739 | PASS |
| `JLZ-EDU-SK-014` | 首次咨询话术 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-SK-015` | 家长需求诊断 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-SK-016` | 客户跟进计划 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-SK-017` | 试听邀约方案 | Skill | 12 | 3 | 6 | True | 0 | 0.569 | PASS |
| `JLZ-EDU-SK-018` | 试听课堂观察 | Skill | 12 | 3 | 6 | True | 0 | 0.569 | PASS |
| `JLZ-EDU-SK-019` | 家长异议分类 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-SK-020` | 沉睡线索激活 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-SK-021` | 招生转化漏斗计算 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-AG-004` | 线索响应调度 | Agent | 12 | 3 | 7 | True | 0 | 0.5246 | PASS |
| `JLZ-EDU-AG-005` | 试听转化复盘 | Agent | 12 | 3 | 7 | True | 0 | 0.5203 | PASS |
| `JLZ-EDU-AG-006` | 续费流失风险预警 | Agent | 12 | 3 | 7 | True | 0 | 0.512 | PASS |
| `JLZ-EDU-SK-022` | 课程标准对齐 | Skill | 12 | 3 | 6 | True | 0 | 0.569 | PASS |
| `JLZ-EDU-SK-023` | 教学目标分解 | Skill | 12 | 3 | 6 | True | 0 | 0.5739 | PASS |
| `JLZ-EDU-SK-024` | 教案设计 | Skill | 12 | 3 | 6 | True | 0 | 0.5366 | PASS |
| `JLZ-EDU-SK-025` | 课堂活动设计 | Skill | 12 | 3 | 6 | True | 0 | 0.55 | PASS |
| `JLZ-EDU-SK-026` | 分层教学任务 | Skill | 12 | 3 | 6 | True | 0 | 0.569 | PASS |
| `JLZ-EDU-SK-027` | 分层作业生成 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-028` | 课堂即时练习 | Skill | 12 | 3 | 6 | True | 0 | 0.5739 | PASS |
| `JLZ-EDU-SK-029` | 单元测评设计 | Skill | 12 | 3 | 6 | True | 0 | 0.569 | PASS |
| `JLZ-EDU-SK-030` | 试卷生成 | Skill | 12 | 3 | 6 | True | 0 | 0.55 | PASS |
| `JLZ-EDU-SK-031` | 题目知识点与难度标注 | Skill | 12 | 3 | 6 | True | 0 | 0.5739 | PASS |
| `JLZ-EDU-SK-032` | 错因分析 | Skill | 12 | 3 | 6 | True | 0 | 0.569 | PASS |
| `JLZ-EDU-SK-033` | 学情分析 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-SK-034` | 课堂观察量表 | Skill | 12 | 3 | 6 | True | 0 | 0.5789 | PASS |
| `JLZ-EDU-SK-035` | 教学反思助手 | Skill | 12 | 3 | 6 | True | 0 | 0.5789 | PASS |
| `JLZ-EDU-AG-007` | 小学数学教研 | Agent | 12 | 3 | 7 | True | 0 | 0.5161 | PASS |
| `JLZ-EDU-AG-008` | 小学语文教研 | Agent | 12 | 3 | 7 | True | 0 | 0.5289 | PASS |
| `JLZ-EDU-AG-009` | 小学英语教研 | Agent | 12 | 3 | 7 | True | 0 | 0.5161 | PASS |
| `JLZ-EDU-AG-010` | 课程体系开发 | Agent | 12 | 3 | 7 | True | 0 | 0.512 | PASS |
| `JLZ-EDU-SK-036` | 智能排课 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-SK-037` | 教室与资源调度 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-SK-038` | 教师课时统计 | Skill | 12 | 3 | 6 | True | 0 | 0.569 | PASS |
| `JLZ-EDU-SK-039` | 考勤异常处理 | Skill | 12 | 3 | 6 | True | 0 | 0.5739 | PASS |
| `JLZ-EDU-SK-040` | 调课补课登记 | Skill | 12 | 3 | 6 | True | 0 | 0.569 | PASS |
| `JLZ-EDU-SK-041` | 代课教师安排 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-SK-042` | 学员名册管理 | Skill | 12 | 3 | 6 | True | 0 | 0.5739 | PASS |
| `JLZ-EDU-SK-043` | 学习进度跟踪 | Skill | 12 | 3 | 6 | True | 0 | 0.5739 | PASS |
| `JLZ-EDU-SK-044` | 学期教学日历 | Skill | 12 | 3 | 6 | True | 0 | 0.569 | PASS |
| `JLZ-EDU-SK-045` | 教务交接清单 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-AG-011` | 教务运营助手 | Agent | 12 | 3 | 7 | True | 0 | 0.5161 | PASS |
| `JLZ-EDU-AG-012` | 排课冲突诊断 | Agent | 12 | 3 | 7 | True | 0 | 0.5246 | PASS |
| `JLZ-EDU-SK-046` | 家校通知生成 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-047` | 学生成长周报 | Skill | 12 | 3 | 6 | True | 0 | 0.5739 | PASS |
| `JLZ-EDU-SK-048` | 家长会策划 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-049` | 家长满意度调查 | Skill | 12 | 3 | 6 | True | 0 | 0.55 | PASS |
| `JLZ-EDU-SK-050` | 家长投诉分类 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-051` | 家长投诉回复 | Skill | 12 | 3 | 6 | True | 0 | 0.5739 | PASS |
| `JLZ-EDU-SK-052` | 家庭学习任务设计 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-SK-053` | 转介绍沟通文案 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-AG-013` | 家校沟通协同 | Agent | 12 | 3 | 7 | True | 0 | 0.512 | PASS |
| `JLZ-EDU-AG-014` | 家长投诉全流程处理 | Agent | 12 | 3 | 7 | True | 0 | 0.5161 | PASS |
| `JLZ-EDU-SK-054` | 教培岗位说明书 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-SK-055` | 招聘计划 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-056` | 岗位面试题库 | Skill | 12 | 3 | 6 | True | 0 | 0.569 | PASS |
| `JLZ-EDU-SK-057` | 面试评价表 | Skill | 12 | 3 | 6 | True | 0 | 0.5789 | PASS |
| `JLZ-EDU-SK-058` | 员工入职清单 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-SK-059` | 教师培训计划 | Skill | 12 | 3 | 6 | True | 0 | 0.55 | PASS |
| `JLZ-EDU-SK-060` | 岗位绩效KPI设计 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-SK-061` | 劳动用工合规检查 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-AG-015` | 招聘流程管理 | Agent | 12 | 3 | 7 | True | 0 | 0.5161 | PASS |
| `JLZ-EDU-AG-016` | 教师能力发展 | Agent | 12 | 3 | 7 | True | 0 | 0.5203 | PASS |
| `JLZ-EDU-SK-062` | 班级成本分摊 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-SK-063` | 学费收入台账 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-SK-064` | 应收款核对 | Skill | 12 | 3 | 6 | True | 0 | 0.5739 | PASS |
| `JLZ-EDU-SK-065` | 教师薪酬提成计算 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-SK-066` | 退费测算 | Skill | 12 | 3 | 6 | True | 0 | 0.569 | PASS |
| `JLZ-EDU-SK-067` | 付款凭证核对 | Skill | 12 | 3 | 6 | True | 0 | 0.569 | PASS |
| `JLZ-EDU-SK-068` | 月度结账清单 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-SK-069` | 费用报销审核 | Skill | 12 | 3 | 6 | True | 0 | 0.5593 | PASS |
| `JLZ-EDU-AG-017` | 财务经营分析 | Agent | 12 | 3 | 7 | True | 0 | 0.5079 | PASS |
| `JLZ-EDU-AG-018` | 学费退费风险管控 | Agent | 12 | 3 | 7 | True | 0 | 0.512 | PASS |
| `JLZ-EDU-SK-070` | 组织与岗位职责映射 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-SK-071` | 工作流程拆解 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-072` | SOP执行检查 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-073` | 校区日常巡检 | Skill | 12 | 3 | 6 | True | 0 | 0.5546 | PASS |
| `JLZ-EDU-SK-074` | 服务质量检查 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-SK-075` | 教学服务标准核查 | Skill | 12 | 3 | 6 | True | 0 | 0.569 | PASS |
| `JLZ-EDU-SK-076` | 招生服务流程检查 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-SK-077` | 教务交接审计 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-SK-078` | 新校区开办清单 | Skill | 12 | 3 | 6 | True | 0 | 0.541 | PASS |
| `JLZ-EDU-SK-079` | 新校区筹建计划 | Skill | 12 | 3 | 6 | True | 0 | 0.5366 | PASS |
| `JLZ-EDU-SK-080` | 多校区标准对比 | Skill | 12 | 3 | 6 | True | 0 | 0.5641 | PASS |
| `JLZ-EDU-AG-019` | 校区标准化体系建设 | Agent | 12 | 3 | 7 | True | 0 | 0.5161 | PASS |
| `JLZ-EDU-AG-020` | 多校区运营协同 | Agent | 12 | 3 | 7 | True | 0 | 0.5161 | PASS |

逐产品机器可读结果见同目录 `EDUCATION_SPEC_AUDIT_MATRIX.csv`。模板共享比例只用于发现重复叙述，不用于证明产品功能差异；功能差异还结合产品目标、输入、执行流程、输出、案例、风险和差异化说明进行核对。

## 4. 六款既有产品证据状态

| 既有产品 | 可读远程证据 | 状态 | 审计处理 |
|---|---|---|---|
| 教师成长反馈专家 | 未找到独立同名仓库或明确产品说明 | UNVERIFIED | 不判定为无重复；相关产品按保守边界审查并保留 UNVERIFIED |
| 教培销冠陪练专家 | `yangsongbaofu-dot/jiaopei-sales-champion-expert` / `88448b7701ae10831d05c18f8e56b344381bfc0a` | VERIFIED_REMOTE_README | 仅按销售模拟与能力训练边界比较 |
| 校长经营OS LITE | 未找到同名独立源码，参考 `yangsongbaofu-dot/he-academy-operations` | UNVERIFIED_EXACT_PRODUCT | 不判定为无重复；综合经营能力按任务基线保守拆分 |
| 教培财税OS LITE | `yangsongbaofu-dot/heyuan-tax-os-lite` / `72f5cc1749e1d8c67c3ea6f49ae124c435ffe2b1` | VERIFIED_REMOTE_README | 新产品仅做经营财务辅助，不复制税政与办理体系 |
| MT-CRM | `yangsongbaofu-dot/mt-crm` / `464707a61eae38cab9ef8dcfc03acd8959fe06e8` | VERIFIED_REMOTE_README | 新产品不做CRM或客户数据托管 |
| techAI·禾苗老师 | `yangsongbaofu-dot/hemiao-teacher-workbench` / `caaca3ad40bd84d5471d4b533b3b32455dd3a5a5` | VERIFIED_REMOTE_README | 新产品限定独立教学任务，不复制完整教研生产平台 |

## 5. 审计结论与冻结条件

P0、P1、P2均无开放项，100份规格书全部通过，可进入基线冻结。

