---
lab:
  title: 'Copilot Fundamentals — Prompting Framework'
  description: 'Understand what Microsoft 365 Copilot is, how it works, and learn the four-element prompting framework used throughout this workshop.'
  duration: 30 minutes
  level: 100
  islab: false
  primarytopics:
    - Microsoft 365 Copilot
    - Prompting
---

# Copilot Fundamentals — Prompting Framework (30 min)
---

> **PPTX Reference:** This section corresponds to **Slides 8–11** of the GJ_Pepsi_Copilot_Workshop.pptx deck.

### What Is Microsoft 365 Copilot?

| Concept | Description |
|---------|-------------|
| **AI-powered assistant** | Copilot is embedded in the apps you use every day — Outlook, Teams, Excel, Word, PowerPoint. It uses large language models combined with your Microsoft 365 data. |
| **Not a search engine — a working partner** | Copilot drafts emails, analyzes data, prepares meeting briefs, creates documents and presentations — all grounded in your context. |
| **Enterprise-grade security** | Copilot inherits your existing Microsoft 365 permissions. It only accesses data you already have access to. Your prompts and data are not used to train the model. |

### Where Copilot Lives

Copilot is available in multiple places across Microsoft 365:

- **Copilot Chat** — Standalone AI chat at microsoft365.com (Web and Work modes)
- **In-app Copilot** — Built into Word, Excel, PowerPoint, Outlook, and Teams
- **Copilot in Edge** — Sidebar assistant in the browser
- **Copilot Studio** — Build custom agents grounded in your documents

---

### The Prompting Framework

Every effective Copilot prompt is built around four elements. You'll use this framework in every exercise today.

| Element | What It Does | Example |
|---------|-------------|---------|
| **Goal** | Clearly state what you want Copilot to do. | "Summarize this quarterly business review into 5 key takeaways." |
| **Context** | Provide background so Copilot understands the situation. | "I'm preparing for a leadership meeting with our regional VP." |
| **Sources** | Specify where Copilot should look for information. | "Reference the attached Q4 sales performance spreadsheet." |
| **Expectations** | Define how you want the response — tone, format, length. | "Use bullet points, keep it to one page, highlight areas below target." |

---

### Generic vs. Specific Prompts

The difference between a mediocre result and a great one comes down to prompt specificity.

**Generic prompt:**
> "Summarize this document."
>
> *Result: A vague summary that may miss what you actually need.*

**Specific prompt:**
> "Summarize this Q4 business review into 5 key takeaways for a leadership meeting. Highlight metrics below target and areas that exceeded expectations. Use bullet points."
>
> *Result: Focused, actionable summary you can present immediately.*

---

### Prompting Best Practices

1. **Be specific about what you want** — Include format, length, tone, and audience in your prompt.
2. **Iterate** — Your first prompt rarely gives the perfect result. Refine, narrow, and redirect.
3. **Attach sources** — Copilot produces much better output when grounded in real documents.
4. **Break complex requests into steps** — If a prompt is doing too much, split it into two or three prompts.
5. **Verify outputs** — Copilot is a powerful starting point, not the final answer. Always review for accuracy.

---

### How Copilot Uses Your Data

- Copilot accesses your Microsoft 365 data via **Microsoft Graph** — the same permissions model that controls who can see what in SharePoint, OneDrive, Teams, and Outlook.
- **If you can't see a file normally, Copilot can't see it either.**
- Your prompts and responses are **not used to train the model**.
- Data stays within your Microsoft 365 tenant boundary.

> [!TIP]
> Think of Copilot as a very capable new colleague who has read access to all the same files and emails you do — but who still needs clear instructions to do good work.
