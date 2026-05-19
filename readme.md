
# MS-4019 – Finance Persona Agents

## Applied Exercise – Financial Planning & Analysis Workflows with Microsoft 365 Copilot Agents

**Session Objective:** This scenario-driven demo shows how Microsoft 365 Copilot’s prebuilt **Researcher** and **Analyst** agents, along with a custom **Copilot Chat** agent, can augment a finance professional’s workflow for tasks like budgeting, financial reporting, and compliance. In this **1-hour session**, the trainer will demonstrate the **power of Copilot** through realistic finance workflows (e.g. **financial reporting, budgeting & forecasting, variance analysis**) relevant to a finance audience. The **demos are designed to be beginner-friendly** yet exhibit clear value for finance roles, using **generic sample files** and publicly available info (no proprietary data required). Prompts and text placeholders (e.g. `[CompanyName]`, `[Finance Report]`, `[Excel File]`) can be replaced with real organization names or files to tailor the narrative. Trainers may also share a “prompt pack” of example queries for the Researcher and Analyst agents with participants, to inspire practice and discussion.

**Target Audience:** Finance managers or analysts interested in leveraging Copilot for financial planning and analysis tasks (e.g. budgeting, forecasting, variance analysis, compliance). This demo focuses on how **Copilot’s Researcher and Analyst** agents can help accelerate financial insights and how a **custom “BudgetBuddy” Copilot agent** can support budget planning inquiries.


**Before you begin this exercise, ensure you have access to:**

* **Microsoft 365 Copilot (Chat)** – with **prebuilt Researcher and Analyst agents** enabled.
* **Microsoft Copilot Studio** – to create a custom Copilot chat agent.
* **Sample data files** (provided under the `assets` folder) either uploaded into your OneDrive or attached in the Copilot Chat as needed:
  * *LastYear\_Finances.xlsx* 
  * *Q1\_Financial\_Report.pdf* 
  * *Q1\_Budget\_vs\_Actual.xlsx* 
  * *Finance\_Compliance\_Guidelines.pdf*
  * *Audit\_Readiness\_Checklist.xlsx*
  * *Budgeting\_Guidelines.pdf*

> **Note:** All sample documents provided are **fictional and for training use only**. Trainers may use these or substitute equivalent data from their own organization to increase relevance, as needed.

## Demo Scenario: **Budget Planning & Forecasting** (Finance Persona Use Case)

**Scenario Overview:** *Contoso, Inc.* (a fictional company) is planning next year’s budget. As a finance manager, you will use **Copilot** to: **(1)** gather external context on industry trends, **(2)** analyze last year’s internal financial data for trends and forecasts, and **(3)** create a custom budgeting assistant agent for ongoing Q\&A support. This end-to-end scenario highlights how Copilot can accelerate budgeting and forecasting processes for finance professionals.

### Exercise 1 — Identify Key Budgeting Trends (Researcher Agent)

Use the **Researcher** agent to gather **external industry context** relevant to budgeting.

**Steps:**

1. Open Microsoft 365 **Copilot Chat** (Teams or M365).

2. In the Copilot chat interface, expand the **Agents** menu and select **Researcher**.

3. Enter the following prompt in Copilot Chat with the Researcher agent:

   **Prompt:**

   ```text
   Our finance team is updating the 2024 budget. Research current industry trends affecting budgeting (inflation, interest rates) and recent market forecasts for our sector, and compile a summary. Use web sources and present 3 key trends with brief commentary and citations.
   ```

4. **Observe the Response:** The Researcher agent should return a summary of **3 current macro-level trends** (e.g., inflation rates, interest rate changes, economic forecasts) relevant to budgeting, each with a brief explanation and source citations. *(If prompted to narrow the search focus by industry, region, or sources, provide appropriate input and continue.)*

### Exercise 2 — Refine Insights for Budget Impact (Researcher Agent, Follow-up)

Use the **Researcher** agent to refine the results and focus on **budget-specific impacts**.

**Steps:**

1. With the Researcher agent’s reply from Exercise 1 visible, ask a follow-up question for more targeted information.

2. Enter the following (as a new prompt with Researcher):

   **Prompt:**

   ```text
   Filter that to impact on corporate budgets specifically. List any examples or stats related to cost forecasting.
   ```

3. **Observe the Response:** The Researcher agent refines the context to focus specifically on **how those trends impact corporate budgeting**, and likely provides some examples or statistics regarding **cost forecasting impacts**. The answer should be a concise list (or short paragraphs) with relevant details, preparing you for the next step of analyzing company data.

### Exercise 3 — Forecast Expenses from Historical Data (Analyst Agent)

Use the **Analyst** agent with an Excel dataset to perform a **forecast** based on last year’s financials.

**Steps:**

1. Return to the **Agents** menu in Copilot Chat and select **Analyst**.

2. Ensure the sample Excel file **LastYear\_Finances.xlsx** is accessible to Copilot (e.g., attached to the chat or stored in your OneDrive).

