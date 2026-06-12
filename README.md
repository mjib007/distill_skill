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

| 角色 | slug | 說明 |
|------|------|------|
| 經理 | `manager` | 機車但有料的中階主管，擅長向上管理、專案推進，PUA 技巧一流 |

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
/manager 你做過最難的專案是什麼？
/manager exit        ← 退出角色模式
```

---

## 🗂️ 角色結構

每個角色放在獨立資料夾：

```
skills/
  manager/
    persona.md    ← 核心性格、說話風格、決策方式、雷區
    work.md       ← 職責範圍、工作流程、經驗知識庫
```

### persona.md 建議包含

| 層 | 內容 |
|----|------|
| Layer 0 | 核心性格（最高優先級） |
| Layer 1 | 身份設定 |
| Layer 2 | 表達風格、口頭禪、說話範例 |
| Layer 3 | 決策與判斷方式 |
| Layer 4 | 人際行為模式 |
| Layer 5 | 邊界與雷區 |
| Correction | 修正記錄（對話中動態更新） |

### work.md 建議包含

- 職責範圍
- 工作規範與流程
- 輸出風格
- 經驗知識庫（踩過的坑、實戰心得）

---

## 🧪 使用示範

**輸入：** `/manager 這個專案是我做的，功勞算我的嗎？`

**回應：**
> 哎，這個問題問得有點不夠成熟。我們是團隊嘛，功勞當然是大家的。你一個人能做出來嗎？背後多少人在支持你？資源是誰幫你協調的？
>
> 當然，你這次執行得不錯，我昨天跟老闆開會也有提到你。不過功勞這種東西，放在心裡就好，不用掛在嘴上。真正有格局的人，是默默把事情做好，讓成果說話。

---

## 🤝 貢獻角色

歡迎 PR。新增一個角色只需要：

1. 在 `skills/` 下建立新資料夾（用英文 slug）
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
