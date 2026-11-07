# G5/G9 未完成事项与限制

## 阻断问题

- 无。

## 非本轮范围

1. 生成式模型真实业务输出：`NOT_RUNTIME_VERIFIED`。
2. WorkBuddy 安装、解析、模型调用、平台预览、审核和正式上架：`WORKBUDDY_VALIDATION_NOT_IN_SCOPE`。
3. 正式发布状态：未设置，也未执行。

## 已解决的实施异常

- 预检发现 100/100 的 1.0.0 ZIP 未包含 LICENSE：已统一修复打包机制并全量复验。
- Git-over-HTTPS 连接失败：前 7 款使用 GitHub Git Data API 重建等价 tree 的 commit；其余使用 SSH:443 原子推送，均已完成远端审计。
- 前 7 款本地与远端 commit SHA 不同：已逐款确认父提交与 tree 完全一致并登记映射；未重写历史、未强推、未覆盖 Tag。
