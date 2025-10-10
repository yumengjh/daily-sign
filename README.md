# 每日签到

每天自动提交代码

[EN](https://github.com/yumengjh/daily-sign/blob/main/README-en.md)

## 步骤一：Fork 仓库

点击右上角 “Fork” → 复制到你的 GitHub 账号。

## 步骤二：添加 Secrets

打开仓库 → Settings → Secrets and variables → Actions → New repository secret
添加以下两个变量：

| 名称         | 示例值       | 说明                                  |
| ------------ | ------------ | ------------------------------------- |
| `USERNAME`   | `yumengjh`   | 你的 GitHub 用户名（区分大小写）      |
| `PUSH_TOKEN` | `ghp_xxx...` | 个人访问令牌（PAT），需有 `repo` 权限 |

创建 PAT 的方法：

进入 https://github.com/settings/tokens

点击 “Generate new token (classic)”

勾选 repo 权限，生成后复制保存。

## 步骤三：查看自动打卡

每天北京时间 0 点（UTC 16 点）
GitHub Actions 会自动运行一次，
并在 README 中追加一行类似：

- 2025-10-10 00:00:00

脚本会自动在 `## record` 下面追加日期

记录区 ↓

## record
- 日期
- 日期
- 日期
- ... 