3. Enter the following prompt with the Analyst agent:

   **Prompt:**

   ```text
   Using the attached LastYear_Finances.xlsx, generate a forecast for 2024 quarterly expenses. Show the projected vs. actual (last year's data) in a short analysis. Include a line chart of expenses by quarter (last year actual vs. forecast).
   ```

4. **Observe the Response:** The Analyst agent reads the **LastYear\_Finances.xlsx** data, applies forecasting (e.g. extrapolating trends into 2024), and produces an **analysis of projected vs. last year’s actual expenses by quarter**. The answer should include a brief summary and may even generate a simple **line chart** comparing last year’s vs projected expenses over the four quarters (if the environment supports chart output).

   *Trainer Tip:* If the Analyst agent doesn’t automatically provide a visual, you can verbally describe the expected trend or optionally switch to Excel and use **Copilot in Excel** to generate a chart. However, the key is demonstrating the **AI-driven analysis** and trend identification, not the specific chart itself.

### Exercise 4 — Summarize Key Forecast Insights (Analyst Agent, Follow-up)

Have the **Analyst** agent provide a concise **summary insight** from the forecast results.

**Steps:**

1. Continue using the **Analyst** agent (with the forecast result from Exercise 3 visible).

2. Enter the following follow-up prompt:

   **Prompt:**

   ```text
   Give a one-paragraph takeaway from that forecast – mention the overall trend and any expected seasonal spike.
   ```

3. **Observe the Response:** The Analyst agent will distill the forecasted data into a **brief summary**, highlighting the overall trend in quarterly expenses (for example, steady growth or seasonal patterns) and any notable spikes or variations in specific quarters. This demonstrates how Copilot can help translate data into key insights for decision-makers.

### Exercise 5 — Create a Custom Budget Assistant Agent (“BudgetBuddy”)

Use **Copilot Agent Builder** to create a custom **“BudgetBuddy”** agent that can answer budgeting and planning queries, **grounded in company guidelines**.

**Steps:**

1. Open **Microsoft 365 Copilot Studio** (the interface for building custom Copilot chat agents).

2. Select **Create agent** and enter an appropriate name, e.g., **BudgetBuddy**.

3. In the **Describe** tab, enter high-level instructions for the agent’s role and style. For example:

   **Agent Instructions:**

   ```text
   You are a Budget Planning Assistant named "BudgetBuddy" for CompanyName]. You help the finance team by answering questions about budgeting timelines, guidelines, and best practices based on provided company documentation. 
   - Provide clear, concise answers focused on budgeting and forecasting. 
   - If you don’t have information in your provided sources, say so and suggest who or where to ask.
   - Always base your answers on the official Budgeting Guidelines document.
   ```

4. Switch to the **Configure** (Knowledge) tab. **Add a knowledge source** – attach **Budgeting\_Guidelines.pdf** from the `assets` folder as the agent’s content. (This document contains Contoso’s budgeting process and policies to ground the agent’s answers.)

5. Save and **Create** the agent.

### Exercise 6 — Use the “BudgetBuddy” Agent for Q\&A

Test the newly created **BudgetBuddy** agent in **Copilot Chat** by asking it a budgeting question.

**Steps:**

1. In Microsoft 365 Copilot Chat, switch to the **BudgetBuddy** agent from your agent list.

2. Ask a relevant question that the agent can answer using the budgeting guidelines. For example:

   **Prompt (to BudgetBuddy):**

   ```text
   What are the quarterly budget submission deadlines according to the guidelines?
   ```

3. **Observe the Response:** The BudgetBuddy agent should pull from the **Budgeting Guidelines** document to answer, providing the **quarterly budget submission deadlines** as specified by Contoso’s policy【5006†L21-L27】. The answer should be concise and reference the guidelines (e.g., citing that *“quarterly reforecast updates are due shortly after each quarter’s close”*).

4. (Optional) **Handling Unknown Queries:** To demonstrate how the agent behaves if asked something outside its knowledge, you can pose a follow-up question that the guidelines don’t cover. For example:

   **Prompt (to BudgetBuddy):**

   ```text
   Who can approve exceptions to the budget submission deadlines?
   ```

   Since this specific detail is likely **not covered in the guidelines**, BudgetBuddy should respond that it does not have that information and might suggest consulting the appropriate person or department for exceptions【5002†L59-L64】. This shows how the custom agent remains within the bounds of its provided knowledge and handles unanswered queries gracefully.

***

## **Additional Scenario Examples (Optional)**

After completing the primary **budget planning & forecasting** scenario above, you may explore the following **alternate finance scenarios** for further practice or demonstration. These can be used if you have extra time or want to tailor the session to specific interests (e.g., reviewing financial performance or compliance tasks). Each scenario is independent and highlights different Copilot capabilities in Finance contexts. They follow a similar format: using the **Researcher agent** for document/context summaries and the **Analyst agent** for data analysis.

