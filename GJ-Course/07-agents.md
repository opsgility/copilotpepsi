---
lab:
  title: 'Exercise 7: Building Custom Agents in Copilot Studio'
  description: 'Use Copilot Studio Agent Builder to create a custom agent that answers questions using your organizational documents as knowledge sources.'
  duration: 45 minutes
  level: 200
  islab: true
  primarytopics:
    - Microsoft 365 Copilot
    - Copilot Studio
    - Agents
---

# Exercise 7: Building Custom Agents in Copilot Studio (45 min)
---

Microsoft 365 Copilot allows you to create custom agents — specialized AI assistants that answer questions using your documents as knowledge sources. Agents are built in the **Copilot Studio lite experience** (Agent Builder), which requires no programming skills.

In this exercise, you'll build an agent that helps G&J Pepsi employees answer common questions about company policies, benefits, and procedures.

---

### Task 1: Create a G&J Employee FAQ Agent (25 min)

1. In **Microsoft Edge**, navigate to [https://www.microsoft365.com](https://www.microsoft365.com).
2. Select **New agent** in the left navigation pane. This opens the **Agent Builder**.
3. In the prompt on the **New Agent** page, describe your agent:

    **Create an agent called "G&J Employee Assistant." This agent helps G&J Pepsi employees find answers to common questions about company benefits, onboarding procedures, and workplace policies. It should use a friendly, professional tone suitable for all employees from warehouse staff to corporate leadership. The agent should only answer questions using the documents provided as knowledge sources — it should not make up information. If it doesn't know the answer, it should say so and suggest who to contact.**

4. Select the **Send** icon to submit. Wait for Copilot to build the agent (1-2 minutes).

5. Select the **Configure** tab to review what Copilot created:
    - **Name** and **Description** should reflect your prompt
    - **Instructions** — Review the detailed instructions Copilot generated. These tell the agent how to behave.

6. Scroll down to **Knowledge**. Disable the **Search all websites** toggle (the agent should only use your documents). Select the **Upload from device** icon and upload these files from your OneDrive:
    - **GJ_New_Hire_Onboarding_Guide.docx**
    - **GJ_Annual_Benefits_Summary.docx**

7. Scroll to **Suggested prompts** and add these starter prompts:

    | Title | Message |
    |---|---|
    | Benefits overview | What health insurance plans are available and what do they cost? |
    | Onboarding checklist | What do I need to complete in my first 30 days as a new hire? |
    | PTO policy | How does PTO work? How many days do I get and how do I request time off? |
    | Who to contact | Who should I contact about a benefits question? |

8. Select **Create** to build the agent.

---

### Task 2: Test and refine your agent (10 min)

1. After the agent is created, select **Go to agent**.
2. Test each of the suggested prompts. Verify the agent pulls accurate information from your uploaded documents.

3. Try some additional test questions:
    - "What is the dental plan coverage?"
    - "What happens if I miss the benefits enrollment deadline?"
    - "What equipment do I receive on my first day?"
    - "Who is my HR contact?"

4. Note any questions where the agent's response is incomplete or incorrect. You'll fix these by updating the instructions.

5. To edit the agent, select the **...** (more options) icon next to the agent name in the left pane and choose **Edit**.

6. On the **Describe** tab, ask Copilot to improve the instructions:

    **Update the instructions to include: (1) When answering benefits questions, always specify the plan year (2026), (2) When the agent doesn't have enough information, direct employees to contact HR at hr@gjpepsi.com, (3) Always format answers with bullet points for readability.**

7. Select **Update** to apply the changes.

---

### Task 3: Build a department-specific agent (10 min)

Choose one scenario and build a second agent:

**HR / L&D:**
> Create a "Training Resources Agent" that helps employees find available training programs, certifications, and development opportunities. Upload the onboarding guide as a starter knowledge source.

**IT:**
> Create a "G&J IT Help Agent" that answers common IT questions — password resets, VPN access, software requests. Upload the IT infrastructure plan as a knowledge source.

**Operations:**
> Create a "Safety & Procedures Agent" that answers questions about warehouse safety protocols, incident reporting, and equipment procedures. Upload relevant documents.

**Sales:**
> Create a "Product Knowledge Agent" that helps sales reps answer questions about product lines, pricing, and promotions. Upload the quarterly business review as a starting knowledge source.

For whichever agent you build:
1. Give it a clear name and description
2. Upload at least one knowledge source document
3. Add 3-4 suggested prompts
4. Test it with 2-3 questions
5. Refine the instructions based on test results

---

### Key Concepts for Agent Building

| Concept | Description |
|---|---|
| **Knowledge sources** | Documents the agent uses to answer questions. Up to 20 files (docx, xlsx, pdf, pptx, txt). |
| **Instructions** | Rules that tell the agent how to behave — tone, format, boundaries. Max 8,000 characters. |
| **Suggested prompts** | Starter questions shown to users. Help them understand what the agent can do. |
| **"Only use specified sources"** | When enabled, the agent prioritizes your documents over general AI knowledge. |
| **Sharing** | Agents are private by default. Share with specific people or your whole organization. |

> [!TIP]
> The best agents are focused on a specific domain. An agent that tries to answer everything will answer nothing well. Start narrow, test, and expand.

