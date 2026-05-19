# SST-TOUFANG-SKILL

一个面向广告投放、买量、ROI、素材、归因、平台算法、IAA/IAP/混合变现和投放团队管理场景的中文 Skill。

当前版本已按工作区“何俊杰”文件夹中的 771 篇文章重新校准，重点补强了预算与客群质量、素材系统、归因口径、平台与 MMP 数据对齐、IAA/IAP/混合变现、管理诊断，以及平台 AI 化趋势等主题。

## 适用场景

- 广告投放分析
- 买量与流量获取
- ROI 异常排查
- 素材迭代与疲劳判断
- 预算、出价、账户结构与放量节奏
- 归因窗口、MMP、AppsFlyer、SAN、SKAN、回传口径
- IAA / IAP / 混合变现
- 小红书、巨量、广点通、应用商店、Facebook、TikTok、Google、Meta
- 投放团队管理、复盘、述职与数据体系建设

## 仓库结构

```text
.
├─ SKILL.md
├─ references/
│  ├─ frameworks.md
│  ├─ problem-playbooks.md
│  ├─ source-map.md
│  └─ style-guide.md
├─ evals/
│  └─ evals.json
├─ agents/
│  └─ openai.yaml
└─ README.md
```

## 文件说明

- `SKILL.md`：主技能定义，包含触发范围、回答原则、默认诊断顺序、输出结构和专题要求。
- `references/frameworks.md`：底层分析框架与核心判断原则。
- `references/problem-playbooks.md`：高频问题作战卡，适合按场景快速拆题。
- `references/source-map.md`：语料来源与主题映射。
- `references/style-guide.md`：回答语气、节奏和表达习惯说明。
- `evals/evals.json`：评测样例。
- `agents/openai.yaml`：显式调用时的 OpenAI agent 元信息。

## 安装方式

如果你在 Codex 或兼容 Skill 目录结构的环境里使用，可以把这个仓库直接放到本地 Skill 目录下，例如：

```text
~/.codex/skills/SST-TOUFANG-SKILL
```

也可以直接克隆：

```bash
git clone https://github.com/sickboy555/-skill.git SST-TOUFANG-SKILL
```

然后确保目录里保留 `SKILL.md`、`references/`、`evals/` 这几个核心部分即可。

## 使用建议

- 当用户的问题本质是投放、买量、流量、素材、归因、回收、平台算法或团队管理时，优先启用这个 Skill。
- 显式唤醒时，优先使用 `$SST-TOUFANG-SKILL`。
- 回答时不要只给动作，先判断问题属于哪一层，再给优先排查项和不建议动作。
- 遇到平台后台、MMP、SAN、SKAN 数据不一致的问题，先对齐统计口径，再讨论优化动作。

## 说明

这个仓库当前以 Skill 发布为主，保持了适合直接导入的目录结构，方便后续继续补充 `references` 和 `evals`。