### *Scenario 2: Quarterly Performance & Variance Review*

**Scenario:** A finance manager reviews the results of Q1 against the budget. Copilot helps summarize a Q1 report and analyze budget vs actual numbers to identify key variances.

**Steps & Prompts:**

1. **Researcher – Summarize Q1 Results:** *Using Researcher on a Q1 report.*  
   **Prompt:**
   ```text
   Summarize Q1 performance vs budget from the file Q1_Financial_Report.pdf. Focus on key metrics and make it concise for a quick review.
   ```
   **Outcome:** Researcher provides a brief summary of Q1’s performance versus budget, highlighting major outcomes or discrepancies in key metrics (revenues, expenses, etc.).

2. **Researcher (Follow-up) – Concise Highlights:** *Refine the summary.*  
   **Prompt:**
   ```text
   Shorten that to three bullet points highlighting the biggest takeaways from Q1.
   ```
   **Outcome:** Researcher responds with a tighter, bullet-point list of the top 3 insights from the Q1 report (e.g., biggest variance, over-performing or under-performing areas).

3. **Analyst – Identify Major Variances:** *Using Analyst on budget vs actual data.*  
   **Prompt:**
   ```text
   Using the Q1_Budget_vs_Actual.xlsx, identify the two departments with the largest budget variances (over or under budget) and provide their variance amounts and percentages.
   ```
   **Outcome:** Analyst reads the Q1 Budget vs Actual data and returns the **two largest variances** between actual and budget by department (e.g., Marketing overspent by $X, which was Y% over budget, and Operations underspent by $Z, which was W% under budget).

4. **Analyst (Follow-up) – Department Deep Dive:** *Focus on a specific department’s variance.*  
   **Prompt:**
   ```text
   Zoom in on the Marketing department: what was its budget variance in dollars and percentage?
   ```
   **Outcome:** Analyst filters or calculates the **Marketing department’s specific variance** from the Q1 budget vs actual data, providing the dollar amount and percentage over/under budget. This demonstrates how to quickly drill into a particular area of interest using follow-up questions.

### *Scenario 3: Audit Preparation & Compliance Checks*

**Scenario:** With an audit coming up, a finance team member uses Copilot to review compliance guidelines and check an audit readiness checklist for outstanding tasks.

**Steps & Prompts:**

1. **Researcher – Summarize Compliance Guidelines:** *Use Researcher on a policy document.*  
   **Prompt:**
   ```text
   Summarize the key points from the Finance Compliance Guidelines.pdf, focusing on any new policies or deadlines introduced.
   ```
   **Outcome:** Researcher returns a summary of the critical points from the compliance guidelines, highlighting recent changes or upcoming deadlines.

2. **Analyst – Analyze Audit Checklist:** *Use Analyst on an audit checklist spreadsheet.*  
   **Prompt:**
   ```text
   Using the Audit_Readiness_Checklist.xlsx, count the number of incomplete tasks in each category and list any high-priority tasks that are still open.
   ```
   **Outcome:** Analyst reviews the checklist data and provides **counts of incomplete tasks per category**, as well as highlighting any tasks marked high-priority that remain unfinished. This shows how Copilot can quickly parse through compliance checklists or task trackers to surface important information.

***

## **Wrap-Up & Next Steps**

**Key Takeaways:** This Finance persona demo illustrated how Copilot’s **prebuilt** and **custom** agents can streamline finance workflows from planning to compliance. The scenario(s) above demonstrated obtaining external insights for financial context, analyzing and visualizing historical data for forecasting, summarizing financial reports and guidelines, and building a tailored Q\&A agent for budgeting support. Trainers should emphasize how these tools **reduce manual analysis time, enhance data-driven decision-making, and ensure alignment with corporate policies**.

**After completing this exercise, participants should be able to:**

* Use the **Researcher** agent to gather **industry and market insights** relevant to financial decisions.
* Use the **Analyst** agent to analyze financial data (e.g., budgets vs actuals) and generate forecasts with visualizations.
* Quickly generate concise **summaries of financial documents** (reports, guidelines) to extract key points.
* Create and use a **custom Copilot agent** (e.g., **“BudgetBuddy”**) by providing it with company-specific knowledge (like budgeting policies) for **specialized Q\&A support**.
* Understand how Copilot agents can be integrated into everyday **finance tasks** (budget planning, performance review, compliance checks) to **save time and improve insights**.

**Repository Usage:** This repository contains all materials and instructions needed to conduct the Finance Persona demo. Clone or download the repo, then **open the README.md** for step-by-step guidance. Ensure you have the sample files from the `assets` folder readily accessible (either uploaded to your Microsoft 365 environment or attached to the Copilot chat as needed) when running through the demo prompts. Adjust the provided prompts or replace sample files with your organization’s data as desired, to make the scenario more relatable to your audience.
