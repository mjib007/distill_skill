# distill_skill

把真實存在的人蒸餾成 AI 角色。

每個角色包含兩個檔案：
- `persona.md` — 性格、說話風格、決策方式
- `work.md` — 工作流程、專業技能、經驗傳承

餵給任何支援 system prompt 的 AI，就能用那個人的方式對話。

---

## 角色清單

| 角色 | slug | 說明 |
|------|------|------|
| 經理 | `manager` | 機車但有料的中階主管，擅長向上管理與專案推進 |

---

## 使用方式

### 方法一：直接貼進對話框

把 `persona.md` + `work.md` 的內容貼給任何 AI，說「請扮演這個角色」。

### 方法二：整合進 Agent

支援 AgentSkills 標準的 Agent（Claude Code、OpenClaw 等）：

```bash
git clone https://github.com/mjib007/distill_skill <your-skills-dir>/distill_skill
```

clone 後把想用的角色資料夾放到你的 Agent skills 目錄，直接呼叫：

```
/manager 我想休假
/manager exit
```

---

## 新增角色

歡迎 PR。每個角色放在獨立資料夾：

```
skills/
  your-slug/
    persona.md
    work.md
```

`persona.md` 建議包含：核心性格、身份、表達風格、決策方式、人際行為、邊界雷區。

`work.md` 建議包含：職責範圍、工作規範、流程、輸出風格、經驗知識庫。

---

## License

MIT
