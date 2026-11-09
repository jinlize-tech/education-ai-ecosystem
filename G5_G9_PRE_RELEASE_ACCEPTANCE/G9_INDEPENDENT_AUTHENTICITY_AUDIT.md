# G9 独立真实性审计

## 结论

- 独立本地审计：100/100 PASS
- 独立远端审计：100/100 PASS
- 失败：0
- GitHub Public：100/100
- 归档仓库：0/100
- 运行状态：`NOT_RUNTIME_VERIFIED`
- WorkBuddy 验证：`WORKBUDDY_VALIDATION_NOT_IN_SCOPE`

## 审计方法

审计程序没有只读取产品测试脚本的 PASS 字段，而是独立执行以下检查：

1. 重跑 100 款产品的完整、缺失、冲突、敏感信息和非法 JSON 输入场景。
2. 重跑 7 款计算产品的全部真实 Node 案例并比对明确预期结果。
3. 通过 SSH 读取每个远端仓库的 `main`、开发分支和 `product-v1.0.1` Tag，确认三者对齐。
4. 获取每个真实远端 commit，核对 remote tree 与本地审计 tree。
5. 从远端 Git 对象读取每个 1.0.1 ZIP，重新计算 SHA-256。
6. 解压远端 ZIP，核对 entries、LICENSE、THIRD_PARTY_NOTICES、版本、测试结果和 `package-manifest.json`。
7. 核对原始规格书、LICENSE 和 BASELINE_VERSION 未被修改。
8. 扫描秘密、收费模型 API、内部绝对路径和敏感凭据模式。

## SHA 说明

前 7 款产品因任务期间 Git-over-HTTPS 连接失败，使用 GitHub Git Data API 重建等价 commit。远端 commit SHA 与本地 commit SHA 不同，但 tree SHA、父提交和全部文件内容一致。其余 93 款使用 SSH 原子推送，远端 SHA 与本地审计 SHA 相同。完整映射见 `G5_G9_CHANGE_MANIFEST.json`。

## 无法证明的事项

本轮没有运行生成式模型的真实业务输出，也没有进行 WorkBuddy 安装、解析、调用、审核或发布。上述事项不得从本地包验收推导为已通过。
