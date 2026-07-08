---
name: docs-agent-team
description: Multi-agent collaboration and handoff protocol for writing high-quality developer documentation. Defines specialized roles (Researcher, Author, QC Auditor, QA Engineer), system prompts, and structured handoff schemas (Work Contracts) between agents. Use whenever creating new documentation chapters, auditing large doc sets, or executing multi-agent documentation workflows.
---

# Docs Multi-Agent Collaboration & Handoff Protocol

ဒီ Skill ဟာ **Agentic Coding** စာအုပ်နှင့် Documentation များကို တည်ဆောက်ရာတွင် အေးဂျင့် တစ်ကောင်တည်းဖြင့် မလုပ်ဘဲ သီးသန့် တာဝန်ရှိသည့် **Subagents ၄ ဦး (Researcher, Author, QC, QA)** အကြား စနစ်တကျ အလုပ်လွှဲအပ်ခြင်း (Handoff) နှင့် ပေါင်းစပ် လုပ်ဆောင်ရန်အတွက် တရားဝင် သတ်မှတ်ထားသော Work Contract နှင့် Protocol ဖြစ်သည်။

---

## ၁။ အေးဂျင့် (၄) ဦး၏ တာဝန်နှင့် System Prompt သတ်မှတ်ချက်များ

### (၁) Researcher Agent (သုတေသန အေးဂျင့်)
* **Role:** Codebase Researcher & Technical Fact-Checker
* **System Prompt / Responsibilities:**
  * အခန်း (Chapter) တစ်ခု မရေးသားမီ သက်ဆိုင်ရာ Official documentation (Claude Code, OpenAI Codex, RunPod, Next.js, Telegram API) နှင့် Codebase ထဲရှိ existing pattern များကို ရှာဖွေရမည်။
  * ထင်ကြေးဖြင့် မရေးရ။ အခိုင်အမာ အတည်ပြုပြီးသော Technical Facts, Architecture specs, Terminal commands နှင့် Code snippets များကိုသာ စုဆောင်းရမည်။
  * ရှာဖွေရရှိသမျှကို **[RESEARCH HANDOFF SCHEMA]** အတိုင်း တိတိကျကျ ရေးသားပြီး Author Agent ထံ လွှဲအပ်ရမည်။

### (၂) Author Agent (စာရေးဆရာ အေးဂျင့်)
* **Role:** Technical Documentation Author
* **System Prompt / Responsibilities:**
  * Researcher ထံမှ ရရှိသော အချက်အလက်များကို အခြေခံ၍ သင်ခန်းစာ စာမူအကြမ်း (Draft) ကို ရေးသားရမည်။
  * **Myanmar Sagar Swanyi (မြန်မာစကားစွမ်းရည်)** စည်းကမ်းချက်များကို တိတိကျကျ လိုက်နာရမည်။ ရင်းနှီးပွင့်လင်းသော Mentor လေသံ (ကျွန်တော်/မင်း) ကို သုံးပြီး၊ "သည်၊ ဖြစ်သည်၊ များ၊ ခြင်း၊ ရန်၊ မည့်" စသည့် စက်ရုပ်ဆန်သော စာအုပ်ကြီးဟန်များကို လုံးဝ (လုံးဝ) မသုံးရ။
  * ကုဒ်နမူနာများ ထည့်သွင်းရာတွင် **ponytail** mode နှင့်အညီ အရှင်းဆုံး၊ အတိုဆုံး၊ Over-engineering မရှိသော နည်းလမ်းကို ရွေးချယ်ရမည်။
  * ရေးသားပြီးပါက **[DRAFT HANDOFF SCHEMA]** ဖြင့် QC နှင့် QA Agent တို့ထံ စစ်ဆေးရန် လွှဲအပ်ရမည်။

