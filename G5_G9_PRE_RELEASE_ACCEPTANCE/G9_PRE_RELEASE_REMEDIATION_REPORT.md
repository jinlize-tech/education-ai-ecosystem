# G9 发布前修复报告

- 修复范围：100/100
- Apache-2.0 ZIP 覆盖：100/100
- 第三方声明 ZIP 覆盖：100/100
- ZIP 清单与 package-manifest 一致：100/100
- ZIP SHA-256 重新计算一致：100/100
- T1-T7 测试状态：100/100 `G9_PRE_RELEASE_ACCEPTED`
- 严重安全问题：0
- 未登记变更：0
- 虚假测试记录：0
- 状态：`GITHUB_PACKAGE_PRE_RELEASE_READY`

## 共性问题与修复

预检发现全部 100 个 1.0.0 ZIP 未包含 `LICENSE`。本轮修复打包机制，而不是只补单个包：

1. 每个 1.0.1 ZIP 加入仓库根 `LICENSE` 与 `THIRD_PARTY_NOTICES.md`。
2. `package-manifest.json` 登记许可证、规范化许可证 SHA-256、清单、版本、ZIP 哈希和旧版本路径。
3. 每个 ZIP 实际解压核对文件清单、许可证内容、SKILL/Agent 结构、输入校验脚本和哈希。
4. 保留全部 1.0.0 ZIP 和 `education-product-baseline-v1.0.0` Tag。
5. 版本文件、Skill/插件元数据、CHANGELOG、product_meta、package-manifest、ZIP 文件名和测试结果统一为 `1.0.1`。

## 测试整改

- T1 文件结构
- T2 元数据契约
- T3 产品输入、流程、输出与边界契约
- T4 确定性输入校验和计算执行
- T5 正常、缺失、冲突、敏感信息、非法 JSON 场景
- T6 秘密、敏感凭据、收费 API 和内部路径扫描
- T7 ZIP 清单、Apache-2.0 许可证、第三方声明和 SHA-256

每条证据均记录输入、执行方式、预期、实际和判定。模型提示词未冒充平台运行测试。
