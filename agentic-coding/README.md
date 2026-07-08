# Agentic Coding Outline (Project Book)

ဒီ Folder (`/agentic-coding`) က Myanmar learners တွေအတွက် AI Coding Agent တွေဖြစ်တဲ့ **Claude** နဲ့ **Codex** တို့ကို သုံးပြီး Idea ကနေ ပြီးပြည့်စုံတဲ့ Working App တစ်ခုအထိ စနစ်တကျ တည်ဆောက်တတ်စေဖို့ ရေးသားထားတဲ့ စာအုပ်/သင်ခန်းစာ Project Book ရဲ့ ပင်မ လမ်းညွှန် (README) ဖြစ်တယ်။

---

## Writing Guidelines & Tone (မြန်မာစကားစွမ်းရည် စည်းကမ်းများ)

ဒီ Project Book ထဲက သင်ခန်းစာ အားလုံးကို အောက်ပါ **Myanmar Sagar Swanyi** (မြန်မာစကားစွမ်းရည်) စည်းကမ်းချက်တွေနဲ့အညီ စနစ်တကျ ရေးသားထားတယ်:

* **Tone & Voice:** နေ့စဉ်ပြောနေကျ ရင်းနှီးပွင့်လင်းတဲ့ ဆရာတစ်ဦးက အနီးကပ်လမ်းညွှန်ပေးနေတဲ့ဟန် (Friendly, Mentor voice) ကို သုံးထားတယ်။ စာဖတ်သူကို "မင်း"၊ ရေးသားသူကို "ကျွန်တော်" လို့ သုံးနှုန်းပြီး စက်ရုပ်ဆန်တဲ့ ဘာသာပြန် လေသံတွေကို လုံးဝ ဖယ်ရှားထားတယ်။
* **Language & Terms:** မြန်မာစကားအသုံးအနှုန်းကို ကြွယ်ဝစွာသုံးပြီး ဖတ်ရတာ သဘာဝကျစေရမယ်။ "သည်"၊ "ဖြစ်သည်"၊ "များ"၊ "နှင့်"၊ "-ခြင်း"၊ "ရန်"၊ "မည့်" စတဲ့ စာအုပ်ကြီးဟန်တွေကို မသုံးဘဲ "တယ်"၊ "မယ်"၊ "တွေ"၊ "နဲ့"၊ "တာ"၊ "ဖို့"၊ "မယ့်" လို့ပဲ သဘာဝကျကျ သုံးတယ်။
* **Technical Jargon:** Technical terms တွေကို မြန်မာလို အတင်း လုံးဝဘာသာမပြန်ဘဲ မူရင်း English terms (ဥပမာ- State, Hook, Endpoint, Webhook, Next.js, React, GUI App, Terminal, Grep Search) တွေကိုပဲ တိုက်ရိုက် ရေးသားထားတယ်။

---

## စာအုပ်ရဲ့ ဖွဲ့စည်းတည်ဆောက်ပုံ (Table of Contents & Navigation)

စာဖတ်သူတွေနဲ့ Contributor တွေ အလွယ်တကူ ရှာဖွေဖတ်ရှုနိုင်ဖို့ (Navigate လုပ်နိုင်ဖို့) သင်ခန်းစာ အားလုံးကို အပိုင်းကြီး ၅ ပိုင်း ခွဲခြားထားပြီး သက်ဆိုင်ရာ ဖိုင်တွေဆီ တိုက်ရိုက် Link ချိတ်ဆက် ပေးထားတယ်:

### ပင်မ မိတ်ဆက်
* **[မိတ်ဆက် (Introduction)](./introduction.mdx)** - Agentic Coding ရဲ့ အနှစ်သာရ၊ Vibe Coding နဲ့ ကွာခြားပုံနဲ့ စာအုပ်ရဲ့ လမ်းညွှန် မြေပုံ။

---

### Part 1: Foundations of Agentic Coding (အခြေခံသဘောတရားတွေ)
AI Agent တွေရဲ့ အခြေခံ သဘောတရား၊ Chatbot နဲ့ ကွာခြားချက်နဲ့ Operator တစ်ယောက်ရဲ့ စိတ်နေစိတ်ထား။

* **[Chapter 1: Introduction to Agentic Coding](./chapter-1-introduction-to-agentic-coding.mdx)**
  * Agentic Coding ဆိုတာ ဘာလဲ။ Chatbot နဲ့ Autonomous Agent ကွာခြားချက်။ Software Development Lifecycle (SDLC) ထဲကို AI ဝင်ရောက်လာပုံနဲ့ Developer Anxiety (အလုပ်အကိုင် စိုးရိမ်ပူပန်မှု) ကို ကျော်လွှားပုံ။
