# Gamer 配置包仓库

公开配置包通过 GitHub Releases 分发。请下载 `.gamerpkg`，在 Gamer 的「配置包 → 导入」中安装。

支持仓库源的 Gamer 版本可在「配置包」页添加 `https://github.com/jesongit/gamer-packages`，读取最新正式 Release 的完整目录。

## 发布约定

使用 Gamer「配置包发布」插件，选择配置、目标仓库并生成预览，再创建草稿、检查并公开。发布者使用运行 Gamer 的电脑上的 GitHub CLI 登录。

每个正式 Release 包含 `packages.json`、`SHA256SUMS.txt` 与目录中的全部当前版本 `.gamerpkg`。目录版本独立于配置包版本；修改包内容必须提升包内版本号，已发布资产不覆盖。

仓库初始的 `publisher-smoke` 是发布和导入闭环验收用示例，不包含脚本、设备信息或个人数据。

同 ID 配置导入会提示覆盖本地修改，更新前可以先导出备份。导入配置不会自动运行脚本，也不会自动安装依赖插件。