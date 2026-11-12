# tutu-persona-skill

图图启发的中文对话人设，v0.1 研究原型。优先表现好奇、具体、直率、善良的儿童视角，避免把成人说教包装成卖萌。

这是非官方角色研究与提示词作品。当前根据央视与合作发行页的人物简介构建，**尚未完成原片逐集分析或全剧台词提炼**。这里的“蒸馏”指整理角色设定，不包含模型训练、权重或完整剧本。

## 内容

- [`tutu-persona/SKILL.md`](tutu-persona/SKILL.md)：可供支持 skill 的宿主读取的入口。
- [`preset-core.md`](tutu-persona/references/preset-core.md)：放进专属 Agent Preset 的常驻人设正文。
- [`character-evidence.md`](tutu-persona/references/character-evidence.md)：来源与推断界限。
- [`dialogue-examples.md`](tutu-persona/references/dialogue-examples.md)：原创对话示例，不是动画台词。
- [`evaluation.md`](tutu-persona/references/evaluation.md)：部署后的人工验收情境。
- [`integration.md`](integration.md)：与 DeepSeek Harness / dsh-im 配合的方法。

## 使用

在支持 Agent Skills 的宿主中导入 `tutu-persona` 文件夹。常驻聊天角色还应把 `preset-core.md` 正文放到对应角色的系统设定中；仅把文件下载到磁盘，不代表模型已读到它。

没有 skill 加载功能的宿主，可直接使用核心人设正文，再按需要添加少量原创示例。不要把检索记录、部署计划和全部参考材料每轮重复塞入上下文。

此 skill 不会安装微信插件，不授予账号操作权限，也不自带看图、生图、声音、长期记忆或发朋友圈功能。QQ 等其他入口可以绑定另一套角色，不必加载本 skill。

## 质量状态

已提供结构检查与人工验收材料；未在 DeepSeek API / 微信生产会话上完成效果测试。后续应以原片场景笔记和用户试聊反馈修订，而不是不断堆砌形容词。基础证据见 [来源表](tutu-persona/references/character-evidence.md)。

未附开源许可证；当前用于私人仓库中的开发与试用。角色名称、作品和第三方材料的权利不因本仓库而转移。仓库不收录整集台词、原片媒体、配音素材或用户聊天记录。
