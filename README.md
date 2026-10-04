# Hyperbolica 简体中文汉化

非官方汉化测试版，版本 **v0.1.0-beta**。采用手动覆盖游戏资源的安装方式。

[下载 v0.1.0-beta](https://github.com/Souls-R/hyperbolica-zh/releases/tag/v0.1.0-beta) · [Release 列表](https://github.com/Souls-R/hyperbolica-zh/releases) · [SHA-256 校验清单](https://github.com/Souls-R/hyperbolica-zh/releases/download/v0.1.0-beta/SHA256SUMS.txt)

## 适用版本与汉化范围

- 游戏：Hyperbolica **1.1.9**，**Windows Steam 版，Build ID 8675290**。
- 覆盖 **22 个文本资源、3,585 条显示行**，包括菜单、NPC 对白、选择项、纪念品和提示。
- 贴图中的英文保留原样。
- 安装包提供 **13 个修改后的资源文件**：`Hyperbolica_Data/sharedassets0.assets` 和 `Hyperbolica_Data/level0` 至 `level11`。
- 这 13 个资源文件的替换不写入用户存档。

其他游戏版本及平台尚未验证。Steam 更新后，请先确认游戏版本与本包匹配。

## 当前验证情况

此前测试构建的菜单、存档和一条黄色 NPC 长对白已通过实机检查，包括长对白的换行显示。文本和排版也做过结构与静态检查，但尚未完成全部剧情、分支、结局和 VR 模式的全流程验收。

公开版字体构建及静态检查已完成：中文轮廓、字宽和原 UI 全局度量与此前测试构建一致；两份等宽字体的拉丁字形改用官方 OFL Roboto Mono，并适配原界面的固定框。**公开字体版尚未实机复核。**

## 安装

1. 关闭 Hyperbolica。
2. 打开游戏安装目录，确认其中有 `Hyperbolica.exe`。
3. 将压缩包中的 `Hyperbolica_Data` 文件夹合并到这个目录，完整替换上述 **13 个同名文件**，保留其他游戏文件。
4. 启动游戏，检查菜单和对白显示。

可选：覆盖前，将这 13 个原版资源文件备份到游戏目录外。备份已经汉化的文件只能恢复到对应汉化版本。

## 更新、冲突与恢复英文

同一游戏版本更新汉化时，完整覆盖新版的 13 个文件。修改相同资源文件的其他补丁会互相覆盖；已有此类修改时，建议先恢复官方文件，再安装本包。

Steam 更新或验证游戏文件可能覆盖汉化。游戏 Build ID 改变后，请等待或确认对应版本的汉化包。

恢复英文或处理覆盖不完整的问题：在 Steam 库中右键 Hyperbolica，选择 **属性 → 已安装文件 → 验证游戏文件完整性**，等待 Steam 检查并修复官方资源。[Steam 官方指引](https://help.steampowered.com/en/faqs/view/0C48-FCBD-DA71-93EB)

## 翻译与排版工作流

翻译初稿由 AI 生成，并经过统一术语表、参考资料核对、多轮 AI 交叉审校和脚本结构检查。几何术语、人物称呼及反复出现的概念尽量统一；几何笑话同时考虑含义与中文表达。可查阅[术语表](glossary.json)与[参考来源](references.txt)。

结构检查覆盖对话键、条件、事件、选择跳转、暂停、演出分组和物理页边界。对白排版在构建时处理换行及中文行首、行尾禁则，不改写这些剧情控制结构。AI 审校与抽样实机测试仍可能遗漏问题，欢迎通过 [Issues](https://github.com/Souls-R/hyperbolica-zh/issues) 反馈译文、缺字或布局问题。

## 字体及许可

公开版使用以下 **SIL Open Font License 1.1（OFL）** 字体组合：

| 字体组件 | 公开版用途 | 字体许可 |
| --- | --- | --- |
| Raleway | 与 Noto 中文字形组合，用于对应菜单与界面字体 | SIL OFL 1.1 |
| Roboto Mono | 为两份等宽字体提供拉丁字形，与 Noto 中文字形组合，并适配原界面的固定框 | SIL OFL 1.1 |
| Noto Sans SC | 提供中文及相应标点字形 | SIL OFL 1.1 |

字体静态检查确认中文轮廓、字宽和原 UI 全局度量与此前测试构建一致；公开字体版尚未实机复核。字体修改、版权及许可信息见 [THIRD_PARTY_NOTICES.txt](THIRD_PARTY_NOTICES.txt) 和 [licenses](licenses/)。

## 非官方说明与游戏资源权利

本项目为非官方汉化，与 CodeParade 无官方关联。Hyperbolica 及发布包中原游戏内容的权利归 **CodeParade**；13 个修改后资源包含原游戏未修改的内容。字体 OFL 许可仅适用于字体，不为游戏资源授予新许可；本项目不声称已取得游戏资源再分发授权。
