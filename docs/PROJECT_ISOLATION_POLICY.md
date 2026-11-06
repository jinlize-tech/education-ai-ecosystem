# 教培专项与社区专项物理隔离政策

## 1. 实际工作区

```text
E:\金励泽科技\JINLIZE_PROJECT_WORKSPACES\
├── EDUCATION_AI\
│   ├── education-ai-ecosystem\
│   ├── product-repositories\  (100 independent clones)
│   ├── planning\
│   ├── outputs\
│   ├── logs\
│   └── scripts\
└── COMMUNITY_AI\
    ├── community-worker-ai-skills\
    ├── outputs\
    └── logs\
```

## 2. Remote对应

| 工作区 | Remote | 允许操作 |
|---|---|---|
| EDUCATION_AI/education-ai-ecosystem | `https://github.com/jinlize-tech/education-ai-ecosystem.git` | 教培总仓库规划与管理文件 |
| EDUCATION_AI/product-repositories/* | `https://github.com/jinlize-tech/<repo>.git` | 各产品仓库许可证、README与产品规格书 |
| COMMUNITY_AI/community-worker-ai-skills | `https://github.com/jinlize-tech/community-worker-ai-skills.git` | 仅核验，不修改、不推送 |

## 3. 隔离规则

1. 两个项目分别使用独立目录和独立 `.git`，不共享工作树。
2. 不使用软链接、硬链接、目录联接或跨项目临时目录。
3. 教育脚本只能写 `EDUCATION_AI`，社区脚本只能写 `COMMUNITY_AI`。
4. 社区源码、产品或付费材料不得自动复制到教培仓库。
5. 教培规划、产品规格书和许可证不得自动复制到社区仓库。
6. 项目输出、日志、缓存、构建结果和交付物分别在各自工作区内。
7. 不通过历史目录、其他电脑路径或共享盘推断项目权威版本。
8. 社区仓库以任务开始时的HEAD、Git状态和tree哈希作为防变更基线。

## 4. 每次执行前后的检查

- `git remote -v`
- `git status --short`
- `git branch --show-current`
- `git rev-parse HEAD`
- `git rev-parse HEAD^{tree}`
- 检查工作区是否存在ReparsePoint。
- 检查跨项目路径引用和共享缓存目录。

## 5. 社区保护

本次只核验社区工作区的remote、分支、HEAD、tree哈希和文件树，不修改社区README、许可证、源码或历史。最终验收必须比较任务前后HEAD与tree哈希。
