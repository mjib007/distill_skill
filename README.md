# 🧬 distill_skill｜人物蒸餾技能庫

![Profile views](https://komarev.com/ghpvc/?username=mjib007&label=Profile%20views&color=4c8eda&style=flat)
[![Stars](https://img.shields.io/github/stars/mjib007/distill_skill?style=flat&color=yellow)](https://github.com/mjib007/distill_skill/stargazers)
[![Forks](https://img.shields.io/github/forks/mjib007/distill_skill?style=flat&color=blue)](https://github.com/mjib007/distill_skill/network/members)
![AI](https://img.shields.io/badge/AI-GPT--4o%20%7C%20Claude-blueviolet)
![Platform](https://img.shields.io/badge/Platform-OpenClaw%20%7C%20Claude%20Code%20%7C%20任意%20AI-orange)
![Language](https://img.shields.io/badge/Language-繁體中文-red)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)
![Status](https://img.shields.io/badge/status-active-success)

> 把真實存在的人蒸餾成 AI 角色。每個角色兩個檔案，餵給任何 AI 就能用那個人的方式對話。

---

## ✨ 功能特色

- 🧠 **雙層架構**：`persona.md`（人格）+ `work.md`（工作技能），分開管理、各司其職
- 🎭 **完整人格**：涵蓋說話風格、決策方式、雷區、口頭禪，不只是表面模仿
- 💼 **工作傳承**：流程、規範、踩過的坑、經驗知識庫，離職帶不走的隱性知識
- 🔌 **跨平台通用**：支援 OpenClaw、Claude Code、Codex，或直接貼進任何 AI 對話框
- 📦 **持續新增**：每個角色獨立資料夾，歡迎 PR 貢獻新角色

---

## 📁 角色清單

### 🧑‍💼 colleague｜職場類

| 角色 | slug | 說明 |
|------|------|------|
| 經理 | `manager` | 機車但有料的中階主管，擅長向上管理、專案推進，PUA 技巧一流 |
| 新創 CEO | `startup-ceo` | Pre-seed 階段、永遠在 pivot、給不起薪水但股票管夠，AI 掛嘴邊 |

### 💞 relationship｜關係類

| 角色 | slug | 說明 |
|------|------|------|
| （陸續新增中） | — | — |

### 🌟 celebrity｜公眾人物類

| 角色 | slug | 說明 |
|------|------|------|
| （陸續新增中） | — | — |

---

## 🚀 使用方法

### 方法一：直接貼進對話框（最快）

把 `persona.md` + `work.md` 的內容貼給任何 AI，說「請完全扮演這個角色，用第一人稱說話」。

### 方法二：整合進 Agent（推薦）

支援 AgentSkills 標準的 Agent（OpenClaw、Claude Code 等）：

```bash
git clone https://github.com/mjib007/distill_skill <your-skills-dir>/distill_skill
```

clone 後把角色資料夾放到你的 Agent skills 目錄，直接呼叫：

```
/manager 我想休假
/startup-ceo 你們 revenue 多少？
/manager exit        ← 退出角色模式
```

---

## 🗂️ 角色結構

```
skills/
  colleague/          ← 職場類
    manager/
    startup-ceo/
  relationship/       ← 關係類
  celebrity/          ← 公眾人物類
```

每個角色包含：

| 檔案 | 內容 |
|------|------|
| `persona.md` | 核心性格、說話風格、決策方式、雷區（Layer 0–5） |
| `work.md` | 職責範圍、工作流程、輸出風格、經驗知識庫 |

---

## 🧪 使用示範

**輸入：** `/startup-ceo 你們 revenue 多少？`

**回應：**
> 好問題！這個問題問得很有深度。我們現在 focus 的不是 revenue，我們 focus 的是 product-market fit。你知道嗎，Amazon 前七年都在虧損，但 Bezos 從來沒有因為這樣就停下來。我們現在在做的事情，本質上是在教育市場，這需要時間。
>
> 但我可以跟你說，我們的 user engagement 數據非常漂亮。你有沒有興趣看一下我們最新的 pitch deck？我昨晚剛更新了 market size 的部分，TAM 比我們想的大很多。

---

## 🤝 貢獻角色

歡迎 PR。新增一個角色只需要：

1. 在對應分類下建立新資料夾（`skills/colleague/your-slug/`）
2. 放入 `persona.md` 和 `work.md`
3. 在 README 的角色清單加一行

---

## 📜 授權

本專案以 [MIT License](LICENSE) 開源，歡迎自由使用、修改與分享。
若有改善建議，歡迎提交 Issue 或 Pull Request。

---

## 🔗 相關專案

- [🦞 OpenClaw](https://github.com/mjib007/openclaw)
- [⚖️ LegalMind AI](https://github.com/mjib007/legalmind-ai)
- [📐 法學論文大綱審查工具](https://github.com/mjib007/legal-thesis-outline)