* **[Chapter 2: The Agentic Mindset: From Vibe Coder to Operator](./chapter-2-the-agentic-mindset.mdx)**
  * ရိုးရိုး Vibe Coding ကနေ စနစ်တကျရှိတဲ့ AI Operator ဖြစ်လာအောင် စိတ်နေစိတ်ထား ပြောင်းလဲပုံ။ Junior Developer တစ်ယောက်လို အလုပ်လွှဲအပ်တဲ့ (Delegation) အနုပညာနဲ့ ၈၀/၂၀ စည်းမျဉ်းကို အသုံးချပုံ။
* **[Chapter 3: How Coding Agents Work (Under the Hood)](./chapter-3-how-coding-agents-work.mdx)**
  * Coding Agent တစ်ခုရဲ့ အတွင်းပိုင်း အလုပ်လုပ်ပုံ Primitives တွေဖြစ်တဲ့ Tools (File I/O, Grep, Terminal)၊ Planning (Step-by-step breakdown) နဲ့ State & Memory (Context Window) အကြောင်း။

---

### Part 2: Tooling & Setup (ကိရိယာတွေနဲ့ ပြင်ဆင်ခြင်း)
ခေတ်သစ် ကိရိယာတွေကို တပ်ဆင်ခြင်းနဲ့ ဘေးကင်းလုံခြုံစွာ မောင်းနှင်ပုံ။

* **[Chapter 4: Using Claude via GUI Apps & Desktop IDEs](./chapter-4-claude-code-gui.mdx)**
  * ခေတ်ဟောင်း CLI ရဲ့ အခက်အခဲတွေကို ကျော်လွှားပြီး GUI App (Desktop Applications & IDEs) တွေနဲ့ Agentic Coding ကို အသုံးချပုံ။ Workspace ဖွင့်ခြင်း၊ Screenshot drag & drop ဖြင့် Context ထည့်ခြင်းနဲ့ Visual Diff ကြည့်ရှုစစ်ဆေးခြင်း။
* **[Chapter 5: Codex & Remote GPU Coding](./chapter-5-codex-remote-gpu.mdx)** _(Coming Soon)_
  * Remote host ဒါမှမဟုတ် GPU/RunPod environment ပေါ်မှာ Codex ကို SSH နဲ့ ချိတ်ဆက်ပြီး Coding လုပ်ပုံ။ SSH Configuration၊ public key setup နဲ့ remote terminal setup။
* **[Chapter 6: Agent Safety & Permissions (လုံခြုံရေးတံခါးတွေ)](./chapter-6-agent-safety-permissions.mdx)** _(Coming Soon)_
  * Coding Agent တွေကို Terminal execution permissions ပေးတဲ့အခါ ဘေးကင်းအောင် ထိန်းကျောင်းပုံ။ Sandboxed environment၊ `rm -rf` လို destructive commands တွေကနေ ကာကွယ်ပုံနဲ့ API Keys/Credentials လုံခြုံရေး။

---

### Part 3: Instructing & Delegating (အေးဂျင့်ကို စနစ်တကျ ခိုင်းစေခြင်း)
ထိရောက်တဲ့ Prompting နည်းဗျူဟာများ၊ Work Contracts များနဲ့ Debugging loops များ။

* **[Chapter 7: Writing Work Contracts (Master System Prompting)](./chapter-7-writing-work-contracts.mdx)** _(Coming Soon)_
  * Agent ကို one-off prompt တွေ ပေးမယ့်အစား လုပ်ငန်းသဘောတူစာချုပ် (Work Contract) ပုံစံ Prompt ရေးနည်း။ `Goal`, `Context`, `Constraints`, `Operating mode` နဲ့ `Output format` တို့ကို ခွဲခြားရေးသားပုံ။
* **[Chapter 8: The Plan-Act-Verify Loop (လုပ်ငန်းစဉ် ပတ်လမ်း)](./chapter-8-plan-act-verify-loop.mdx)** _(Coming Soon)_
  * Agent နဲ့အတူ အလုပ်လုပ်တဲ့အခါ အောင်မြင်မှုရစေမယ့် အဆင့် ၃ ဆင့် Loop (Plan ရေးခိုင်းခြင်း၊ Act ကုဒ်ပြင်ခြင်း၊ Verify စမ်းသပ်စစ်ဆေးခြင်း)။
* **[Chapter 9: Handling Mistakes & Debugging Loops](./chapter-9-handling-mistakes-debugging.mdx)** _(Coming Soon)_
  * Agent က လမ်းမှားသွားတဲ့အခါ၊ ဒါမှမဟုတ် bug တွေ ထပ်ခါထပ်ခါ တက်နေတဲ့အခါ Infinite loop ကို ဖြတ်တောက်ပြီး အမှားအယွင်း logs တွေကို စနစ်တကျ ဖတ်ပြ လမ်းညွှန်ပုံ။

---