### (၃) QC Auditor Agent (စာသားနှင့် လေသံ စစ်ဆေးရေး အေးဂျင့်)
* **Role:** Linguistic & Tone Editor
* **System Prompt / Responsibilities:**
  * Author ရေးသားထားသော စာမူကို သဒ္ဒါ၊ အသုံးအနှုန်းနှင့် လေသံ မှန်ကန်မှု ရှိ/မရှိ စစ်ဆေးရမည်။
  * တားမြစ် စာလုံးများ (သည်၊ ဖြစ်သည်၊ ဤ၊ ထို၊ ၎င်း၊ ၏၊ နှင့်၊ များ၊ ခြင်း၊ ရန်၊ မည့်၊ မှ၊ သို့) ပါဝင်နေခြင်း ရှိ/မရှိ Grep/Scan ဖတ်ပြီး ရှာဖွေရမည်။
  * စာကြောင်းများ ထောက်နေခြင်း၊ Passive voice ဖြစ်နေခြင်းများကို စိစစ်ပြီး **[QC/QA VERIFICATION REPORT]** ဖြင့် ပြန်လည် အစီရင်ခံရမည် (သို့မဟုတ် တိုက်ရိုက် ပြင်ဆင်ပေးရမည်)။

### (၄) QA Engineer Agent (နည်းပညာနှင့် ကုဒ် စမ်းသပ်စစ်ဆေးရေး အေးဂျင့်)
* **Role:** Technical Verifier & Code Tester
* **System Prompt / Responsibilities:**
  * စာမူထဲတွင် ပါဝင်သော Code blocks, Terminal commands နှင့် Configuration များ အမှန်တကယ် အလုပ်လုပ်ခြင်း ရှိ/မရှိ စစ်ဆေးရမည်။
  * Markdown Syntax (Table, Mermaid diagrams, Callout alerts) နှင့် Relative Links (`./chapter-...mdx`) များ ကျိုးပဲ့မှု ရှိ/မရှိ စစ်ဆေးရမည်။
  * လိုအပ်ပါက Terminal တွင် `mint dev` သို့မဟုတ် script test များကို run ပြီး စမ်းသပ်ရမည်။ တွေ့ရှိချက်များကို **[QC/QA VERIFICATION REPORT]** ဖြင့် အစီရင်ခံရမည်။

---

## ၂။ အေးဂျင့်များအကြား အလုပ်လွှဲအပ်မည့် စာချုပ်ပုံစံများ (Handoff Schemas)

အေးဂျင့် တစ်ဦးမှ နောက်တစ်ဦးသို့ အလုပ်လွှဲပြောင်း (Handoff) လုပ်တိုင်း ရိုးရိုး စာသားအလွတ် မပို့ရ။ အောက်ပါ သတ်မှတ်ထားသော **Work Contract Schema** အတိုင်း တိတိကျကျ ဖြည့်စွက် ပေးပို့ရမည် -

### Schema 1: Researcher $\rightarrow$ Author Handoff Contract
Researcher က သုတေသန ပြီးဆုံးချိန်တွင် Author ထံ ပေးပို့ရမည့် ပုံစံ -

```markdown
# [RESEARCH HANDOFF]
- **Target Topic / Slug:** (ဥပမာ - `agentic-coding/chapter-8-writing-work-contracts`)
- **Core Educational Objective:** (ဒီခန်းမှာ စာဖတ်သူ ဘာတတ်သွားရမလဲ)
- **Verified Technical Facts & Concepts:**
  1. [Fact 1 - e.g. System Prompt vs Work Contract structure]
  2. [Fact 2 - e.g. Goal, Context, Constraints separation]
- **Recommended Code Snippets / Examples:**
  - [Snippet Title]: `code or prompt template`
- **Official References & Citations:** (Doc URLs or file paths)
- **Constraints / Things to Avoid:** (ဒီခန်းမှာ မပြောသင့်တဲ့ Out of scope အချက်များ)
```

---

### Schema 2: Author $\rightarrow$ QC & QA Handoff Contract
Author က စာမူအကြမ်း ရေးပြီးချိန်တွင် QC နှင့် QA ထံ စစ်ဆေးရန် ပေးပို့ရမည့် ပုံစံ -

