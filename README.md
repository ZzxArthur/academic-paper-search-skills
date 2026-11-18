# Academic Paper Search Skill

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Awesome Agent Skills](https://img.shields.io/badge/Agent_Skills-Ready-brightgreen.svg)](#)
[![Multi-Platform](https://img.shields.io/badge/Platform-Codex%20%7C%20Antigravity%20%7C%20Cursor%20%7C%20Claude-orange.svg)](#)
[![Codex](https://img.shields.io/badge/OpenAI_Codex-Supported-black.svg)](#)

> **为科研探索量身定制的 AI 文献调研工作流**：将模糊的研究诉求转化为层次化、可比对、可验证的文献知识图谱与空白创新点挖掘报告。

---

## ⚡ 一键极速安装 (Quick One-Liner)

无需繁琐配置，在终端执行以下一行命令，将**自动检测本机已安装的 AI 编程环境（Codex / Antigravity / Claude Code）并自动完成全局技能挂载**：

```bash
curl -fsSL https://raw.githubusercontent.com/ZzxArthur/academic-paper-search-skills/main/install.sh | bash
```

---

## 🌟 核心特色与解决痛点

在进行学术文献调研时，常规大模型通常直接罗列论文标题，缺乏上下文梯度与证据核验。本技能通过标准化五步法解决这一问题：

1. **宽泛主题澄清机制**：识别宏观主题，主动提示选择最新综述或具体子方向，避免信息过载。
2. **渐进式阅读次序**：按「奠基开创 $\to$ 架构解耦 $\to$ 最新 SOTA」组织阅读路径，而非单纯按发表时间堆砌。
3. **真实性与开源核验**：严格核对正式录用状态（预印本/顶会/期刊）及官方代码仓库，不编造虚假信息。
4. **多维特征对比矩阵**：横向对比核心机制与能力维度，使用 `✓` / `✗` 明确标注技术实现。
5. **融合创新空白挖掘**：基于矩阵空白交叉点，审慎推导尚未有人探索的交叉研究方向与最小验证方案。

---

## 📋 仓库文件结构

```text
academic-paper-search-skills/
├── SKILL.md                  # 核心技能规范（符合 Agent Skill 标准）
├── install.sh                # 跨平台一键自动化安装脚本
├── references/
│   └── REPORT_TEMPLATE.md    # 标准文献调研报告模板
├── adapters/                 # 跨平台一键适配配置
│   ├── .cursorrules          # Cursor 适配规则
│   ├── CLAUDE.md             # Claude Code 适配规则
│   └── system_prompt.txt     # 通用 Web 大模型系统提示词
├── examples/
│   └── embodied_ai_vla_demo.md # 实测示例：具身智能 VLA 基础模型 10 篇精选调研
├── README.md
└── LICENSE
```

---

## 🚀 跨平台使用指引

### 1. OpenAI Codex 用户
本技能深度兼容 Codex 的技能机制：
- **一键极速安装**：
  ```bash
  curl -fsSL https://raw.githubusercontent.com/ZzxArthur/academic-paper-search-skills/main/install.sh | bash -s -- --codex
  ```
- **手动安装方式**：
  将技能文件放入 Codex 全局配置库：
  ```bash
  mkdir -p ~/.codex/skills/academic-paper-search
  cp SKILL.md ~/.codex/skills/academic-paper-search/
  cp -r references ~/.codex/skills/academic-paper-search/
  ```
安装后，Codex 会在会话中自动识别学术论文检索指令并执行本规范。

### 2. Antigravity 用户
运行一键安装脚本，或手动复制到全局配置目录：
```bash
cp -r . ~/.gemini/config/skills/academic-paper-search
```

### 3. Cursor 用户
直接将 `adapters/.cursorrules` 复制到当前项目根目录下：
```bash
cp adapters/.cursorrules /path/to/project/.cursorrules
```

### 4. Claude Code 用户
复制到项目根目录的 `CLAUDE.md` 或全局 `~/.claude/skills/` 即可生效。

### 5. ChatGPT / Claude / DeepSeek 网页端
复制 `adapters/system_prompt.txt` 的内容作为智能体系统的预设 System Prompt。

---

## 💡 真实案例演示

在 `examples/embodied_ai_vla_demo.md` 中查看基于本技能生成的完整分析报告：
- **主题**：具身智能·视觉-语言-动作（VLA）基础模型
- **规模**：10 篇里程碑与最新顶会工作（RT 系列、Octo、OpenVLA、$\pi_0$ 等）
- **产出**：循序渐进阅读链条、八维能力对比矩阵、视-触-语-动融合方向推导

---

## 📄 开源许可证

本项目基于 MIT 许可证开源。