### Part 4: Quality & Verification (အရည်အသွေး ထိန်းချုပ်ခြင်း)
ကုဒ်အရည်အသွေး စံနှုန်းများနဲ့ အလိုအလျောက် စမ်းသပ်စစ်ဆေးခြင်း (Automated Testing)။

* **[Chapter 10: Coding Quality Gates (အရည်အသွေး တံခါးတွေ)](./chapter-10-coding-quality-gates.mdx)** _(Coming Soon)_
  * Code မရေးခင်နဲ့ ရေးပြီးနောက် မဖြစ်မနေ ဖြတ်သန်းရမယ့် Quality Gates တွေ။ Code linting၊ type checking နဲ့ formatting standard တွေကို AI နဲ့ ဖြေရှင်းခိုင်းပုံ။
* **[Chapter 11: Automated Verification and Testing](./chapter-11-automated-verification-testing.mdx)** _(Coming Soon)_
  * Unit tests တွေ ရေးပြီး အလုပ်ကို အလိုအလျောက် verify လုပ်ပုံ။ Python/JS testing frameworks တွေ သုံးပြီး test spec ရေးဆွဲတာနဲ့ Agent ကို test pass ဖြစ်တဲ့အထိ ပြင်ဆင်ခိုင်းပုံ။

---

### Part 5: Example Project - Build from Scratch (လက်တွေ့ App တစ်ခု ဆောက်လုပ်ခြင်း)
**Next.js & React + Telegram Bot Webhook** ကို သုံးပြီး analytics dashboard ပါဝင်တဲ့ application တစ်ခုလုံးကို အေးဂျင့်နဲ့အတူ အစကနေ အဆုံးအထိ လက်တွေ့တည်ဆောက်မယ့် အပိုင်း။

* **[Chapter 12: Next.js Telegram Bot with React Dashboard Spec & Architecture](./chapter-12-nextjs-telegram-bot-dashboard-spec.mdx)** _(Coming Soon)_
  * Telegram Bot နဲ့ web-based admin dashboard ပါဝင်မယ့် Full-stack app တစ်ခုကို design ဆွဲတာ။ Telegram Bot API architecture (Webhooks vs Polling)၊ Next.js Route Handlers နဲ့ dashboard layout spec။
* **[Chapter 13: Project Setup & Telegram Bot Integration](./chapter-13-project-setup-telegram-bot.mdx)** _(Coming Soon)_
  * Next.js application အသစ်တစ်ခု စတင်ပြီး Telegram webhook routing နဲ့ core logic တွေကို Agent နဲ့ တည်ဆောက်တာ။ Environment variables setup နဲ့ message processing logic။
* **[Chapter 14: Building the React Dashboard](./chapter-14-building-react-dashboard.mdx)** _(Coming Soon)_
  * Next.js App Router နဲ့ React Server Components/Client Components ကို သုံးပြီး bot analytics နဲ့ interaction history ပြသမယ့် user interface တစ်ခု ဆောက်လုပ်တာ။
* **[Chapter 15: Security Audit, Deployment & Post-Launch Checklist](./chapter-15-security-audit-deployment.mdx)** _(Coming Soon)_
  * Production deploy မလုပ်ခင် app ရဲ့ security စစ်ဆေးတာ၊ Vercel deployment လုပ်တာနဲ့ Agent production ready checklist။

---

## ဘယ်လို လေ့လာသင့်လဲ (How to Use This Book)

1. **အစီအစဉ်အတိုင်း ဖတ်ပါ:** အရှေ့ပိုင်းက Foundations (Part 1) နဲ့ Tooling (Part 2) ကို သေချာ နားလည်မှ ရှေ့ဆက်မယ့် လုပ်ငန်းစဉ်တွေမှာ အေးဂျင့်ကို ထိထိမိမိ မောင်းနှင်နိုင်မှာ ဖြစ်တယ်။
2. **လက်တွေ့ လိုက်လုပ်ပါ:** သက်ဆိုင်ရာ သင်ခန်းစာ တစ်ခုချင်းစီရဲ့ နောက်ဆုံးမှာ ပါဝင်တဲ့ **Checklist** မေးခွန်းတွေကို ကိုယ့်ကိုယ်ကိုယ် ပြန်မေးပြီး လက်တွေ့ အသုံးချကြည့်ပါ။
3. **Operator စိတ်နေစိတ်ထား ထားရှိပါ:** AI ဟာ အရာရာကို အလိုအလျောက် သိနေတဲ့ မှော်ဆရာ မဟုတ်ပါဘူး။ မင်းကသာ တိကျတဲ့ Spec၊ ရှင်းလင်းတဲ့ Context နဲ့ ထိရောက်တဲ့ Verification ပေးနိုင်တဲ့ Operator ကောင်း တစ်ယောက် ဖြစ်ရမယ်။