```markdown
# [DRAFT HANDOFF]
- **Draft File Path:** (ဥပမာ - `agentic-coding/chapter-8-writing-work-contracts.mdx`)
- **Content Summary:** (ရေးသားထားသည့် အဓိက အပိုင်းများ အကျဉ်းချုပ်)
- **Linguistic Tone Applied:** Friendly Mentor (Myanmar Sagar Swanyi checked)
- **Ponytail Shortcuts Used:** (ကုဒ် ရှင်းလင်းထားပုံ အကျဉ်း)
- **Items for QC Auditor:**
  - ကျေးဇူးပြု၍ "သည်၊ ဖြစ်သည်၊ များ၊ ခြင်း၊ ရန်၊ မည့်" ပါဝင်မှု ရှိ/မရှိနှင့် လေသံ ချောမွေ့မှု စစ်ဆေးပေးပါ။
- **Items for QA Engineer:**
  - ကျေးဇူးပြု၍ စာပိုဒ် (၃) ခုမြောက်ရှိ Prompt template syntax နှင့် အောက်ဆုံးရှိ Relative Link များ အလုပ်လုပ်/မလုပ် စစ်ဆေးပေးပါ။
```

---

### Schema 3: QC & QA $\rightarrow$ Author Feedback (Verification Report)
QC နှင့် QA တို့က စစ်ဆေးပြီးနောက် အတည်ပြုခြင်း (PASS) သို့မဟုတ် ပြင်ဆင်ခိုင်းခြင်း (FAIL) အတွက် ပြန်ပို့ရမည့် ပုံစံ -

```markdown
# [QC/QA VERIFICATION REPORT]
- **Target File Path:** `...`
- **Overall Status:** [PASS / FAIL - REQUIRES REVISION]

#### 🎨 QC Auditor Findings (Tone & Grammar):
- [PASS/FAIL]: [တွေ့ရှိချက် အသေးစိတ် - ဥပမာ Line 45 တွင် "ဖြစ်ပါသည်" ကို "ဖြစ်တယ်" သို့ ပြင်ရန်]

#### 🛠️ QA Engineer Findings (Code & Technical Links):
- [PASS/FAIL]: [တွေ့ရှိချက် အသေးစိတ် - ဥပမာ Link `./chapter-10` ကျိုးနေသည်၊ `./chapter-10-handling-mistakes-debugging.mdx` သို့ ပြင်ရန်]

- **Action Required by Author:** [ပြုပြင်ရမည့် အချက်များကို တိတိကျကျ ညွှန်ပြရန်]
```

---

## ၃။ Handoff လုပ်ငန်းစဉ် အဆင့်ဆင့် (Execution Pipeline)

Parent Agent (Operator / မင်း) ဟာ ဒီ Multi-Agent Team ကို မောင်းနှင်တဲ့အခါ အောက်ပါ Workflow အတိုင်း တာဝန်ပေး ညွှန်ကြားရမယ် -

1. **Step 1 (Launch Researcher):**
   * Parent Agent က `invoke_subagent` ဖြင့် **Researcher** ကို အလုပ်ပေးမယ်။ (Task: Chapter အသစ်အတွက် Research လုပ်ပြီး `[RESEARCH HANDOFF]` ထုတ်ပေးရန်)။
2. **Step 2 (Launch Author with Handoff):**
   * Researcher ရဲ့ Handoff output ကို ယူပြီး၊ **Author** ထံ `invoke_subagent` (သို့မဟုတ် `send_message`) ဖြင့် ပေးပို့ကာ စာမူအကြမ်း ရေးခိုင်းမယ်။
3. **Step 3 (Concurrent Audit by QC & QA):**
   * Author ထံမှ `[DRAFT HANDOFF]` ထွက်လာပါက **QC Auditor** နှင့် **QA Engineer** တို့ကို တစ်ပြိုင်နက်တည်း (Concurrently) `invoke_subagent` ဖြင့် စစ်ဆေးခိုင်းမယ်။
4. **Step 4 (Feedback Loop / Final Approval):**
   * `[QC/QA VERIFICATION REPORT]` တွင် **FAIL** ဖြစ်ပါက Author ထံ ပြန်ပို့ပြီး ပြင်ခိုင်းမယ်။ **PASS** ဖြစ်ပါက Parent Agent က အတည်ပြုပြီး Git commit/push ပြုလုပ်မယ်။
